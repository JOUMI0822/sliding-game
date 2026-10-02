/**
 * Sliding Maze V29 - Supabase Account + Daily/Weekly Ranking Server
 *
 * Supabase tables expected:
 * accounts:
 *   id, nickname, password_hash, created_at
 *
 * game_scores:
 *   id, account_id, clears, max_streak, skips, life_losses, score, created_at
 *
 * Score:
 * clears * 50 + maxStreak * 100 - skips * 10 - lifeLosses * 10
 *
 * IMPORTANT:
 * - Accounts and scores are stored in Supabase, not local files.
 * - The server does NOT use accounts.json anymore.
 * - Session cookies are signed, so a Render restart does not erase login sessions.
 * - For cross-site GitHub Pages -> Render cookies, SameSite=None + Secure is used.
 */
"use strict";

const express = require("express");
const http = require("http");
const { WebSocketServer } = require("ws");
const crypto = require("crypto");
const path = require("path");

const app = express();
const PORT = Number(process.env.PORT || 3000);
const SESSION_DAYS = Math.max(1, Number(process.env.SESSION_DAYS || 30));
const SUPABASE_URL = String(process.env.SUPABASE_URL || "").replace(/\/$/, "");
const SUPABASE_SERVICE_ROLE_KEY = String(process.env.SUPABASE_SERVICE_ROLE_KEY || "");
const ALLOWED_ORIGIN = String(
  process.env.ALLOWED_ORIGIN || "https://joumi0822.github.io"
).replace(/\/$/, "");

if (!SUPABASE_URL || !SUPABASE_SERVICE_ROLE_KEY) {
  console.error("Missing SUPABASE_URL or SUPABASE_SERVICE_ROLE_KEY.");
  process.exit(1);
}

// A stable server-side secret is required for sessions to survive Render restarts.
// If SESSION_SECRET is not set, the Supabase service-role key is used as a fallback.
// The service-role key never leaves this server.
const SESSION_SECRET = String(
  process.env.SESSION_SECRET || SUPABASE_SERVICE_ROLE_KEY
);

const SCORE_FORMULA =
  "clears * 50 + maxStreak * 100 - skips * 10 - lifeLosses * 10";

const SUPABASE_REST = `${SUPABASE_URL}/rest/v1`;

app.disable("x-powered-by");
app.use(express.json({ limit: "16kb" }));

/* =========================================================
   Request / CORS diagnostics
   - Logs request method/path/origin without passwords or tokens.
   - Adds a request id so one login attempt can be traced in Render logs.
========================================================= */

function makeRequestId() {
  return crypto.randomBytes(6).toString("hex");
}

app.use((req, res, next) => {
  const requestId = String(req.headers["x-request-id"] || req.headers["rndr-id"] || makeRequestId());
  const origin = String(req.headers.origin || "(none)");

  req.requestId = requestId;
  res.setHeader("X-Request-Debug-Id", requestId);

  console.log(`[HTTP ${requestId}] ${req.method} ${req.path} origin=${origin}`);

  res.on("finish", () => {
    console.log(`[HTTP ${requestId}] RESPONSE ${res.statusCode} ${req.method} ${req.path}`);
  });

  next();
});

/* =========================================================
   CORS
========================================================= */

app.use((req, res, next) => {
  const origin = req.headers.origin;
  const requestId = req.requestId || "unknown";

  if (origin && origin === ALLOWED_ORIGIN) {
    res.setHeader("Access-Control-Allow-Origin", origin);
    res.setHeader("Vary", "Origin");
    res.setHeader("Access-Control-Allow-Credentials", "true");
    res.setHeader("Access-Control-Allow-Headers", "Content-Type, Authorization, X-Requested-With, Cache-Control, Pragma");
    res.setHeader("Access-Control-Allow-Methods", "GET,POST,OPTIONS");
    res.setHeader("Access-Control-Max-Age", "600");
    console.log(`[CORS ${requestId}] ALLOWED origin=${origin}`);
  } else if (origin) {
    console.warn(`[CORS ${requestId}] BLOCKED origin=${origin} expected=${ALLOWED_ORIGIN}`);
  } else {
    console.log(`[CORS ${requestId}] NO_ORIGIN`);
  }

  if (req.method === "OPTIONS") {
    console.log(`[CORS ${requestId}] PREFLIGHT method=${req.headers["access-control-request-method"] || "(none)"} headers=${req.headers["access-control-request-headers"] || "(none)"}`);
    return res.status(204).end();
  }

  next();
});

/* =========================================================
   Basic helpers
========================================================= */

function normalizeId(value) {
  return String(value || "").trim().toLowerCase();
}

function normalizeNickname(value) {
  return String(value || "").trim().toLowerCase();
}

function validId(value) {
  return /^[A-Za-z0-9_]{3,24}$/.test(value);
}

function validNickname(value) {
  return (
    value.length >= 2 &&
    value.length <= 16 &&
    !/[\u0000-\u001F\u007F]/.test(value)
  );
}

function hashPassword(password, salt = crypto.randomBytes(16).toString("hex")) {
  return {
    salt,
    hash: crypto.scryptSync(String(password), salt, 64).toString("hex")
  };
}

function verifyPassword(password, storedValue) {
  try {
    const stored =
      typeof storedValue === "string"
        ? JSON.parse(storedValue)
        : storedValue;

    if (!stored || !stored.salt || !stored.hash) return false;

    const actual = Buffer.from(
      hashPassword(String(password), stored.salt).hash,
      "hex"
    );
    const expected = Buffer.from(String(stored.hash), "hex");

    return (
      actual.length === expected.length &&
      crypto.timingSafeEqual(actual, expected)
    );
  } catch (_) {
    return false;
  }
}

function calculateScore(clears, maxStreak, skips, lifeLosses) {
  const c = Math.max(0, Math.min(100000, Math.floor(Number(clears) || 0)));
  const s = Math.max(0, Math.min(c, Math.floor(Number(maxStreak) || 0)));
  const k = Math.max(0, Math.min(100000, Math.floor(Number(skips) || 0)));
  const l = Math.max(0, Math.min(100000, Math.floor(Number(lifeLosses) || 0)));

  return Math.max(0, c * 50 + s * 100 - k * 10 - l * 10);
}

function escapeSupabaseValue(value) {
  return encodeURIComponent(String(value));
}

/* =========================================================
   Supabase REST helper
========================================================= */

async function supabaseRequest(table, options = {}) {
  const url = `${SUPABASE_REST}/${table}${options.query || ""}`;

  const headers = {
    apikey: SUPABASE_SERVICE_ROLE_KEY,
    Authorization: `Bearer ${SUPABASE_SERVICE_ROLE_KEY}`,
    "Content-Type": "application/json",
    ...(options.headers || {})
  };

  const response = await fetch(url, {
    method: options.method || "GET",
    headers,
    body: options.body === undefined ? undefined : JSON.stringify(options.body)
  });

  const text = await response.text();
  let data = null;

  try {
    data = text ? JSON.parse(text) : null;
  } catch (_) {
    data = text;
  }

  if (!response.ok) {
    const message =
      data?.message ||
      data?.hint ||
      data?.details ||
      data?.error_description ||
      `Supabase request failed (${response.status})`;

    const error = new Error(String(message));
    error.status = response.status;
    error.supabase = data;
    throw error;
  }

  return data;
}

async function selectOneAccountById(id) {
  const rows = await supabaseRequest("accounts", {
    query: `?select=id,nickname,password_hash,created_at&id=eq.${escapeSupabaseValue(id)}&limit=1`
  });
  return Array.isArray(rows) && rows.length ? rows[0] : null;
}

async function selectAccountByNickname(nickname) {
  const rows = await supabaseRequest("accounts", {
    query: `?select=id,nickname,password_hash,created_at&nickname=ilike.${escapeSupabaseValue(nickname)}&limit=1`
  });
  return Array.isArray(rows) && rows.length ? rows[0] : null;
}

/* =========================================================
   Signed session cookie

   Format:
     base64url(JSON payload).base64url(HMAC-SHA256)

   Because the token is signed and contains the account id + expiry,
   it does not need an in-memory session Map. Render restarts therefore
   do not erase login sessions.
========================================================= */

const SESSION_COOKIE = "sliding_session";

function signSessionPayload(payloadText) {
  return crypto
    .createHmac("sha256", SESSION_SECRET)
    .update(payloadText)
    .digest("base64url");
}

function createSessionToken(accountId) {
  const payload = {
    accountId,
    exp: Date.now() + SESSION_DAYS * 86400000
  };

  const payloadText = Buffer.from(JSON.stringify(payload)).toString("base64url");
  const signature = signSessionPayload(payloadText);
  return `${payloadText}.${signature}`;
}

function parseSessionToken(token) {
  try {
    const parts = String(token || "").split(".");
    if (parts.length !== 2) return null;

    const [payloadText, signature] = parts;
    const expected = signSessionPayload(payloadText);
    const a = Buffer.from(signature);
    const b = Buffer.from(expected);

    if (a.length !== b.length || !crypto.timingSafeEqual(a, b)) {
      return null;
    }

    const payload = JSON.parse(
      Buffer.from(payloadText, "base64url").toString("utf8")
    );

    if (!payload?.accountId || Number(payload.exp) <= Date.now()) {
      return null;
    }

    return payload;
  } catch (_) {
    return null;
  }
}

function parseCookies(header) {
  const output = {};

  String(header || "")
    .split(";")
    .forEach(part => {
      const index = part.indexOf("=");
      if (index < 0) return;

      const key = part.slice(0, index).trim();
      let value = part.slice(index + 1).trim();

      try {
        value = decodeURIComponent(value);
      } catch (_) {}

      output[key] = value;
    });

  return output;
}

function getSessionPayload(req) {
  const cookies = parseCookies(req.headers.cookie);
  return parseSessionToken(cookies[SESSION_COOKIE]);
}

function setSessionCookie(res, token) {
  const maxAge = SESSION_DAYS * 86400;

  res.setHeader(
    "Set-Cookie",
    [
      `${SESSION_COOKIE}=${encodeURIComponent(token)}`,
      "HttpOnly",
      "Secure",
      "SameSite=None",
      `Max-Age=${maxAge}`,
      "Path=/"
    ].join("; ")
  );
}

function clearSessionCookie(res) {
  res.setHeader(
    "Set-Cookie",
    [
      `${SESSION_COOKIE}=`,
      "HttpOnly",
      "Secure",
      "SameSite=None",
      "Max-Age=0",
      "Path=/"
    ].join("; ")
  );
}

async function requireAuth(req, res, next) {
  try {
    const session = getSessionPayload(req);

    if (!session) {
      return res.status(401).json({ error: "로그인이 필요합니다." });
    }

    const account = await selectOneAccountById(session.accountId);

    if (!account) {
      clearSessionCookie(res);
      return res.status(401).json({ error: "계정을 찾을 수 없습니다." });
    }

    req.session = session;
    req.account = account;
    next();
  } catch (error) {
    console.error("AUTH ERROR:", error);
    res.status(500).json({ error: "계정 정보를 확인하지 못했습니다." });
  }
}

/* =========================================================
   Korea/Seoul date helpers

   Daily/weekly ranking is based on Korea Standard Time so the
   ranking changes at midnight in Korea rather than at UTC midnight.
========================================================= */

const KST_TIME_ZONE = "Asia/Seoul";

function getKstParts(date = new Date()) {
  const parts = new Intl.DateTimeFormat("en-US", {
    timeZone: KST_TIME_ZONE,
    year: "numeric",
    month: "2-digit",
    day: "2-digit",
    weekday: "short",
    hour: "2-digit",
    minute: "2-digit",
    second: "2-digit",
    hourCycle: "h23"
  }).formatToParts(date);

  const map = {};
  for (const part of parts) map[part.type] = part.value;

  return {
    year: Number(map.year),
    month: Number(map.month),
    day: Number(map.day),
    weekday: map.weekday,
    hour: Number(map.hour),
    minute: Number(map.minute),
    second: Number(map.second)
  };
}

function dateKey(date = new Date()) {
  const p = getKstParts(date);
  return `${p.year}-${String(p.month).padStart(2, "0")}-${String(p.day).padStart(2, "0")}`;
}

function kstMidnightUtc(date = new Date()) {
  const p = getKstParts(date);

  // KST is UTC+09:00.
  return new Date(
    Date.UTC(p.year, p.month - 1, p.day) - 9 * 60 * 60 * 1000
  );
}

function startOfWeekKst(date = new Date()) {
  const midnight = kstMidnightUtc(date);
  const p = getKstParts(midnight);
  const weekdayNumber = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"].indexOf(p.weekday);
  const daysFromMonday = weekdayNumber === 0 ? 6 : weekdayNumber - 1;
  return new Date(midnight.getTime() - daysFromMonday * 86400000);
}

function weekKey(date = new Date()) {
  return dateKey(startOfWeekKst(date));
}

function nextDayUtc(date) {
  return new Date(date.getTime() + 86400000);
}

/* =========================================================
   Health
========================================================= */

app.get("/api/health", (req, res) => {
  res.json({
    ok: true,
    version: "V29",
    dailyRanking: true,
    weeklyRanking: true,
    scoreFormula: SCORE_FORMULA,
    supabaseUrl: "FOUND",
    supabaseServiceRoleKey: "FOUND",
    allowedOrigin: ALLOWED_ORIGIN
  });
});

/* =========================================================
   Register
========================================================= */

app.post("/api/register", async (req, res) => {
  try {
    const id = normalizeId(req.body?.id);
    const nickname = String(req.body?.nickname || "").trim();
    const password = String(req.body?.password || "");

    if (!validId(id)) {
      return res
        .status(400)
        .json({ error: "아이디는 영문/숫자/_ 3~24자로 입력해주세요." });
    }

    if (password.length < 8 || password.length > 72) {
      return res
        .status(400)
        .json({ error: "비밀번호는 8~72자로 입력해주세요." });
    }

    if (!validNickname(nickname)) {
      return res
        .status(400)
        .json({ error: "닉네임은 2~16자로 입력해주세요." });
    }

    const existingId = await selectOneAccountById(id);
    if (existingId) {
      return res.status(409).json({ error: "이미 사용 중인 아이디입니다." });
    }

    const existingNickname = await selectAccountByNickname(nickname);
    if (existingNickname) {
      return res.status(409).json({ error: "이미 사용 중인 닉네임입니다." });
    }

    const passwordHash = JSON.stringify(hashPassword(password));

    const rows = await supabaseRequest("accounts", {
      method: "POST",
      query: "?select=id,nickname,created_at",
      headers: {
        Prefer: "return=representation"
      },
      body: {
        id,
        nickname,
        password_hash: passwordHash
      }
    });

    const account = Array.isArray(rows) ? rows[0] : rows;

    if (!account?.id) {
      throw new Error("계정 저장 결과를 확인하지 못했습니다.");
    }

    const token = createSessionToken(account.id);
    setSessionCookie(res, token);

    return res.json({
      ok: true,
      user: {
        id: account.id,
        nickname: account.nickname
      }
    });
  } catch (error) {
    console.error("REGISTER ERROR:", error);

    // PostgreSQL unique violation
    if (error?.supabase?.code === "23505") {
      return res.status(409).json({ error: "이미 사용 중인 아이디 또는 닉네임입니다." });
    }

    return res.status(500).json({
      error: "회원가입 저장 중 오류가 발생했습니다."
    });
  }
});

/* =========================================================
   Login
========================================================= */

app.post("/api/login", async (req, res) => {
  const requestId = req.requestId || "unknown";

  try {
    const id = normalizeId(req.body?.id);
    const password = String(req.body?.password || "");

    console.log(`[LOGIN ${requestId}] START id=${id || "(empty)"} passwordLength=${password.length}`);

    if (!id || !password) {
      console.warn(`[LOGIN ${requestId}] BAD_INPUT idPresent=${!!id} passwordPresent=${!!password}`);
      return res.status(400).json({ error: "아이디와 비밀번호를 입력해주세요." });
    }

    const account = await selectOneAccountById(id);
    console.log(`[LOGIN ${requestId}] ACCOUNT_FOUND=${!!account}`);

    if (!account) {
      console.warn(`[LOGIN ${requestId}] ACCOUNT_NOT_FOUND id=${id}`);
      return res
        .status(401)
        .json({ error: "아이디 또는 비밀번호가 올바르지 않습니다." });
    }

    const passwordValid = verifyPassword(password, account.password_hash);
    console.log(`[LOGIN ${requestId}] PASSWORD_VALID=${passwordValid}`);

    if (!passwordValid) {
      console.warn(`[LOGIN ${requestId}] PASSWORD_MISMATCH id=${id}`);
      return res
        .status(401)
        .json({ error: "아이디 또는 비밀번호가 올바르지 않습니다." });
    }

    const token = createSessionToken(account.id);
    setSessionCookie(res, token);

    console.log(`[LOGIN ${requestId}] SUCCESS accountId=${account.id} nickname=${account.nickname}`);

    return res.json({
      ok: true,
      user: {
        id: account.id,
        nickname: account.nickname
      }
    });
  } catch (error) {
    console.error(`[LOGIN ${requestId}] ERROR`, error);
    console.error(`[LOGIN ${requestId}] ERROR_MESSAGE`, error?.message || String(error));
    if (error?.supabase) {
      console.error(`[LOGIN ${requestId}] SUPABASE_ERROR`, JSON.stringify(error.supabase));
    }
    return res.status(500).json({ error: "로그인 처리 중 오류가 발생했습니다." });
  }
});

/* =========================================================
   Current session
========================================================= */

app.get("/api/me", requireAuth, async (req, res) => {
  try {
    const progress = await selectAccountProgress(req.account.id);

    res.json({
      id: req.account.id,
      nickname: req.account.nickname,
      level: progress?.level ?? 1,
      exp: progress?.exp ?? 0
    });
  } catch (error) {
    console.error("[ME] progress lookup failed", error);
    res.json({
      id: req.account.id,
      nickname: req.account.nickname,
      level: 1,
      exp: 0
    });
  }
});

/* =========================================================
   Level / EXP
   - level 1 requires 100 EXP
   - each next level requires +50 EXP
========================================================= */

function getLevelRequiredExp(level) {
  const lv = Math.max(1, Math.floor(Number(level) || 1));
  return 100 + (lv - 1) * 50;
}

function normalizeAccountProgress(level, exp) {
  let lv = Math.max(1, Math.floor(Number(level) || 1));
  let xp = Math.max(0, Math.floor(Number(exp) || 0));

  while (xp >= getLevelRequiredExp(lv)) {
    xp -= getLevelRequiredExp(lv);
    lv++;
  }

  return { level: lv, exp: xp };
}

async function selectAccountProgress(accountId) {
  const rows = await supabaseRequest("accounts", {
    query: `?select=id,level,exp&id=eq.${escapeSupabaseValue(accountId)}&limit=1`
  });

  if (!Array.isArray(rows) || !rows.length) return null;

  return normalizeAccountProgress(rows[0].level, rows[0].exp);
}

app.get("/api/progress", requireAuth, async (req, res) => {
  try {
    const progress = await selectAccountProgress(req.account.id);

    if (!progress) {
      return res.status(404).json({ error: "계정을 찾을 수 없습니다." });
    }

    res.json(progress);
  } catch (error) {
    console.error("[EXP] GET progress failed", error);
    res.status(500).json({ error: "EXP 정보를 불러오지 못했습니다." });
  }
});

app.post("/api/progress/award", requireAuth, async (req, res) => {
  try {
    const rawAmount = Number(req.body?.amount);

    if (!Number.isFinite(rawAmount) || rawAmount <= 0) {
      return res.status(400).json({ error: "잘못된 EXP 값입니다." });
    }

    // 한 번의 결과 화면에서 비정상적으로 큰 값이 들어오는 것을 방지.
    const amount = Math.min(10000, Math.floor(rawAmount));

    const current = await selectAccountProgress(req.account.id);

    if (!current) {
      return res.status(404).json({ error: "계정을 찾을 수 없습니다." });
    }

    let level = current.level;
    let exp = current.exp;
    let remaining = amount;

    while (remaining > 0) {
      const required = getLevelRequiredExp(level);
      const add = Math.min(remaining, required - exp);

      exp += add;
      remaining -= add;

      if (exp >= required) {
        level++;
        exp = 0;
      }
    }

    const progress = normalizeAccountProgress(level, exp);

    await supabaseRequest("accounts", {
      method: "PATCH",
      query: `?id=eq.${escapeSupabaseValue(req.account.id)}`,
      headers: {
        Prefer: "return=minimal"
      },
      body: {
        level: progress.level,
        exp: progress.exp
      }
    });

    res.json({
      awarded: amount,
      level: progress.level,
      exp: progress.exp,
      saved: true
    });
  } catch (error) {
    console.error("[EXP] POST award failed", error);
    if (error?.supabase) {
      console.error("[EXP] SUPABASE_ERROR", JSON.stringify(error.supabase));
    }
    res.status(500).json({ error: "EXP 저장에 실패했습니다." });
  }
});

/* =========================================================
   Logout
========================================================= */

app.post("/api/logout", (req, res) => {
  clearSessionCookie(res);
  res.json({ ok: true });
});

/* =========================================================
   Score validation / insertion
========================================================= */

function parseScoreBody(body) {
  const clears = Number(body?.clears);
  const maxStreak = Number(body?.maxStreak);
  const skips = Number(body?.skips);
  const lifeLosses = Number(body?.lifeLosses);

  if (![clears, maxStreak, skips, lifeLosses].every(Number.isFinite)) {
    return null;
  }

  const c = Math.max(0, Math.min(100000, Math.floor(clears)));
  const s = Math.max(0, Math.min(c, Math.floor(maxStreak)));
  const k = Math.max(0, Math.min(100000, Math.floor(skips)));
  const l = Math.max(0, Math.min(100000, Math.floor(lifeLosses)));
  const score = calculateScore(c, s, k, l);

  return {
    clears: c,
    max_streak: s,
    skips: k,
    life_losses: l,
    score
  };
}

/* =========================================================
   Submit score

   Every finished game is stored in game_scores. Ranking endpoints
   aggregate the best score per account for the requested period.
========================================================= */

app.post("/api/ranking/score", requireAuth, async (req, res) => {
  try {
    const score = parseScoreBody(req.body);

    if (!score) {
      return res.status(400).json({ error: "잘못된 게임 기록입니다." });
    }

    const rows = await supabaseRequest("game_scores", {
      method: "POST",
      query: "?select=id,account_id,clears,max_streak,skips,life_losses,score,created_at",
      headers: {
        Prefer: "return=representation"
      },
      body: {
        id: crypto.randomUUID(),
        account_id: req.account.id,
        clears: score.clears,
        max_streak: score.max_streak,
        skips: score.skips,
        life_losses: score.life_losses,
        score: score.score
      }
    });

    const saved = Array.isArray(rows) ? rows[0] : rows;

    res.json({
      saved: true,
      score: score.score,
      record: saved || score
    });
  } catch (error) {
    console.error("SCORE SAVE ERROR:", error);
    res.status(500).json({ error: "랭킹 점수를 저장하지 못했습니다." });
  }
});

/* =========================================================
   Ranking aggregation
========================================================= */

function betterScore(a, b) {
  if (!a) return b;
  if (!b) return a;

  if (b.score !== a.score) return b.score > a.score ? b : a;
  if (b.max_streak !== a.max_streak) return b.max_streak > a.max_streak ? b : a;
  if (b.clears !== a.clears) return b.clears > a.clears ? b : a;
  if (b.life_losses !== a.life_losses) return b.life_losses < a.life_losses ? b : a;
  if (b.skips !== a.skips) return b.skips < a.skips ? b : a;
  return new Date(b.created_at).getTime() < new Date(a.created_at).getTime() ? b : a;
}

function sortRanking(rows) {
  return rows.sort((a, b) => {
    if (b.score !== a.score) return b.score - a.score;
    if (b.max_streak !== a.max_streak) return b.max_streak - a.max_streak;
    if (b.clears !== a.clears) return b.clears - a.clears;
    if (a.life_losses !== b.life_losses) return a.life_losses - b.life_losses;
    if (a.skips !== b.skips) return a.skips - b.skips;
    return String(a.nickname).localeCompare(String(b.nickname), "ko");
  });
}

function aggregateBestScores(scores, accountsById) {
  const best = new Map();

  for (const score of scores) {
    const accountId = String(score.account_id);
    const account = accountsById.get(accountId);
    if (!account) continue;

    const row = {
      accountId,
      nickname: account.nickname,
      score: Number(score.score) || 0,
      clears: Number(score.clears) || 0,
      maxStreak: Number(score.max_streak) || 0,
      skips: Number(score.skips) || 0,
      lifeLosses: Number(score.life_losses) || 0,
      created_at: score.created_at
    };

    best.set(accountId, betterScore(best.get(accountId), row));
  }

  return sortRanking([...best.values()]);
}

async function getScoresBetween(startInclusive, endExclusive) {
  return supabaseRequest("game_scores", {
    query:
      `?select=id,account_id,clears,max_streak,skips,life_losses,score,created_at` +
      `&created_at=gte.${escapeSupabaseValue(startInclusive.toISOString())}` +
      `&created_at=lt.${escapeSupabaseValue(endExclusive.toISOString())}` +
      `&order=score.desc&limit=10000`
  });
}

async function getAccountsForScoreRows(scores) {
  const ids = [...new Set(scores.map(row => String(row.account_id)).filter(Boolean))];
  const map = new Map();

  // Supabase's REST URL length can become large, so fetch in small batches.
  for (let i = 0; i < ids.length; i += 50) {
    const batch = ids.slice(i, i + 50);
    if (!batch.length) continue;

    const filter = batch
      .map(id => `"${String(id).replace(/"/g, '\\"')}"`)
      .join(",");

    const rows = await supabaseRequest("accounts", {
      query: `?select=id,nickname&id=in.(${encodeURIComponent(filter)})`
    });

    for (const account of Array.isArray(rows) ? rows : []) {
      map.set(String(account.id), account);
    }
  }

  return map;
}

async function buildRanking(scope) {
  const now = new Date();
  let start;
  let end;

  if (scope === "weekly") {
    start = startOfWeekKst(now);
    end = new Date(start.getTime() + 7 * 86400000);
  } else {
    start = kstMidnightUtc(now);
    end = nextDayUtc(start);
  }

  const scores = await getScoresBetween(start, end);
  const accountsById = await getAccountsForScoreRows(scores);
  return aggregateBestScores(scores, accountsById);
}

function publicRanking(rows, accountId) {
  return rows.slice(0, 100).map((row, index) => ({
    rank: index + 1,
    nickname: row.nickname,
    score: row.score,
    clears: row.clears,
    maxStreak: row.maxStreak,
    skips: row.skips,
    lifeLosses: row.lifeLosses,
    me: row.accountId === String(accountId)
  }));
}

/* =========================================================
   Today ranking
========================================================= */

app.get("/api/ranking/today", requireAuth, async (req, res) => {
  try {
    const rows = await buildRanking("daily");
    const mineIndex = rows.findIndex(
      row => row.accountId === String(req.account.id)
    );

    res.json({
      date: dateKey(),
      ranking: publicRanking(rows, req.account.id),
      mine:
        mineIndex >= 0
          ? { rank: mineIndex + 1, ...rows[mineIndex] }
          : null
    });
  } catch (error) {
    console.error("DAILY RANKING ERROR:", error);
    res.status(500).json({ error: "오늘 랭킹을 불러오지 못했습니다." });
  }
});

/* =========================================================
   Weekly ranking
========================================================= */

app.get("/api/ranking/weekly", requireAuth, async (req, res) => {
  try {
    const rows = await buildRanking("weekly");
    const mineIndex = rows.findIndex(
      row => row.accountId === String(req.account.id)
    );

    const weekStart = startOfWeekKst(new Date());
    const weekEnd = new Date(weekStart.getTime() + 6 * 86400000);

    res.json({
      week: weekKey(),
      weekEnds: dateKey(weekEnd),
      ranking: publicRanking(rows, req.account.id),
      mine:
        mineIndex >= 0
          ? { rank: mineIndex + 1, ...rows[mineIndex] }
          : null
    });
  } catch (error) {
    console.error("WEEKLY RANKING ERROR:", error);
    res.status(500).json({ error: "주간 랭킹을 불러오지 못했습니다." });
  }
});

/* =========================================================
   My daily record
========================================================= */

app.get("/api/ranking/me", requireAuth, async (req, res) => {
  try {
    const rows = await buildRanking("daily");
    const mineIndex = rows.findIndex(
      row => row.accountId === String(req.account.id)
    );

    res.json({
      record: mineIndex >= 0 ? rows[mineIndex] : null,
      rank: mineIndex >= 0 ? mineIndex + 1 : null
    });
  } catch (error) {
    console.error("MY DAILY RANKING ERROR:", error);
    res.status(500).json({ error: "내 랭킹을 불러오지 못했습니다." });
  }
});

/* =========================================================
   My weekly record
========================================================= */

app.get("/api/ranking/weekly/me", requireAuth, async (req, res) => {
  try {
    const rows = await buildRanking("weekly");
    const mineIndex = rows.findIndex(
      row => row.accountId === String(req.account.id)
    );

    res.json({
      record: mineIndex >= 0 ? rows[mineIndex] : null,
      rank: mineIndex >= 0 ? mineIndex + 1 : null
    });
  } catch (error) {
    console.error("MY WEEKLY RANKING ERROR:", error);
    res.status(500).json({ error: "내 주간 랭킹을 불러오지 못했습니다." });
  }
});

/* =========================================================
   Static files / fallback

   Express 5 does not accept app.get("*") because path-to-regexp
   requires a named wildcard. Use middleware instead.
========================================================= */

app.use(express.static(__dirname));

app.use((req, res, next) => {
  if (req.method !== "GET") return next();

  const indexPath = path.join(__dirname, "index.html");
  res.sendFile(indexPath, error => {
    if (error) next(error);
  });
});

app.use((error, req, res, next) => {
  console.error("SERVER ERROR:", error);
  if (res.headersSent) return next(error);
  res.status(500).json({ error: "서버 오류가 발생했습니다." });
});

/* =========================================================
   V29 Multiplayer WebSocket relay
   The frontend connects to wss://sliding-multiplayer-server-1.onrender.com
   and sends: matchmake / create / join / matchStart / position / finish / eliminated.
========================================================= */

const httpServer = http.createServer(app);
const wss = new WebSocketServer({ server: httpServer });

const quickQueue = [];
const rooms = new Map();
const socketState = new Map();

function wsSend(ws, payload) {
  if (!ws || ws.readyState !== 1) return;
  try { ws.send(JSON.stringify(payload)); } catch (_) {}
}

function removeFromQueue(ws) {
  for (let i = quickQueue.length - 1; i >= 0; i--) {
    if (quickQueue[i] === ws) quickQueue.splice(i, 1);
  }
}

function makeRoomState(room, host, guest, type) {
  return {
    room,
    host,
    guest,
    type,
    round: 0,
    finishes: new Map(),
    eliminated: new Map(),
    lastStart: null
  };
}

function peerOf(room, ws) {
  if (!room) return null;
  return room.host === ws ? room.guest : room.host;
}

function roomFor(ws) {
  const state = socketState.get(ws);
  return state?.room ? rooms.get(state.room) : null;
}

function notifyPeerLeft(room, leaving) {
  const peer = peerOf(room, leaving);
  if (peer) {
    wsSend(peer, { type: "peerLeft" });
    setTimeout(() => {
      if (peer.readyState === 1) wsSend(peer, { type: "playerLeftTimeout", winner: socketState.get(peer)?.role || "draw" });
    }, 10000);
  }
}

function attachRoom(ws, room, role) {
  socketState.set(ws, { room: room.room, role });
  if (role === "host") room.host = ws;
  else room.guest = ws;
}

function finishRoom(room) {
  if (!room) return;
  rooms.delete(room.room);
  if (room.host) socketState.delete(room.host);
  if (room.guest) socketState.delete(room.guest);
}

function pairQuickMatch(a, b) {
  const roomCode = `Q${Math.random().toString(36).slice(2, 9).toUpperCase()}`;
  const room = makeRoomState(roomCode, a, b, "quick");
  rooms.set(roomCode, room);
  attachRoom(a, room, "host");
  attachRoom(b, room, "guest");
  wsSend(a, { type: "matchFound", role: "host" });
  wsSend(b, { type: "matchFound", role: "guest" });
}

wss.on("connection", ws => {
  socketState.set(ws, { room: null, role: null });

  ws.on("message", raw => {
    let data;
    try { data = JSON.parse(raw.toString()); } catch (_) {
      wsSend(ws, { type: "error", message: "잘못된 WebSocket 메시지입니다." });
      return;
    }

    const state = socketState.get(ws) || { room: null, role: null };

    if (data.type === "matchmake") {
      removeFromQueue(ws);
      const other = quickQueue.shift();
      if (other && other.readyState === 1 && other !== ws) pairQuickMatch(other, ws);
      else {
        quickQueue.push(ws);
        socketState.set(ws, { room: null, role: null, queued: true });
        wsSend(ws, { type: "queued" });
      }
      return;
    }

    if (data.type === "create") {
      const roomCode = String(data.room || "").trim().toUpperCase();
      if (!/^[A-Z0-9]{5}$/.test(roomCode)) {
        wsSend(ws, { type: "error", message: "방 코드가 올바르지 않습니다." });
        return;
      }
      if (rooms.has(roomCode)) {
        wsSend(ws, { type: "error", message: "이미 사용 중인 방 코드입니다." });
        return;
      }
      const room = makeRoomState(roomCode, ws, null, "friend");
      rooms.set(roomCode, room);
      attachRoom(ws, room, "host");
      wsSend(ws, { type: "roomCreated", room: roomCode });
      return;
    }

    if (data.type === "join") {
      const roomCode = String(data.room || "").trim().toUpperCase();
      const room = rooms.get(roomCode);
      if (!room || !room.host) {
        wsSend(ws, { type: "error", message: "존재하지 않는 방입니다." });
        return;
      }
      if (room.guest && room.guest !== ws) {
        wsSend(ws, { type: "error", message: "방이 이미 가득 찼습니다." });
        return;
      }
      attachRoom(ws, room, "guest");
      wsSend(ws, { type: "roomJoined", room: roomCode });
      wsSend(room.host, { type: "peerJoined" });
      return;
    }

    const room = roomFor(ws);
    if (!room) {
      wsSend(ws, { type: "error", message: "먼저 빠른 대전이나 방에 참가해주세요." });
      return;
    }

    if (data.type === "position") {
      wsSend(peerOf(room, ws), data);
      return;
    }

    if (data.type === "matchStart") {
      if (state.role !== "host") return;
      room.round = Number(data.round) || room.round + 1;
      room.finishes.clear();
      room.eliminated.clear();
      room.lastStart = data;
      wsSend(room.guest, data);
      return;
    }

    if (data.type === "finish") {
      const round = Number(data.round) || room.round;
      room.finishes.set(state.role, data);
      const otherRole = state.role === "host" ? "guest" : "host";
      if (room.finishes.has(otherRole)) {
        const winner = state.role;
        const nextStart = data.position || room.finishes.get(otherRole)?.position || { c: 1, r: 1 };
        const payload = { type: "roundWon", round, winner, nextStart };
        wsSend(room.host, payload);
        wsSend(room.guest, payload);
        room.finishes.clear();
        room.eliminated.clear();
      }
      return;
    }

    if (data.type === "eliminated") {
      const round = Number(data.round) || room.round;
      room.eliminated.set(state.role, data);
      const otherRole = state.role === "host" ? "guest" : "host";
      if (Number(data.livesRemaining) <= 0) {
        if (room.finishes.has(otherRole)) {
          const payload = { type: "roundWon", round, winner: otherRole, nextStart: room.finishes.get(otherRole)?.position || { c: 1, r: 1 } };
          wsSend(room.host, payload);
          wsSend(room.guest, payload);
          room.finishes.clear(); room.eliminated.clear();
        } else {
          wsSend(peerOf(room, ws), { type: "roundWon", round, winner: otherRole, nextStart: data.position || { c: 1, r: 1 } });
          wsSend(ws, { type: "roundWon", round, winner: otherRole, nextStart: data.position || { c: 1, r: 1 } });
          room.finishes.clear(); room.eliminated.clear();
        }
      }
      return;
    }
  });

  ws.on("close", () => {
    removeFromQueue(ws);
    const room = roomFor(ws);
    if (room) {
      notifyPeerLeft(room, ws);
      finishRoom(room);
    }
    socketState.delete(ws);
  });
});

httpServer.listen(PORT, () => {
  console.log(`Sliding Maze V29 backend running on port ${PORT}`);
  console.log("[ENV CHECK] SUPABASE_URL: FOUND");
  console.log("[ENV CHECK] SUPABASE_SERVICE_ROLE_KEY: FOUND");
  console.log(`[ENV CHECK] ALLOWED_ORIGIN: ${ALLOWED_ORIGIN}`);
  console.log("Daily ranking: ON");
  console.log("Weekly ranking: ON (Monday-Sunday, Asia/Seoul)");
  console.log(`Score: ${SCORE_FORMULA}`);
  console.log("WebSocket multiplayer: ON");
});

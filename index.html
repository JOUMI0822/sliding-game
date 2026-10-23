<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>슬라이딩</title>

<style>
* {
    box-sizing: border-box;
}

html,
html,
body {
    width: 100%;
    min-height: 100%;
    margin: 0;
    overscroll-behavior: none;
}

html.login-lock,
body.login-lock {
    overflow: hidden !important;
    position: fixed;
    width: 100%;
    height: 100%;
}

body {
    margin: 0;
    padding: 0;
    width: 100%;
    min-height: 100%;
    background: #0b0e13;
    color: #f2f5f7;
    font-family: "Pretendard","Noto Sans KR",Arial,sans-serif;
}

body {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    width: 100%;
    min-height: 100vh;
    height: 100dvh;
    overflow: hidden;
    overscroll-behavior: none;
    touch-action: none;
}

#gameWrapper {
    width: 800px;
    max-width: 100vw;
    min-height: 100vh;
    min-height: 100dvh;
    padding-bottom: 15px;
    touch-action: none;
    overscroll-behavior: none;
}

.topbar {
    width: 800px;
    max-width: 100vw;
    min-height: 44px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 8px;
    padding: 7px 10px;
    background: #151a22;
    border: 1px solid #29303b;
    border-bottom: none;
    font-size: 14px;
    font-weight: 600;
}

.topbar > div {
    white-space: nowrap;
}

#equippedItemBox {
    width: 185px;
    height: 30px;
    min-width: 185px;
    border: 1px solid #46515f;
    border-radius: 9px;
    background: #10151c;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 1px;
    line-height: 1;
    overflow: hidden;
}

#itemInfo {
    width: 100%;
    color: #b8f0ff;
    font-size: 11px;
    text-align: center;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    padding: 0 6px;
}

#itemWarning {
    width: 100%;
    color: #ffbd66;
    font-size: 8px;
    min-height: 0;
    text-align: center;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    padding: 0 4px;
}

#time {
    color: #f4f6f8;
}

#lives {
    color: #ff6672;
}

#clears {
    color: #7ddcff;
}

#score {
    color: #ffd76a;
    font-weight: 800;
}

#mapSkips {
    color: #d9c7ff;
    letter-spacing: 1px;
}

canvas {
    display: block;
    width: 800px;
    height: 600px;
    max-width: 100vw;
    border: 1px solid #29303b;
    background: #0f1319;
    touch-action: none;
}

#canvasStage {
    position: relative;
    width: 800px;
    max-width: 100vw;
    aspect-ratio: 4 / 3;
    line-height: 0;
    touch-action: none;
}

#canvasStage > canvas {
    width: 100%;
    height: 100%;
    max-width: none;
}

#questRewardOverlay {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 100;
    touch-action: none;
}

#questRewardOverlay .quest-reward-button {
    position: absolute;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0;
    margin: 0;
    border: 2px solid rgba(99,184,255,0.95);
    border-radius: 7px;
    background: rgba(99,184,255,0.18);
    color: #fff;
    font: bold 12px Pretendard, "Noto Sans KR", sans-serif;
    line-height: 1;
    cursor: pointer;
    pointer-events: auto;
    touch-action: manipulation;
    -webkit-tap-highlight-color: rgba(99,184,255,0.25);
    -webkit-appearance: none;
    appearance: none;
    box-shadow: 0 0 8px rgba(99,184,255,0.45);
    user-select: none;
    -webkit-user-select: none;
}

#questRewardOverlay .quest-reward-button:active {
    background: rgba(99,184,255,0.34);
    transform: scale(0.98);
}

#questRewardOverlay .quest-reward-button:focus-visible {
    outline: 3px solid rgba(255,215,106,0.9);
    outline-offset: 2px;
}

@media (max-width:820px) {
    .topbar {
        font-size: 10px;
        gap: 4px;
        padding: 6px 5px;
        min-height: 50px;
    }

    #equippedItemBox {
        width: 25vw;
        min-width: 92px;
        max-width: 150px;
        height: 30px;
        border-radius: 8px;
    }

    #itemInfo {
        font-size: 8px;
    }

    #itemWarning {
        font-size: 6px;
    }

    canvas {
        width: 100vw;
        height: auto;
        aspect-ratio: 4 / 3;
    }
}




/* =========================================================
   V28 로그인 / 회원가입 / 게스트 / 랭킹 UI
========================================================= */

.entry-screen {
    position: fixed;
    inset: 0;
    z-index: 10000;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100%;
    padding: 24px;
    box-sizing: border-box;
    background:
        radial-gradient(circle at 50% 20%, rgba(75,163,255,0.12), transparent 35%),
        #0b0e13;
    overflow: hidden;
    overscroll-behavior: none;
    touch-action: none;
    -webkit-overflow-scrolling: auto;
}

.entry-screen.session-checking {
    visibility: hidden;
    pointer-events: none;
}

.entry-card {
    width: min(420px, 92vw);
    padding: 30px 28px 26px;
    border: 1px solid #394352;
    border-radius: 20px;
    background: rgba(23,28,37,0.98);
    box-shadow: 0 24px 80px rgba(0,0,0,0.45);
}

.entry-title {
    text-align: center;
    color: #f3f5f7;
    font-size: 30px;
    font-weight: 800;
    margin-bottom: 8px;
}

.entry-subtitle {
    text-align: center;
    color: #8f9aa8;
    font-size: 14px;
    margin-bottom: 22px;
}

.entry-form {
    display: grid;
    gap: 10px;
}

.entry-form input {
    width: 100%;
    height: 46px;
    border: 1px solid #46515f;
    border-radius: 10px;
    background: #10151c;
    color: #f3f5f7;
    padding: 0 13px;
    font: 500 15px Pretendard, "Noto Sans KR", Arial, sans-serif;
    outline: none;
}

.entry-form input:focus {
    border-color: #63b8ff;
    box-shadow: 0 0 0 3px rgba(99,184,255,0.12);
}

.entry-form button,
.entry-card > button {
    width: 100%;
    height: 46px;
    border-radius: 10px;
    cursor: pointer;
    font: 700 15px Pretendard, "Noto Sans KR", Arial, sans-serif;
    touch-action: manipulation;
    -webkit-tap-highlight-color: transparent;
}

.remember-login {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    gap: 7px;
    margin: -2px 0 2px;
    color: #9ca8b5;
    font-size: 12px;
    cursor: pointer;
}

.remember-login input {
    width: 15px;
    height: 15px;
    margin: 0;
    accent-color: #63b8ff;
}

.entry-primary {
    border: 1px solid rgba(99,184,255,0.75);
    background: #236ea8;
    color: #fff;
}

.entry-secondary {
    border: 1px solid #46515f;
    background: #1b222c;
    color: #f0f3f6;
}

.entry-guest {
    margin-top: 10px;
    border: 1px solid rgba(125,255,157,0.45);
    background: rgba(80,160,100,0.16);
    color: #9dffb4;
}

.entry-divider {
    display: flex;
    align-items: center;
    gap: 10px;
    margin: 18px 0 12px;
    color: #697584;
    font-size: 12px;
}

.entry-divider::before,
.entry-divider::after {
    content: "";
    flex: 1;
    height: 1px;
    background: #303844;
}

.entry-divider span {
    flex: none;
}

.entry-status {
    min-height: 20px;
    margin-top: 10px;
    text-align: center;
    color: #aeb8c5;
    font-size: 12px;
    line-height: 1.5;
}

.entry-status.error {
    color: #ff8f9b;
}

.entry-status.success {
    color: #7dff9d;
}

#startMenuOverlay {
    position: absolute;
    inset: 0;
    z-index: 150;
    pointer-events: none;
    display: none;
}

#startMenuOverlay.visible {
    display: block;
}

.start-menu-actions {
    position: absolute;
    top: 12px;
    left: 12px;
    right: auto;
    display: block;
    pointer-events: none;
}

.start-menu-account {
    position: static;
    width: 240px;
    max-width: 240px;
    padding: 6px 9px 7px;
    border: 1px solid rgba(255,255,255,0.14);
    border-radius: 9px;
    background: rgba(9,12,17,0.68);
    color: #cbd4dc;
    font-size: 12px;
    line-height: 1.2;
    pointer-events: none;
}

.start-account-main { display:flex; align-items:center; gap:6px; min-width:0; }
.start-account-level { flex:0 0 auto; color:#ffd76a; font-size:11px; font-weight:800; }
.start-account-name { min-width:0; overflow:hidden; text-overflow:ellipsis; white-space:nowrap; }
.start-account-exp { width:100%; height:5px; margin-top:5px; overflow:hidden; border-radius:999px; background:rgba(255,255,255,0.10); }
.start-account-exp-fill { width:0%; height:100%; border-radius:inherit; background:linear-gradient(90deg,#63b8ff,#7ddcff); transition:width .18s ease; }
.start-account-exp-text { margin-top:3px; color:#7f8b99; font-size:8px; text-align:right; white-space:nowrap; }

.start-menu-competitive {
    position: absolute;
    top: 50px;
    right: 12px;
    pointer-events: auto;
}

.start-menu-ranking {
    position: absolute;
    top: 8px;
    right: 12px;
    pointer-events: auto;
}

.start-menu-logout {
    position: absolute;
    right: 12px;
    bottom: 12px;
    pointer-events: auto;
}

.start-menu-button {
    min-width: 92px;
    height: 34px;
    padding: 0 10px;
    border: 1px solid rgba(255,255,255,0.14);
    border-radius: 9px;
    background: rgba(9,12,17,0.68);
    color: #cbd4dc;
    font: 700 12px Pretendard, "Noto Sans KR", Arial, sans-serif;
    box-shadow: inset 0 1px 0 rgba(255,255,255,0.025);
    cursor: pointer;
    touch-action: manipulation;
}

.start-menu-button:active {
    transform: scale(0.98);
}

.ranking-modal {
    display: none !important;
    position: fixed;
    inset: 0;
    z-index: 11000;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
    background: rgba(0,0,0,0.72);
    touch-action: auto;
    pointer-events: auto;
}

.ranking-modal.ranking-open {
    display: flex !important;
}

.ranking-card {
    width: min(760px, 96vw);
    max-height: min(720px, 92vh);
    padding: 20px;
    border: 1px solid #3c4858;
    border-radius: 18px;
    background: #151b24;
    box-shadow: 0 24px 80px rgba(0,0,0,0.55);
    overflow: auto;
}

.ranking-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    color: #f3f5f7;
    font-size: 26px;
    font-weight: 800;
}

.modal-close {
    width: 36px;
    height: 36px;
    border: 1px solid #46515f;
    border-radius: 9px;
    background: #10151c;
    color: #fff;
    font-size: 24px;
    line-height: 1;
    cursor: pointer;
}

.ranking-account-label {
    margin-top: 6px;
    color: #8f9aa8;
    font-size: 12px;
}

.ranking-tabs {
    display: flex;
    gap: 8px;
    margin: 18px 0 10px;
}

.ranking-tab {
    flex: 1;
    height: 40px;
    border: 1px solid #46515f;
    border-radius: 9px;
    background: #10151c;
    color: #aeb8c5;
    font: 700 14px Pretendard, "Noto Sans KR", Arial, sans-serif;
    cursor: pointer;
}

.ranking-tab.active {
    border-color: rgba(99,184,255,0.75);
    background: rgba(99,184,255,0.16);
    color: #eaf6ff;
}

.ranking-status {
    min-height: 22px;
    margin-bottom: 6px;
    color: #aeb8c5;
    text-align: center;
    font-size: 12px;
}

.ranking-table-wrap {
    overflow-x: auto;
}

.ranking-table {
    width: 100%;
    border-collapse: collapse;
    font-size: 13px;
}

.ranking-table th,
.ranking-table td {
    padding: 10px 8px;
    border-bottom: 1px solid rgba(255,255,255,0.07);
    text-align: center;
    white-space: nowrap;
}

.ranking-table th {
    color: #8f9aa8;
    font-size: 11px;
}

.ranking-table td {
    color: #e7edf2;
}

.ranking-table {
    table-layout: fixed;
}

.ranking-table th:nth-child(1),
.ranking-table td:nth-child(1) {
    width: 10%;
    text-align: center !important;
}

.ranking-table th:nth-child(2),
.ranking-table td:nth-child(2) {
    width: 14%;
    text-align: center !important;
    font-variant-numeric: tabular-nums;
}

.ranking-table th:nth-child(3),
.ranking-table td:nth-child(3) {
    width: 24%;
    text-align: center !important;
    overflow: hidden;
    text-overflow: ellipsis;
}

.ranking-table th:nth-child(4),
.ranking-table td:nth-child(4) {
    width: 18%;
    text-align: center !important;
}

.ranking-table th:nth-child(5),
.ranking-table td:nth-child(5) {
    width: 17%;
    text-align: center !important;
}

.ranking-table th:nth-child(6),
.ranking-table td:nth-child(6) {
    width: 17%;
    text-align: center !important;
}

@media (max-width: 520px) {
    .entry-card {
        padding: 24px 20px 22px;
    }

  .start-menu-account {
        width: 150px;
        max-width: 150px;
        padding: 5px 7px 6px;
        font-size: 10px;
    }
    .start-account-level { font-size:9px; }
    .start-account-exp-text { font-size:7px; }

    .start-menu-actions {
        top: 8px;
        left: 8px;
        right: auto;
    }

    .start-menu-ranking {
        top: 8px;
        right: 8px;
    }

    .start-menu-competitive {
        top: 50px;
        right: 8px;
    }

    .start-menu-logout {
        right: 8px;
        bottom: 8px;
    }

    .start-menu-button {
        min-width: 78px;
        height: 31px;
        font-size: 10px;
    }
}



/* 로그아웃 확인용 커스텀 대화상자 */
#logoutConfirmOverlay {
    position: fixed;
    inset: 0;
    z-index: 10010;   /* 프로필/상점 위에 확인창이 뜨도록 */
    display: none;
    align-items: center;
    justify-content: center;
    padding: 20px;
    background: rgba(0,0,0,0.62);
    touch-action: none;
}

#logoutConfirmOverlay.visible {
    display: flex;
}

#logoutConfirmDialog {
    width: min(360px, calc(100vw - 40px));
    padding: 24px 22px 20px;
    border: 1px solid #394352;
    border-radius: 18px;
    background: #171c25;
    box-shadow: 0 18px 50px rgba(0,0,0,0.45);
    text-align: center;
}

#logoutConfirmDialogTitle {
    margin: 0 0 10px;
    color: #ffffff;
    font-size: 21px;
    font-weight: 700;
}

#logoutConfirmDialogMessage {
    margin: 0 0 20px;
    color: #aeb8c5;
    font-size: 15px;
    line-height: 1.5;
}

.logout-confirm-actions {
    display: flex;
    gap: 10px;
}

.logout-confirm-actions button {
    flex: 1;
    min-height: 44px;
    border: 1px solid #46515f;
    border-radius: 10px;
    font: 600 14px Pretendard, Noto Sans KR, sans-serif;
    cursor: pointer;
    touch-action: manipulation;
}

#logoutCancelButton {
    color: #dfe5ea;
    background: #222934;
}

#logoutConfirmButton {
    color: #ffffff;
    background: #b83b49;
    border-color: #d15a67;
}


/* 튜토리얼 버튼 / 확인창 줄바꿈 / 레벨 보상 모달 */
#logoutConfirmDialogMessage { white-space: pre-line; }

.start-menu-tutorial {
    position: absolute;
    right: 12px;
    bottom: 12px;
    pointer-events: auto;
}

@media (max-width: 520px) {
    .start-menu-tutorial { right: 8px; bottom: 8px; }
}

#levelRewardOverlay {
    position: fixed;
    inset: 0;
    z-index: 10001;
    display: none;
    align-items: center;
    justify-content: center;
    padding: 20px;
    background: rgba(0,0,0,0.68);
    touch-action: none;
}

#levelRewardOverlay.visible { display: flex; }

#levelRewardDialog {
    width: min(380px, calc(100vw - 40px));
    max-height: 86vh;
    overflow: auto;
    padding: 24px 22px 20px;
    border: 1px solid #4b596b;
    border-radius: 18px;
    background: #171c25;
    box-shadow: 0 18px 50px rgba(0,0,0,0.5);
    text-align: center;
}

#levelRewardTitle { margin: 0 0 6px; color: #ffd76a; font-size: 22px; font-weight: 800; }
#levelRewardSubtitle { margin: 0 0 14px; color: #aeb8c5; font-size: 14px; line-height: 1.5; }

#levelRewardList {
    display: grid;
    gap: 8px;
    margin-bottom: 18px;
}

.level-reward-row {
    padding: 10px 12px;
    border: 1px solid rgba(255,255,255,0.12);
    border-radius: 10px;
    background: rgba(255,255,255,0.045);
    color: #f1f4f7;
    font-size: 15px;
    font-weight: 600;
}

.level-reward-row.special { border-color: rgba(255,215,106,0.55); color: #ffd76a; }

#levelRewardOkButton {
    width: 100%;
    min-height: 44px;
    border: 1px solid rgba(99,184,255,0.75);
    border-radius: 10px;
    background: #236ea8;
    color: #fff;
    font: 700 15px Pretendard, Noto Sans KR, sans-serif;
    cursor: pointer;
    touch-action: manipulation;
}

/* ---------- 프로필 박스 클릭 가능 + 레벨 보상표 ---------- */
.start-menu-account {
    pointer-events: auto;
    cursor: pointer;
    -webkit-tap-highlight-color: transparent;
    touch-action: manipulation;
}
.start-menu-account:active { background: rgba(30,40,55,0.85); }
.start-account-chevron { flex:0 0 auto; margin-left:auto; color:#7f8b99; font-size:13px; line-height:1; }

#rewardListOverlay {
    position: fixed;
    inset: 0;
    z-index: 10000;
    display: none;
    align-items: center;
    justify-content: center;
    padding: 20px;
    background: rgba(0,0,0,0.68);
    touch-action: none;
}
#rewardListOverlay.visible { display: flex; }

#rewardListDialog {
    width: min(420px, calc(100vw - 32px));
    max-height: 86vh;
    display: flex;
    flex-direction: column;
    padding: 20px 18px 16px;
    border: 1px solid #4b596b;
    border-radius: 18px;
    background: #171c25;
    box-shadow: 0 18px 50px rgba(0,0,0,0.5);
}
#rewardListTitle { margin: 0 0 4px; color: #ffd76a; font-size: 21px; font-weight: 800; text-align: center; }
#rewardListSubtitle { margin: 0 0 12px; color: #aeb8c5; font-size: 13px; text-align: center; line-height: 1.5; }

#rewardListBody {
    position: relative;
    flex: 1 1 auto;
    min-height: 120px;
    overflow-y: auto;
    overscroll-behavior: contain;
    touch-action: pan-y;
    -webkit-overflow-scrolling: touch;
    display: grid;
    gap: 6px;
    align-content: start;
    margin-bottom: 14px;
    padding-right: 2px;
}
.reward-list-row {
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 9px 12px;
    border: 1px solid rgba(255,255,255,0.12);
    border-radius: 10px;
    background: rgba(255,255,255,0.045);
    color: #f1f4f7;
    font-size: 14px;
}
.reward-list-level { flex: 0 0 62px; font-weight: 800; color: #7ddcff; }
.reward-list-items { flex: 1 1 auto; display: flex; flex-wrap: wrap; gap: 4px 10px; font-weight: 600; }
.reward-list-state { flex: 0 0 auto; font-size: 11px; color: #7f8b99; }
.reward-list-row.done { opacity: 0.42; }
.reward-list-row.done .reward-list-state { color: #7dff9d; }
.reward-list-row.current { border-color: rgba(99,184,255,0.85); background: rgba(99,184,255,0.14); }
.reward-list-row.next { border-color: rgba(255,215,106,0.65); background: rgba(255,215,106,0.08); }
.reward-list-row.next .reward-list-state { color: #ffd76a; }
.reward-list-row.special .reward-list-level { color: #ffd76a; }
.reward-list-message { padding: 24px 8px; text-align: center; color: #aeb8c5; font-size: 14px; }

#rewardListCloseButton {
    width: 100%;
    min-height: 44px;
    border: 1px solid rgba(99,184,255,0.75);
    border-radius: 10px;
    background: #236ea8;
    color: #fff;
    font: 700 15px Pretendard, Noto Sans KR, sans-serif;
    cursor: pointer;
    touch-action: manipulation;
}

/* ---------- 레벨 보상표: 아래→위 상승 + 세로 레벨 게이지 ---------- */
#rewardListBody { display: block; }
.reward-track {
    position: relative;
    display: grid;
    gap: 6px;
    align-content: start;
    padding-left: 38px;
}
.reward-gauge {
    position: absolute;
    left: 11px;
    width: 10px;
    border-radius: 6px;
    background: rgba(255,255,255,0.12);
    overflow: hidden;
}
.reward-gauge-fill {
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: 6px;
    background: linear-gradient(0deg, #3b8fd9, #7ddcff);
    transition: height .5s ease;
}
.reward-tick {
    position: absolute;
    left: 7px;
    width: 18px;
    height: 2px;
    border-radius: 1px;
    background: rgba(255,255,255,0.28);
    transform: translateY(-1px);
}
.reward-tick.reached { background: #bfeeff; }
.reward-tick.big { left: 4px; width: 24px; height: 3px; transform: translateY(-1.5px); }
.reward-now {
    position: absolute;
    left: 6px;
    width: 20px;
    height: 20px;
    margin-top: -10px;
    border-radius: 50%;
    background: #ffd76a;
    box-shadow: 0 0 10px rgba(255,215,106,0.85);
    border: 2px solid #171c25;
    z-index: 2;
}
.reward-list-row.start .reward-list-level { color: #9eabb9; }
.reward-list-row.start .reward-list-items { color: #9eabb9; font-weight: 500; }

/* ---------- 프로필 창: 탭 / 내 정보 / 닉네임 변경 ---------- */
.profile-tabs { display:flex; gap:8px; margin-bottom:12px; }
.profile-tab {
    flex:1; height:38px; border:1px solid #46515f; border-radius:9px;
    background:#10151c; color:#aeb8c5;
    font:700 13px Pretendard, "Noto Sans KR", Arial, sans-serif;
    cursor:pointer; touch-action:manipulation;
}
.profile-tab.active { border-color:rgba(99,184,255,0.75); background:rgba(99,184,255,0.16); color:#eaf6ff; }
.profile-section-title { margin:2px 2px 8px; color:#ffd76a; font-size:13px; font-weight:800; }
.profile-stat-grid { display:grid; grid-template-columns:1fr 1fr; gap:8px; margin-bottom:16px; }
.profile-stat {
    display:flex; flex-direction:column; gap:4px; padding:10px 12px;
    border:1px solid rgba(255,255,255,0.12); border-radius:10px; background:rgba(255,255,255,0.045);
}
.profile-stat span { color:#9eabb9; font-size:11px; }
.profile-stat b { color:#f1f4f7; font-size:17px; }
.profile-stat.wide { grid-column:1 / -1; }
.profile-stat.win b { color:#7dff9d; }
.profile-stat.loss b { color:#ff8f9b; }
.profile-stat.rate b { color:#7ddcff; }
.profile-nick-box {
    display:grid; gap:8px; padding:12px;
    border:1px solid rgba(255,255,255,0.12); border-radius:10px; background:rgba(255,255,255,0.045);
}
.profile-nick-current { color:#c5ced8; font-size:13px; }
.profile-nick-current b { color:#fff; }
.profile-nick-box input {
    width:100%; height:42px; border:1px solid #46515f; border-radius:9px;
    background:#10151c; color:#f3f5f7; padding:0 12px;
    font:500 14px Pretendard, "Noto Sans KR", Arial, sans-serif; outline:none;
}
.profile-nick-box input:focus { border-color:#63b8ff; }
.profile-nick-box input:disabled { opacity:0.5; }
.profile-nick-box button {
    height:42px; border:1px solid rgba(99,184,255,0.75); border-radius:9px;
    background:#236ea8; color:#fff; font:700 14px Pretendard, "Noto Sans KR", Arial, sans-serif;
    cursor:pointer; touch-action:manipulation;
}
.profile-nick-box button:disabled { opacity:0.45; cursor:default; }
.profile-nick-note { min-height:18px; color:#9eabb9; font-size:12px; line-height:1.5; text-align:center; }
.profile-nick-note.error { color:#ff8f9b; }
.profile-nick-note.success { color:#7dff9d; }
.profile-stat-grid + .profile-reset-box { margin-top:-8px; }
.profile-reset-box { display:grid; gap:6px; margin-bottom:16px; }
.profile-reset-box button {
    height:38px; border:1px solid rgba(255,143,155,0.6); border-radius:9px;
    background:rgba(184,59,73,0.25); color:#ffd0d5;
    font:700 13px Pretendard, "Noto Sans KR", Arial, sans-serif;
    cursor:pointer; touch-action:manipulation;
}
.profile-reset-box button:disabled { opacity:0.45; cursor:default; }

/* ---------- 모바일 가로 모드: 게임 전체(상단바+캔버스+오버레이)를 통째로 축소 ---------- */
/* html.fit-scale 클래스는 JS(fitGameToViewport)가 화면이 낮을 때만 붙입니다. */
html.fit-scale body {
    align-items: center;
    overflow: hidden;
}

html.fit-scale #gameWrapper {
    position: fixed;
    left: 50%;
    top: 50%;
    width: 800px;
    max-width: none;
    height: 644px;          /* 상단바 44 + 캔버스 600 */
    min-height: 0;
    padding: 0;
    transform: translate(-50%, -50%) scale(var(--fit-scale, 1));
    transform-origin: center center;
}

html.fit-scale #gameWrapper[hidden] {
    display: none;
}

html.fit-scale .topbar {
    width: 800px;
    max-width: none;
    min-height: 44px;
    padding: 7px 10px;
    gap: 8px;
    font-size: 14px;
}

html.fit-scale #equippedItemBox {
    width: 185px;
    min-width: 185px;
    max-width: none;
    height: 30px;
}

html.fit-scale #itemInfo { font-size: 11px; }
html.fit-scale #itemWarning { font-size: 8px; }

html.fit-scale #canvasStage {
    width: 800px;
    max-width: none;
    height: 600px;
    aspect-ratio: auto;
}

html.fit-scale #canvasStage > canvas,
html.fit-scale canvas {
    width: 800px;
    height: 600px;
    max-width: none;
}

/* 게스트 이름 입력창 */
#guestNameOverlay {
    position: fixed; inset: 0; z-index: 10002;
    display: none; align-items: center; justify-content: center;
    padding: 20px; background: rgba(0,0,0,0.68); touch-action: none;
}
#guestNameOverlay.visible { display: flex; }
#guestNameDialog {
    width: min(380px, calc(100vw - 40px));
    padding: 24px 22px 20px;
    border: 1px solid #4b596b; border-radius: 18px;
    background: #171c25; box-shadow: 0 18px 50px rgba(0,0,0,0.5);
    text-align: center;
}
#guestNameDialog h2 { margin: 0 0 8px; color: #fff; font-size: 21px; font-weight: 700; }
#guestNameDialog p { margin: 0 0 14px; color: #aeb8c5; font-size: 14px; line-height: 1.5; }
#guestNameInput {
    width: 100%; height: 46px; border: 1px solid #46515f; border-radius: 10px;
    background: #10151c; color: #f3f5f7; padding: 0 13px; text-align: center;
    font: 600 17px Pretendard, "Noto Sans KR", Arial, sans-serif; outline: none;
}
#guestNameInput:focus { border-color: #63b8ff; box-shadow: 0 0 0 3px rgba(99,184,255,0.12); }
#guestNameError { min-height: 20px; margin: 8px 0 12px; color: #ff8f9b; font-size: 12px; }
#guestNameDialog .logout-confirm-actions button { color: #fff; background: #222934; }
#guestNameOk { background: #236ea8 !important; border-color: rgba(99,184,255,0.75) !important; }

/* ---------- 로딩 화면 / 팁 ---------- */
#loadingOverlay {
    position: fixed; inset: 0; z-index: 10050;
    display: none; align-items: center; justify-content: center;
    padding: 24px;
    background: radial-gradient(circle at 50% 28%, rgba(75,163,255,0.16), transparent 46%), #0b0e13;
    touch-action: none; cursor: pointer;
    user-select: none; -webkit-user-select: none;
    -webkit-tap-highlight-color: transparent;
}
#loadingOverlay.visible { display: flex; }
#loadingInner { width: min(520px, 100%); text-align: center; }
#loadingTitle { color: #f3f5f7; font-size: 26px; font-weight: 800; margin-bottom: 26px; }
#loadingTipCard {
    min-height: 150px; padding: 24px 22px 20px;
    border: 1px solid #394352; border-radius: 18px;
    background: rgba(23,28,37,0.96);
    box-shadow: 0 18px 60px rgba(0,0,0,0.45);
    display: flex; flex-direction: column; align-items: center; justify-content: center; gap: 12px;
}
#loadingTipCard.swap { animation: loadingTipIn .28s ease; }
@keyframes loadingTipIn { from { opacity: 0; transform: translateY(8px); } to { opacity: 1; transform: none; } }
#loadingTipLabel { color: #ffd76a; font-size: 13px; font-weight: 800; letter-spacing: 1px; }
#loadingTipText { color: #e7edf2; font-size: 18px; font-weight: 600; line-height: 1.6; word-break: keep-all; }
#loadingTipCount { color: #697584; font-size: 12px; }
#loadingHint { margin-top: 14px; color: #8f9aa8; font-size: 13px; }
#loadingBar { margin: 22px auto 0; width: min(360px, 80%); height: 6px; border-radius: 999px; background: rgba(255,255,255,0.10); overflow: hidden; }
#loadingBarFill { width: 0; height: 100%; border-radius: inherit; background: linear-gradient(90deg, #63b8ff, #7ddcff); }
@keyframes loadingFill { from { width: 0; } to { width: 100%; } }
#loadingStatus { margin-top: 10px; color: #7f8b99; font-size: 12px; }

/* ---------- 게임 종료 / 포기 확인 팝업 ---------- */
#gamePopupOverlay {
    position: fixed; inset: 0; z-index: 10020;
    display: none; align-items: center; justify-content: center;
    padding: 20px; background: rgba(0,0,0,0.55); touch-action: none;
}
#gamePopupOverlay.visible { display: flex; }
#gamePopupDialog {
    width: min(360px, calc(100vw - 40px));
    padding: 24px 22px 20px;
    border: 1px solid #394352; border-radius: 18px;
    background: #171c25; box-shadow: 0 18px 50px rgba(0,0,0,0.45);
    text-align: center;
}
#gamePopupTitle { margin: 0 0 10px; color: #fff; font-size: 21px; font-weight: 700; }
#gamePopupMessage { margin: 0 0 8px; color: #aeb8c5; font-size: 15px; line-height: 1.5; }
#gamePopupMessage:empty { display: none; }
#gamePopupNote { margin: 0 0 18px; color: #8f9aa8; font-size: 12px; line-height: 1.5; }
.game-popup-actions { display: flex; gap: 10px; }
.game-popup-actions button {
    flex: 1; min-height: 46px; border-radius: 10px;
    font: 700 14px Pretendard, "Noto Sans KR", sans-serif;
    color: #fff; cursor: pointer; touch-action: manipulation;
}
#gamePopupConfirm { background: #b83b49; border: 1px solid #d15a67; }
#gamePopupConfirm:disabled { opacity: 0.45; cursor: default; }
#gamePopupContinue { background: #236ea8; border: 1px solid rgba(99,184,255,0.75); }
</style>
</head>

<body>



<div id="loadingOverlay" aria-hidden="true">
    <div id="loadingInner">
        <div id="loadingTitle">로딩 중...</div>
        <div id="loadingTipCard">
            <div id="loadingTipLabel">💡 TIP</div>
            <div id="loadingTipText"></div>
            <div id="loadingTipCount"></div>
        </div>
        <div id="loadingHint">화면을 터치하면 다음 팁이 나와요</div>
        <div id="loadingBar"><div id="loadingBarFill"></div></div>
        <div id="loadingStatus"></div>
    </div>
</div>

<div id="gamePopupOverlay" aria-hidden="true">
    <div id="gamePopupDialog" role="dialog" aria-modal="true" aria-labelledby="gamePopupTitle">
        <h2 id="gamePopupTitle"></h2>
        <p id="gamePopupMessage"></p>
        <p id="gamePopupNote"></p>
        <div class="game-popup-actions">
            <button id="gamePopupConfirm" type="button"></button>
            <button id="gamePopupContinue" type="button">계속하기</button>
        </div>
    </div>
</div>

<div id="logoutConfirmOverlay" aria-hidden="true">
    <div id="logoutConfirmDialog" role="dialog" aria-modal="true" aria-labelledby="logoutConfirmDialogTitle">
        <h2 id="logoutConfirmDialogTitle">로그아웃</h2>
        <p id="logoutConfirmDialogMessage">로그아웃하시겠습니까?</p>
        <div class="logout-confirm-actions">
            <button id="logoutCancelButton" type="button">취소</button>
            <button id="logoutConfirmButton" type="button">로그아웃</button>
        </div>
    </div>
</div>

<div id="guestNameOverlay" aria-hidden="true">
    <div id="guestNameDialog" role="dialog" aria-modal="true" aria-labelledby="guestNameTitle">
        <h2 id="guestNameTitle">🎮 이름 입력</h2>
        <p>랭킹에 표시될 이름을 적어주세요.<br>이전 이름이 보이면 지우고 새로 적으면 돼요.</p>
        <input id="guestNameInput" type="text" maxlength="16" placeholder="이름 (2~16자)" autocomplete="off">
        <div id="guestNameError"></div>
        <div class="logout-confirm-actions">
            <button id="guestNameCancel" type="button">취소</button>
            <button id="guestNameOk" type="button">시작</button>
        </div>
    </div>
</div>

<div id="rewardListOverlay" aria-hidden="true">
    <div id="rewardListDialog" role="dialog" aria-modal="true" aria-labelledby="rewardListTitle">
        <h2 id="rewardListTitle">👤 프로필</h2>
        <div class="profile-tabs">
            <button id="profileTabStats" class="profile-tab active" type="button">📊 내 정보</button>
            <button id="profileTabRewards" class="profile-tab" type="button">🎁 레벨 보상표</button>
        </div>
        <p id="rewardListSubtitle"></p>
        <div id="rewardListBody"></div>
        <button id="rewardListCloseButton" type="button">닫기</button>
    </div>
</div>

<div id="levelRewardOverlay" aria-hidden="true">
    <div id="levelRewardDialog" role="dialog" aria-modal="true" aria-labelledby="levelRewardTitle">
        <h2 id="levelRewardTitle">🎁 레벨 보상</h2>
        <p id="levelRewardSubtitle"></p>
        <div id="levelRewardList"></div>
        <button id="levelRewardOkButton" type="button">확인</button>
    </div>
</div>

<div id="entryGate" class="entry-screen">
    <div id="loginView" class="entry-card">
        <div class="entry-title">슬라이딩</div>
        <div class="entry-subtitle">로그인해서 게임을 시작하세요</div>

        <form id="loginForm" class="entry-form" autocomplete="on">
            <input id="loginId" name="username" type="text" maxlength="30" placeholder="아이디" autocomplete="username" required>
            <input id="loginPassword" name="password" type="password" maxlength="100" placeholder="비밀번호" autocomplete="current-password" required>
            <label class="remember-login"><input id="rememberLogin" type="checkbox" checked> 로그인 상태 유지</label>
            <button id="loginButton" class="entry-primary" type="submit">로그인</button>
        </form>

        <div id="loginStatus" class="entry-status" aria-live="polite"></div>

        <div class="entry-divider"><span>또는</span></div>

        <button id="registerOpenButton" class="entry-secondary" type="button">회원가입</button>
        <button id="guestPlayButton" class="entry-guest" type="button">게스트로 플레이</button>
    </div>

    <div id="registerView" class="entry-card" hidden>
        <div class="entry-title">회원가입</div>
        <div class="entry-subtitle">아이디, 비밀번호, 닉네임을 등록하세요</div>

        <form id="registerForm" class="entry-form" autocomplete="off">
            <input id="registerId" name="new-username" type="text" maxlength="30" placeholder="아이디" autocomplete="username" required>
            <input id="registerPassword" name="new-password" type="password" maxlength="100" placeholder="비밀번호" autocomplete="new-password" required>
            <input id="registerPasswordConfirm" name="new-password-confirm" type="password" maxlength="100" placeholder="비밀번호 확인" autocomplete="new-password" required>
            <input id="registerNickname" name="nickname" type="text" maxlength="20" placeholder="닉네임" autocomplete="off" required>
            <button id="registerButton" class="entry-primary" type="submit">회원가입 완료</button>
        </form>

        <div id="registerStatus" class="entry-status" aria-live="polite"></div>
        <button id="registerBackButton" class="entry-secondary" type="button">로그인으로 돌아가기</button>
    </div>
</div>

<div id="gameWrapper" hidden>

    <div class="topbar">
        <div id="time">시간 20.0초</div>
        <div id="lives">목숨 ♥ ♥ ♥</div>
        <div id="clears">클리어 0회</div>
        <div id="score">점수 0</div>
        <div id="equippedItemBox">
            <div id="itemInfo">아이템 미사용</div>
            <div id="itemWarning"></div>
        </div>
        <div id="mapSkips">맵 넘기기 ● ● ● ● ●</div>
    </div>

    <div id="canvasStage">
        <canvas id="game" width="800" height="600"></canvas>
        <div id="questRewardOverlay" aria-hidden="true"></div>

        <div id="startMenuOverlay" aria-hidden="true">
            <div class="start-menu-actions">
                <div class="start-menu-account" id="startMenuAccount">
                    <div class="start-account-main"><span class="start-account-level">Lv. 1</span><span class="start-account-name">게스트 모드</span></div>
                    <div class="start-account-exp"><div class="start-account-exp-fill"></div></div>
                    <div class="start-account-exp-text">랭킹 기록 가능 · 레벨 저장 제외</div>
                </div>
            </div>
            <div class="start-menu-competitive"><button id="startMultiplayerButton" class="start-menu-button" type="button">⚔ 2인 대전</button></div>
            <div class="start-menu-tutorial"><button id="startTutorialButton" class="start-menu-button" type="button">📖 튜토리얼</button></div>
            <div class="start-menu-ranking">
                <button id="startRankingButton" class="start-menu-button" type="button">🏆 랭킹</button>
            </div>
        </div>
    </div>

</div>

<div id="rankingPanel" class="ranking-modal" hidden aria-hidden="true">
    <div class="ranking-card">
        <div class="ranking-header">
            <div>🏆 랭킹</div>
            <button id="rankingClose" class="modal-close" type="button" aria-label="닫기">×</button>
        </div>
        <div id="rankingAccountLabel" class="ranking-account-label"></div>
        <div class="ranking-tabs">
            <button id="rankingTodayTab" class="ranking-tab active" type="button">오늘</button>
            <button id="rankingWeeklyTab" class="ranking-tab" type="button">이번 주</button>
        </div>
        <div id="rankingStatus" class="ranking-status" aria-live="polite"></div>
        <div class="ranking-table-wrap">
            <table class="ranking-table">
                <thead>
                    <tr>
                        <th>순위</th>
                        <th>Lv.</th>
                        <th>닉네임</th>
                        <th>점수</th>
                        <th>클리어</th>
                        <th>연속</th>
                    </tr>
                </thead>
                <tbody id="rankingBody"></tbody>
            </table>
        </div>
    </div>
</div>

<script>
"use strict";

/* =========================================================
   기본 설정
========================================================= */

const canvas = document.getElementById("game");
const gameWrapper = document.getElementById("gameWrapper");
const canvasStage = document.getElementById("canvasStage");
const questRewardOverlay = document.getElementById("questRewardOverlay");
const ctx = canvas.getContext("2d");

// 실제 캔버스 픽셀 해상도 배율. 게임 내부 좌표계(800x600)는 유지합니다.
let renderScale = 1;
let lastResolutionCheck = -Infinity;

// 이모지 아이콘만 전용 폰트로 그려 기기별 컬러 이모지가 선명하게 보이도록 합니다.
const EMOJI_FONT = '"Apple Color Emoji","Segoe UI Emoji","Noto Color Emoji",sans-serif';
function drawClearEmoji(emoji, x, y, size = 24) {
    ctx.save();
    ctx.font = `normal ${size}px ${EMOJI_FONT}`;
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    ctx.fillText(emoji, x, y);
    ctx.restore();
}

const CELL = 40;
const COLS = 20;
const ROWS = 15;

const WIDTH = 800;
const HEIGHT = 600;

const TIME_LIMIT = 20;

/* 클리어 횟수에 따른 제한 시간
   0~4회: 20초 / 5~9회: 17초 / 10~19회: 15초
   20~24회: 12초 / 25~29회: 10초 / 30회 이상: 7초
*/
function getStageTimeLimit() {
    const progress = multiplayerMatchActive ? Math.max(0, multiplayerRound - 1) : clearCount;
    if (progress >= 30) return 7;
    if (progress >= 25) return 10;
    if (progress >= 20) return 12;
    if (progress >= 10) return 15;
    if (progress >= 5) return 17;
    return 20;
}

const MAX_LIVES = 3;
const MAX_MAP_SKIPS = 5;

const START = {
    c: 1,
    r: 1
};

let stageStart = {
    c: START.c,
    r: START.r
};

const MAX_MAP_ATTEMPTS = 1200;
const MIN_REACHABLE_STATES = 28;
const MIN_PATH_LENGTH = 5;
const MIN_BRANCHING_STATES = 5;
const MAX_PREVIOUS_LAYOUTS = 180;


/* =========================================================
   게임 상태
========================================================= */

let gameState = "start";

/* =========================================================
   로딩 화면(팁) / 시작 카운트다운 / 종료·포기 확인 팝업
========================================================= */
const LOADING_MIN_MS = 7000;            // 로딩 화면 최소 표시 시간 (팁을 읽을 수 있도록 7초)
const COUNTDOWN_MS = 3000;              // 게임 시작 전 카운트다운
const SOLO_END_CONFIRM_DELAY_MS = 2000; // 싱글 '끝내기' 버튼 조작 딜레이

const LOADING_TIPS = [
    "블록은 벽에 부딪힐 때까지 쭉 미끄러져요. 어디서 멈출지 미리 계산해 보세요!",
    "빨간 위험 블록에 닿으면 목숨이 1개 줄어요. 목숨은 모두 3개예요.",
    "맵 넘기기는 화면 더블 터치(PC는 G 키)! 한 게임에 5번까지 쓸 수 있고, 쓸 때마다 10점씩 감점돼요.",
    "점수는 클리어 1회당 50점, 최고 연속 클리어 1회당 100점이에요. 연속 클리어가 핵심!",
    "클리어를 많이 할수록 제한 시간이 줄어들어요. 5 · 10 · 20 · 25 · 30회에서 단계가 올라가요.",
    "클리어할 때마다 코인 1개! 🛒 상점에서 아이템을 살 수 있어요.",
    "🎒 인벤토리에서 아이템을 장착하면 게임을 시작할 때 사용돼요.",
    "🧭 경로 안내 장치는 맵 시작 때 길을 보여주고, 더블 터치로 맵당 한 번 더 볼 수 있어요.",
    "🔰 에너지 보호막은 위험 블록 충돌을 1회 막아주고, 2스테이지마다 다시 충전돼요.",
    "🔋 에너지 복구 장치는 맵 넘기기를 모두 썼을 때 꺼내 쓸 수 있어요.",
    "📜 일일 퀘스트를 완료하면 코인 보상을 받아요. 마음에 안 들면 다시 뽑을 수도 있어요!",
    "게임이 끝나면 EXP를 얻어요. 레벨업하면 코인과 아이템 보상이 지급돼요! (최고 Lv.100)",
    "⚔ 2인 대전은 같은 맵에서 겨루는 모드예요. 먼저 골인한 사람이 그 라운드의 승자!",
    "2인 대전은 5000점에 먼저 도달하거나, 둘 다 목숨을 잃었을 때 점수가 더 높은 쪽이 이겨요.",
    "🏆 랭킹은 매일, 매주 새로 시작해요. 하루 최고 점수로 순위를 올려 보세요.",
    "👔 스킨 메뉴에서 벽 · 배경 · 캐릭터 · 잔상 · 도착 지점까지 꾸밀 수 있어요.",
    "📖 튜토리얼은 코인 · 점수 · 랭킹에 영향이 없어요. 부담 없이 연습해 보세요!"
];

let loadingActive = false;
let loadingShownAt = 0;
let loadingTimer = null;
let loadingToken = 0;
let loadingTipIndex = 0;

let countdownActive = false;
let countdownEndAt = 0;

let gamePopupOpen = false;
let gamePopupMode = null;            // "solo" | "multi"
let gamePopupDelayTimer = null;
let gamePopupConfirmReadyAt = 0;
let forfeitFallbackTimer = null;
const GAME_POPUP_STATES = ["playing", "transition", "cleared", "dead", "timeout", "countdown", "multiplayerWaitingRound", "multiplayerWaitingResult"];

function renderLoadingTip(animate) {
    const text = document.getElementById("loadingTipText");
    const count = document.getElementById("loadingTipCount");
    const card = document.getElementById("loadingTipCard");
    if (text) text.textContent = LOADING_TIPS[loadingTipIndex];
    if (count) count.textContent = `${loadingTipIndex + 1} / ${LOADING_TIPS.length}`;
    if (animate && card) {
        card.classList.remove("swap");
        void card.offsetWidth;
        card.classList.add("swap");
    }
}

function showLoadingScreen(minMs = LOADING_MIN_MS, status = "게임을 준비하는 중...") {
    const overlay = document.getElementById("loadingOverlay");
    if (!overlay) return;
    loadingToken++;
    clearTimeout(loadingTimer);
    loadingTimer = null;
    loadingActive = true;
    loadingShownAt = performance.now();
    loadingTipIndex = Math.floor(Math.random() * LOADING_TIPS.length);
    renderLoadingTip(false);

    const statusEl = document.getElementById("loadingStatus");
    if (statusEl) statusEl.textContent = status;
    const fill = document.getElementById("loadingBarFill");
    if (fill) {
        fill.style.animation = "none";
        void fill.offsetWidth;
        fill.style.animation = `loadingFill ${Math.max(300, minMs)}ms linear forwards`;
    }
    overlay.classList.add("visible");
    overlay.setAttribute("aria-hidden", "false");
}

function hideLoadingScreen() {
    if (!loadingActive) return;
    loadingActive = false;
    clearTimeout(loadingTimer);
    loadingTimer = null;
    const overlay = document.getElementById("loadingOverlay");
    if (overlay) {
        overlay.classList.remove("visible");
        overlay.setAttribute("aria-hidden", "true");
    }
}

// 로딩 화면을 최소 minMs 동안 보여준 뒤 callback 실행
function runLoadingThen(callback, minMs = LOADING_MIN_MS, status) {
    showLoadingScreen(minMs, status);
    const token = loadingToken;
    loadingTimer = setTimeout(() => {
        loadingTimer = null;
        if (!loadingActive || token !== loadingToken) return;
        hideLoadingScreen();
        callback();
    }, minMs);
}

document.getElementById("loadingOverlay")?.addEventListener("click", event => {
    event.preventDefault();
    if (!loadingActive) return;
    loadingTipIndex = (loadingTipIndex + 1) % LOADING_TIPS.length;
    renderLoadingTip(true);
    playUIClickSound();
});

/* ---------- 시작 전 3초 카운트다운 ---------- */
function beginIntroCountdown() {
    countdownActive = true;
    countdownEndAt = performance.now() + COUNTDOWN_MS;
    movement = null;
    gameState = "countdown";
}

function finishIntroCountdown() {
    countdownActive = false;
    if (gameState === "countdown") gameState = "playing";
    if (activeItem === "pathGuide" && pathGuideUses >= 1) showPathGuide();
    if (multiplayerMatchActive) sendMultiplayerPosition(true);
    updateUI();
}

function drawIntroCountdown(now) {
    const remain = Math.max(0, countdownEndAt - now);
    const num = Math.min(3, Math.max(1, Math.ceil(remain / 1000)));
    const within = (remain % 1000) / 1000;          // 1 → 0 (각 숫자가 보이는 동안)
    const scale = 1 + 0.4 * within;
    const alpha = Math.min(1, within * 2.5 + 0.15);

    ctx.save();
    ctx.fillStyle = "rgba(0,0,0,0.38)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);

    ctx.translate(WIDTH / 2, HEIGHT / 2);
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";

    ctx.save();
    ctx.scale(scale, scale);
    ctx.globalAlpha = alpha;
    ctx.strokeStyle = "rgba(125,220,255,0.85)";
    ctx.lineWidth = 6;
    ctx.shadowBlur = 24;
    ctx.shadowColor = "#55cfff";
    ctx.beginPath();
    ctx.arc(0, 0, 92, 0, Math.PI * 2);
    ctx.stroke();
    ctx.shadowBlur = 0;
    ctx.fillStyle = "#ffffff";
    ctx.font = "bold 120px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(String(num), 0, 6);
    ctx.restore();

    ctx.fillStyle = "#dfe5ea";
    ctx.font = "600 18px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("곧 게임이 시작됩니다", 0, 140);
    ctx.restore();
}

/* ---------- 종료(싱글) / 포기(멀티) 확인 팝업 ---------- */
function openGamePopup(mode) {
    if (gamePopupOpen || loadingActive) return;
    const overlay = document.getElementById("gamePopupOverlay");
    const title = document.getElementById("gamePopupTitle");
    const message = document.getElementById("gamePopupMessage");
    const note = document.getElementById("gamePopupNote");
    const confirmBtn = document.getElementById("gamePopupConfirm");
    if (!overlay || !confirmBtn) return;

    gamePopupOpen = true;
    gamePopupMode = mode;
    clearInterval(gamePopupDelayTimer);
    gamePopupDelayTimer = null;

    if (mode === "multi") {
        title.textContent = "게임을 포기하시겠습니까?";
        message.textContent = "";
        note.textContent = "포기하면 패배 처리 됩니다.";
        confirmBtn.disabled = false;
        confirmBtn.textContent = "포기하기";
    } else {
        title.textContent = "게임을 끝내시겠습니까?";
        message.textContent = "지금까지의 기록으로 게임이 종료돼요.";
        note.textContent = "이 창이 떠 있는 동안에도 제한 시간은 계속 흘러요.";
        // 잘못 누르는 것을 막기 위해 '끝내기'에만 딜레이를 둡니다. ('계속하기'는 즉시 가능)
        gamePopupConfirmReadyAt = performance.now() + SOLO_END_CONFIRM_DELAY_MS;
        const tick = () => {
            const left = gamePopupConfirmReadyAt - performance.now();
            if (left > 0) {
                confirmBtn.disabled = true;
                confirmBtn.textContent = `끝내기 (${Math.ceil(left / 1000)})`;
            } else {
                confirmBtn.disabled = false;
                confirmBtn.textContent = "끝내기";
                clearInterval(gamePopupDelayTimer);
                gamePopupDelayTimer = null;
            }
        };
        tick();
        gamePopupDelayTimer = setInterval(tick, 100);
    }

    overlay.classList.add("visible");
    overlay.setAttribute("aria-hidden", "false");
}

function closeGamePopup() {
    gamePopupOpen = false;
    gamePopupMode = null;
    clearInterval(gamePopupDelayTimer);
    gamePopupDelayTimer = null;
    const overlay = document.getElementById("gamePopupOverlay");
    if (overlay) {
        overlay.classList.remove("visible");
        overlay.setAttribute("aria-hidden", "true");
    }
}

function confirmGamePopup() {
    const mode = gamePopupMode;
    if (!gamePopupOpen) return;
    if (mode === "solo" && performance.now() < gamePopupConfirmReadyAt) return;
    closeGamePopup();

    if (mode === "solo") {
        if (!multiplayerMatchActive && ["playing", "transition", "cleared", "dead", "timeout"].includes(gameState)) {
            finishGameOver();
        }
    } else if (mode === "multi") {
        forfeitMultiplayerMatch();
    }
}

document.getElementById("gamePopupConfirm")?.addEventListener("click", event => {
    event.preventDefault();
    if (event.currentTarget.disabled) return;
    playUIClickSound();
    confirmGamePopup();
});
document.getElementById("gamePopupContinue")?.addEventListener("click", event => {
    event.preventDefault();
    playUIClickSound();
    closeGamePopup();
});

/* ---------- 멀티플레이 포기 ---------- */
function applyLocalForfeit() {
    if (!multiplayerMatchActive) return;
    const winner = multiplayerRole === "host" ? "guest" : "host";
    handleMultiplayerMessage({ type: "matchOver", winner, scores: multiplayerScores, reason: "forfeit" });
    // 서버가 forfeit 메시지를 처리하지 못한 경우에도 연결 종료가 상대의 이탈 승리로 처리됩니다.
    closeMultiplayerSocket();
}

function forfeitMultiplayerMatch() {
    if (!multiplayerMatchActive) return;
    movement = null;
    setMessage("포기 처리 중...");
    if (!multiplayerSend({ type: "forfeit" })) {
        applyLocalForfeit();
        return;
    }
    clearTimeout(forfeitFallbackTimer);
    forfeitFallbackTimer = setTimeout(() => {
        forfeitFallbackTimer = null;
        applyLocalForfeit();
    }, 2000);
}


/* =========================================================
   V28 계정 / 게스트 / 랭킹 상태
========================================================= */
let currentAccount = null;
let guestMode = false;
let gameAccessGranted = false;
let rankingMode = "today";
let rankingLoading = false;

/* 게스트 계정: 서버가 브라우저마다 만들어 주는 guest_ 계정 (랭킹 기록용) */
let guestAccount = null;
let guestSessionPromise = null;

/* =========================================================
   V30 레벨 / EXP 시스템
========================================================= */
const DEFAULT_LEVEL = 1;
const DEFAULT_EXP = 0;
const MAX_LEVEL = 100;
let playerLevel = DEFAULT_LEVEL;
let playerExp = DEFAULT_EXP;
let pendingExpAward = 0;
let pendingExpReason = "";
let expResultData = null;
let expResultSubmitting = false;
let expAnimation = null;

function getLevelRequiredExp(level) {
    const lv = Math.max(1, Math.floor(Number(level) || 1));
    return 100 + (lv - 1) * 50;
}
function normalizeProgress(level, exp) {
    let lv = Math.max(1, Math.floor(Number(level) || 1));
    let xp = Math.max(0, Math.floor(Number(exp) || 0));
    while (lv < MAX_LEVEL && xp >= getLevelRequiredExp(lv)) { xp -= getLevelRequiredExp(lv); lv++; }
    if (lv >= MAX_LEVEL) { lv = MAX_LEVEL; xp = 0; }
    return { level: lv, exp: xp };
}
function setPlayerProgress(level, exp) {
    const p = normalizeProgress(level, exp); playerLevel=p.level; playerExp=p.exp;
    if (currentAccount) { currentAccount.level=playerLevel; currentAccount.exp=playerExp; }
    updateStartMenuOverlay();
}
function calculateSoloExperience() { return Math.max(0, Math.floor(clearCount)*10 + Math.max(0,Math.floor(maxClearStreak))*25); }
function calculateMultiplayerExperience() {
    if (!multiplayerResult || multiplayerResult === "draw") return 0;
    const clears=Math.max(0,Math.floor(clearCount)), streak=Math.max(0,Math.floor(maxClearStreak));
    if (multiplayerResult === multiplayerRole) return clears*20 + streak*30 + Math.max(0,Math.floor(lives))*5;
    return clears*10 + streak*25;
}
function buildLocalProgressAfterAward(amount) {
    let lv=playerLevel, xp=playerExp, remaining=Math.max(0,Math.floor(amount));
    while (remaining>0 && lv<MAX_LEVEL) { const need=getLevelRequiredExp(lv); const add=Math.min(remaining,need-xp); xp+=add; remaining-=add; if(xp>=need){lv++;xp=0;} }
    return normalizeProgress(lv,xp);
}
function formatExp(value) { return Math.max(0,Math.floor(Number(value)||0)).toLocaleString("ko-KR"); }
async function refreshPlayerProgress() {
    if (!currentAccount || guestMode) { setPlayerProgress(DEFAULT_LEVEL,DEFAULT_EXP); return; }
    try { const data=await apiJSON("/api/progress"); setPlayerProgress(data?.level ?? DEFAULT_LEVEL,data?.exp ?? DEFAULT_EXP); }
    catch(error){ setPlayerProgress(currentAccount.level ?? DEFAULT_LEVEL,currentAccount.exp ?? DEFAULT_EXP); console.warn("레벨/EXP 불러오기 실패",error); }
}
async function submitExperienceAward(amount, reason, stats={}) {
    if(!currentAccount || guestMode || !gameAccessGranted || amount<=0) return {level:playerLevel,exp:playerExp,saved:true};
    try { const data=await apiJSON("/api/progress/award",{method:"POST",body:JSON.stringify({amount,reason,...stats})}); setPlayerProgress(data?.level ?? playerLevel,data?.exp ?? playerExp); return data; }
    catch(error){ console.warn("EXP 저장 실패",error); return {level:playerLevel,exp:playerExp,awarded:amount,saved:false}; }
}


let lifeLossCount = 0;
let mapSkipCount = 0;

const RANKING_API_BASE = "https://sliding-multiplayer-server-1.onrender.com";

function setEntryStatus(elementId, message, type = "") {
    const element = document.getElementById(elementId);
    if (!element) return;
    element.textContent = message || "";
    element.className = `entry-status${type ? ` ${type}` : ""}`;
}

function showLoginView(message = "", type = "") {
    document.getElementById("loginView").hidden = false;
    document.getElementById("registerView").hidden = true;
    setEntryStatus("loginStatus", message, type);
}

function showRegisterView() {
    document.getElementById("loginView").hidden = true;
    document.getElementById("registerView").hidden = false;
    setEntryStatus("registerStatus", "", "");
    const input = document.getElementById("registerId");
    if (input) setTimeout(() => input.focus(), 0);
}

function showEntryGate() {
    gameAccessGranted = false;
    const gate = document.getElementById("entryGate");
    const wrapper = document.getElementById("gameWrapper");
    if (gate) {
        gate.classList.remove("session-checking");
        gate.style.display = "flex";
    }
    if (wrapper) wrapper.hidden = true;
    showLoginView();
}

function enterGameAsAccount(account) {
    currentAccount = account && typeof account === "object" ? account : null;
    guestMode = false;
    guestAccount = null;
    gameAccessGranted = true;
    const gate = document.getElementById("entryGate");
    if (gate) {
        gate.classList.remove("session-checking");
        gate.style.display = "none";
    }
    document.getElementById("gameWrapper").hidden = false;
    gameState = "start";
    questOpen = false;
    shopOpen = false;
    inventoryOpen = false;
    skinOpen = false;
    settingsOpen = false;
    multiplayerOpen = false;
    updateStartMenuOverlay();
    updateUI();
    refreshPlayerProgress();
}

function enterGameAsGuest() {
    currentAccount = null;
    guestMode = true;
    guestAccount = null;
    gameAccessGranted = true;
    const gate = document.getElementById("entryGate");
    if (gate) {
        gate.classList.remove("session-checking");
        gate.style.display = "none";
    }
    document.getElementById("gameWrapper").hidden = false;
    gameState = "start";
    questOpen = false;
    shopOpen = false;
    inventoryOpen = false;
    skinOpen = false;
    settingsOpen = false;
    multiplayerOpen = false;
    updateStartMenuOverlay();
    updateUI();
}

function updateStartMenuOverlay() {
    const overlay = document.getElementById("startMenuOverlay");
    const accountLabel = document.getElementById("startMenuAccount");
    if (!overlay || !accountLabel) return;

    const visible = gameAccessGranted && gameState === "start" && !questOpen && !shopOpen && !inventoryOpen && !skinOpen && !settingsOpen && !multiplayerOpen;
    overlay.classList.toggle("visible", visible);
    overlay.setAttribute("aria-hidden", visible ? "false" : "true");

    let accountHTML;
    if (currentAccount) {
        const need=getLevelRequiredExp(playerLevel);
        const ratio=playerLevel>=MAX_LEVEL?1:Math.max(0,Math.min(1,playerExp/need));
        accountHTML=`<div class="start-account-main"><span class="start-account-level">Lv. ${playerLevel}</span><span class="start-account-name">👤 ${escapeHTML(currentAccount.nickname || currentAccount.id || "회원")}</span><span class="start-account-chevron">›</span></div><div class="start-account-exp"><div class="start-account-exp-fill" style="width:${ratio*100}%"></div></div><div class="start-account-exp-text">${playerLevel>=MAX_LEVEL?"MAX LEVEL":`EXP ${formatExp(playerExp)} / ${formatExp(need)}`}</div>`;
    } else {
        accountHTML=`<div class="start-account-main"><span class="start-account-level">Lv. -</span><span class="start-account-name">👤 게스트 모드</span></div><div class="start-account-exp"><div class="start-account-exp-fill" style="width:0%"></div></div><div class="start-account-exp-text">랭킹 기록 가능 · 레벨 저장 제외</div>`;
    }
    if (accountLabel.dataset.html !== accountHTML) {
        accountLabel.dataset.html = accountHTML;
        accountLabel.innerHTML = accountHTML;
    }
}

function escapeHTML(value) {
    return String(value ?? "")
        .replaceAll("&", "&amp;")
        .replaceAll("<", "&lt;")
        .replaceAll(">", "&gt;")
        .replaceAll('"', "&quot;")
        .replaceAll("'", "&#039;");
}

const AUTH_TOKEN_KEY = "slidingMazeAuthToken_v2";
const GUEST_TOKEN_KEY = "slidingMazeGuestToken_v1";

async function apiJSON(path, options = {}) {
    let savedToken = "";
    // 게스트 모드에서는 게스트 전용 토큰을, 로그인 상태에서는 계정 토큰을 보냅니다.
    try {
        savedToken = localStorage.getItem(guestMode && !currentAccount ? GUEST_TOKEN_KEY : AUTH_TOKEN_KEY) || "";
    } catch (error) {}

    const requestHeaders = {
        "Content-Type": "application/json",
        ...(savedToken ? { "Authorization": `Bearer ${savedToken}` } : {}),
        ...(options.headers || {})
    };

    const response = await fetch(`${RANKING_API_BASE}${path}`, {
        ...options,
        // Login state is stored per browser in localStorage and sent as a bearer token.
        // This avoids third-party-cookie restrictions between GitHub Pages and Render.
        credentials: "omit",
        headers: requestHeaders,
        cache: "no-store"
    });

    let data = null;
    try { data = await response.json(); } catch (error) {}

    if (!response.ok) {
        const message = data?.message || data?.error || `요청 실패 (${response.status})`;
        const requestError = new Error(message);
        requestError.status = response.status;
        throw requestError;
    }

    return data;
}

// 게스트 계정을 준비합니다. (저장된 토큰이 유효하면 재사용, 없거나 만료되면 새로 발급)
function ensureGuestSession() {
    if (!guestMode || currentAccount) return Promise.resolve(null);
    if (guestAccount) return Promise.resolve(guestAccount);
    if (guestSessionPromise) return guestSessionPromise;

    guestSessionPromise = (async () => {
        try {
            let token = "";
            try { token = localStorage.getItem(GUEST_TOKEN_KEY) || ""; } catch (error) {}

            if (token) {
                try {
                    const me = await apiJSON("/api/me");
                    if (me && me.id) {
                        guestAccount = { id: me.id, nickname: me.nickname };
                        return guestAccount;
                    }
                } catch (error) {
                    // 만료/삭제된 세션(401)만 버리고, 네트워크 오류는 토큰을 지키기 위해 그대로 실패 처리
                    if (error && error.status === 401) {
                        try { localStorage.removeItem(GUEST_TOKEN_KEY); } catch (e) {}
                    } else {
                        throw error;
                    }
                }
            }

            const data = await apiJSON("/api/guest", { method: "POST", body: "{}" });
            if (!data?.sessionToken || !data?.user) throw new Error("게스트 세션을 만들지 못했습니다.");
            try { localStorage.setItem(GUEST_TOKEN_KEY, data.sessionToken); } catch (error) {}
            guestAccount = { id: data.user.id, nickname: data.user.nickname };
            return guestAccount;
        } catch (error) {
            console.warn("게스트 세션 준비 실패", error);
            return null;
        } finally {
            guestSessionPromise = null;
        }
    })();

    return guestSessionPromise;
}

const LOGIN_REMEMBER_KEY = "slidingMazeRememberLogin_v1";
const LOGIN_ID_KEY = "slidingMazeSavedLoginId_v1";

function loadSavedLoginId() {
    try {
        const saved = localStorage.getItem(LOGIN_ID_KEY);
        const remember = localStorage.getItem(LOGIN_REMEMBER_KEY) !== "0";
        const input = document.getElementById("loginId");
        const checkbox = document.getElementById("rememberLogin");
        if (input && saved) input.value = saved;
        if (checkbox) checkbox.checked = remember;
    } catch (error) {}
}

function saveLoginPreference(id) {
    try {
        const remember = document.getElementById("rememberLogin")?.checked !== false;
        localStorage.setItem(LOGIN_REMEMBER_KEY, remember ? "1" : "0");
        if (remember) localStorage.setItem(LOGIN_ID_KEY, id);
        else localStorage.removeItem(LOGIN_ID_KEY);
    } catch (error) {}
}

async function loginAccount() {
    const id = document.getElementById("loginId").value.trim();
    const password = document.getElementById("loginPassword").value;

    if (!id || !password) {
        setEntryStatus("loginStatus", "아이디와 비밀번호를 입력하세요.", "error");
        return;
    }

    const button = document.getElementById("loginButton");
    button.disabled = true;
    setEntryStatus("loginStatus", "로그인 중...");

    try {
        const data = await apiJSON("/api/login", {
            method: "POST",
            body: JSON.stringify({ id, password })
        });
        const account = data?.account || data?.user || data;
        if (data?.sessionToken) {
            try { localStorage.setItem(AUTH_TOKEN_KEY, data.sessionToken); } catch (error) {}
        } else {
            throw new Error("로그인 세션 토큰을 받지 못했습니다. 서버 코드를 함께 업데이트해 주세요.");
        }
        saveLoginPreference(id);
        document.getElementById("loginPassword").value = "";
        enterGameAsAccount(account);
    } catch (error) {
        setEntryStatus("loginStatus", error.message || "로그인에 실패했습니다.", "error");
    } finally {
        button.disabled = false;
    }
}

async function registerAccount() {
    const id = document.getElementById("registerId").value.trim();
    const password = document.getElementById("registerPassword").value;
    const passwordConfirm = document.getElementById("registerPasswordConfirm").value;
    const nickname = document.getElementById("registerNickname").value.trim();

    if (!id || !password || !passwordConfirm || !nickname) {
        setEntryStatus("registerStatus", "모든 항목을 입력하세요.", "error");
        return;
    }

    if (password !== passwordConfirm) {
        setEntryStatus("registerStatus", "비밀번호가 일치하지 않습니다.", "error");
        return;
    }

    const button = document.getElementById("registerButton");
    button.disabled = true;
    setEntryStatus("registerStatus", "회원가입 중...");

    try {
        await apiJSON("/api/register", {
            method: "POST",
            body: JSON.stringify({ id, password, nickname })
        });

        // 현재 V28 서버는 가입 직후 세션도 만들 수 있으므로,
        // UX 요구사항에 맞춰 명시적으로 로그아웃한 뒤 로그인 화면으로 돌아갑니다.
        try { await apiJSON("/api/logout", { method: "POST", body: "{}" }); } catch (error) {}

        document.getElementById("loginId").value = id;
        document.getElementById("loginPassword").value = "";
        document.getElementById("registerForm").reset();
        showLoginView("회원가입이 완료되었습니다. 로그인해 주세요.", "success");
    } catch (error) {
        setEntryStatus("registerStatus", error.message || "회원가입에 실패했습니다.", "error");
    } finally {
        button.disabled = false;
    }
}

let logoutConfirmOpen = false;

function closeLogoutConfirm() {
    const overlay = document.getElementById("logoutConfirmOverlay");
    if (!overlay) return;
    overlay.classList.remove("visible");
    overlay.setAttribute("aria-hidden", "true");
    logoutConfirmOpen = false;
}

function openLogoutConfirm(options = {}) {
    const overlay = document.getElementById("logoutConfirmOverlay");
    if (!overlay || logoutConfirmOpen) return;

    logoutConfirmOpen = true;
    overlay.classList.add("visible");
    overlay.setAttribute("aria-hidden", "false");

    const cancelButton = document.getElementById("logoutCancelButton");
    const confirmButton = document.getElementById("logoutConfirmButton");
    const dialogTitle = document.getElementById("logoutConfirmDialogTitle");
    const dialogMessage = document.getElementById("logoutConfirmDialogMessage");
    if (dialogTitle) dialogTitle.textContent = options.title || "로그아웃";
    if (dialogMessage) dialogMessage.textContent = options.message || "로그아웃하시겠습니까?";
    if (confirmButton) {
        const neutral = options.danger === false;
        confirmButton.textContent = options.confirmLabel || "로그아웃";
        confirmButton.style.background = neutral ? "#236ea8" : "";
        confirmButton.style.borderColor = neutral ? "rgba(99,184,255,0.75)" : "";
    }
    if (cancelButton) cancelButton.focus();

    return new Promise(resolve => {
        const finish = confirmed => {
            overlay.removeEventListener("click", onOverlayClick);
            cancelButton?.removeEventListener("click", onCancel);
            confirmButton?.removeEventListener("click", onConfirm);
            closeLogoutConfirm();
            resolve(confirmed);
        };
        const onCancel = () => finish(false);
        const onConfirm = () => finish(true);
        const onOverlayClick = event => {
            if (event.target === overlay) finish(false);
        };

        cancelButton?.addEventListener("click", onCancel, { once: true });
        confirmButton?.addEventListener("click", onConfirm, { once: true });
        overlay.addEventListener("click", onOverlayClick);
    });
}

async function logoutToEntry() {
    const confirmed = await openLogoutConfirm();
    if (!confirmed) return;

    try {
        await apiJSON("/api/logout", { method: "POST", body: "{}" });
    } catch (error) {}
    try { localStorage.removeItem(AUTH_TOKEN_KEY); } catch (error) {}

    closeRankingPanel();
    closeMultiplayerSocket();
    currentAccount = null;
    guestMode = false;
    guestAccount = null;
    gameAccessGranted = false;
    try { localStorage.setItem(LOGIN_REMEMBER_KEY, "0"); } catch (error) {}
    document.getElementById("loginId").value = "";
    document.getElementById("loginPassword").value = "";
    document.getElementById("registerForm").reset();
    document.getElementById("gameWrapper").hidden = true;
    document.getElementById("entryGate").style.display = "flex";
    showLoginView("로그아웃되었습니다.", "success");
}

function calculateV28Score() {
    return Math.max(
        0,
        clearCount * 50 +
        maxClearStreak * 100 -
        mapSkipCount * 10 -
        lifeLossCount * 10
    );
}

async function submitV28Score() {
    if (!gameAccessGranted || (!currentAccount && !guestMode)) return false;

    const score = calculateV28Score();

    try {
        // 게스트는 랭킹 저장 전에 게스트 계정이 준비되어 있어야 합니다.
        if (!currentAccount && guestMode) {
            const guest = await ensureGuestSession();
            if (!guest) return false;
        }

        await apiJSON("/api/ranking/score", {
            method: "POST",
            body: JSON.stringify({
                clears: clearCount,
                maxStreak: maxClearStreak,
                skips: mapSkipCount,
                lifeLosses: lifeLossCount,
                score
            })
        });

        // 랭킹 창이 열려 있으면 저장이 끝난 뒤 현재 탭을 다시 불러옵니다.
        const panel = document.getElementById("rankingPanel");
        if (panel && panel.hidden === false && (currentAccount || guestMode)) {
            await loadRanking(rankingMode);
        }
        return true;
    } catch (error) {
        console.warn("랭킹 점수 저장 실패:", error);
        const status = document.getElementById("rankingStatus");
        const panel = document.getElementById("rankingPanel");
        if (panel && panel.hidden === false && status) {
            status.textContent = `랭킹 저장에 실패했습니다: ${error?.message || "서버 응답 오류"}. 잠시 후 다시 시도해 주세요.`;
        }
        return false;
    }
}

/* 프로필 통계: 게임 1회가 끝날 때 한 번만 서버에 기록 */
let playStatsSentFor = null;

function getMultiplayerOutcome() {
    if (multiplayerResult === multiplayerRole) return "win";
    if (multiplayerResult === "draw" || !multiplayerResult) return "draw";
    return "loss";
}

async function submitPlayStats(mode, result = null) {
    if (!currentAccount || guestMode || !gameAccessGranted) return;
    if (!runStartTime || playStatsSentFor === runStartTime) return;   // 같은 판 중복 방지
    playStatsSentFor = runStartTime;

    const seconds = Math.max(0, Math.min(21600, Math.round((Date.now() - runStartTime.getTime()) / 1000)));
    try {
        await apiJSON("/api/profile/record", {
            method: "POST",
            body: JSON.stringify({
                mode, result, seconds,
                clears: clearCount,
                maxStreak: maxClearStreak,
                skips: mapSkipCount,
                lifeLosses: lifeLossCount
            })
        });
    } catch (error) {
        console.warn("플레이 기록 저장 실패", error);
    }
}

let rankingBodyOverflowBackup = null;

function lockPageForRanking() {
    const body = document.body;
    const html = document.documentElement;
    if (!body || !html) return;
    rankingBodyOverflowBackup = {
        bodyOverflow: body.style.overflow,
        htmlOverflow: html.style.overflow
    };
    html.style.overflow = "hidden";
    body.style.overflow = "hidden";
}

function unlockPageForRanking() {
    const body = document.body;
    const html = document.documentElement;
    if (!body || !html) return;
    const backup = rankingBodyOverflowBackup || { bodyOverflow: "", htmlOverflow: "" };
    body.style.overflow = backup.bodyOverflow;
    html.style.overflow = backup.htmlOverflow;
    rankingBodyOverflowBackup = null;
}

// iPad/iOS keyboard가 input을 화면에 맞추기 위해 자동 스크롤할 때
// body를 fixed로 잠그지 않고, 모달이 열려 있을 때만 배경 스크롤을 막습니다.
window.addEventListener("focusin", event => {
    if (!event.target || !["INPUT", "TEXTAREA", "SELECT"].includes(event.target.tagName)) return;
    if (document.getElementById("rankingPanel")?.hidden === false) return;
    // 입력창을 fixed body와 함께 움직이지 않게 하는 별도 스크롤 강제는 하지 않습니다.
}, { passive: true });

function openRankingPanel(mode = "today") {
    if (!currentAccount && !guestMode) return;

    rankingMode = mode === "weekly" ? "weekly" : "today";
    const panel = document.getElementById("rankingPanel");
    lockPageForRanking();
    panel.hidden = false;
    panel.classList.add("ranking-open");
    panel.setAttribute("aria-hidden", "false");
    updateRankingTabs();
    loadRanking(rankingMode);
}

function closeRankingPanel() {
    const panel = document.getElementById("rankingPanel");
    if (!panel) return;
    panel.hidden = true;
    panel.classList.remove("ranking-open");
    panel.setAttribute("aria-hidden", "true");
    unlockPageForRanking();
}

function updateRankingTabs() {
    document.getElementById("rankingTodayTab")?.classList.toggle("active", rankingMode === "today");
    document.getElementById("rankingWeeklyTab")?.classList.toggle("active", rankingMode === "weekly");
}

async function loadRanking(mode = rankingMode) {
    if (!currentAccount && !guestMode) return;
    rankingLoading = true;
    rankingMode = mode === "weekly" ? "weekly" : "today";
    updateRankingTabs();
    const status = document.getElementById("rankingStatus");
    const body = document.getElementById("rankingBody");
    status.textContent = rankingMode === "weekly" ? "이번 주 랭킹을 불러오는 중..." : "오늘 랭킹을 불러오는 중...";
    body.innerHTML = "";

    try {
        const data = await apiJSON(rankingMode === "weekly" ? "/api/ranking/weekly" : "/api/ranking/today");
        const rows = Array.isArray(data?.rows) ? data.rows : Array.isArray(data?.ranking) ? data.ranking : Array.isArray(data) ? data : [];

        if (rows.length === 0) {
            body.innerHTML = `<tr><td colspan="6">아직 랭킹 기록이 없습니다.</td></tr>`;
        } else {
            body.innerHTML = rows.map((row, index) => {
                const rank = Number(row.rank) || index + 1;
                const level = Math.max(1, Number(row.level) || 1);
                const nickname = row.nickname || row.name || "-";
                const score = Number(row.score) || 0;
                const clears = Number(row.clears) || 0;
                const streak = Number(row.maxStreak) || Number(row.max_streak) || 0;
                return `<tr>
                    <td>${rank}</td>
                    <td>Lv. ${level}</td>
                    <td>${escapeHTML(nickname)}</td>
                    <td>${score.toLocaleString("ko-KR")}</td>
                    <td>${clears}</td>
                    <td>${streak}</td>
                </tr>`;
            }).join("");
        }

        status.textContent = (rankingMode === "weekly"
            ? "이번 주 월요일부터 일요일까지의 랭킹입니다."
            : "오늘의 랭킹입니다.") +
            (guestMode && !currentAccount ? " (게스트 기록은 이 기기에서만 이어져요)" : "");
    } catch (error) {
        status.textContent = error.message || "랭킹을 불러오지 못했습니다.";
        body.innerHTML = `<tr><td colspan="6">랭킹 정보를 불러오지 못했습니다.</td></tr>`;
    } finally {
        rankingLoading = false;
    }
}

function bindEntryAndRankingUI() {
    const initialRankingPanel = document.getElementById("rankingPanel");
    if (initialRankingPanel) {
        initialRankingPanel.hidden = true;
        initialRankingPanel.classList.remove("ranking-open");
        initialRankingPanel.setAttribute("aria-hidden", "true");
    }
    loadSavedLoginId();
    document.getElementById("loginForm")?.addEventListener("submit", event => {
        event.preventDefault();
        loginAccount();
    });

    document.getElementById("registerForm")?.addEventListener("submit", event => {
        event.preventDefault();
        registerAccount();
    });

    document.getElementById("registerOpenButton")?.addEventListener("click", () => {
        playUIClickSound();
        showRegisterView();
    });

    document.getElementById("registerBackButton")?.addEventListener("click", () => {
        playUIClickSound();
        showLoginView();
    });

    document.getElementById("guestPlayButton")?.addEventListener("click", () => {
        playUIClickSound();
        enterGameAsGuest();
    });

    document.getElementById("startRankingButton")?.addEventListener("click", event => {
        event.preventDefault();
        event.stopPropagation();
        playUIClickSound();
        openRankingPanel("today");
    });

    document.getElementById("startMultiplayerButton")?.addEventListener("click", event => {
        event.preventDefault();
        event.stopPropagation();
        playUIClickSound();
        withGuestName(openMultiplayerMenu);
    });

    document.getElementById("rankingClose")?.addEventListener("click", event => {
        event.preventDefault();
        event.stopPropagation();
        playUIClickSound();
        closeRankingPanel();
    });

    document.getElementById("rankingTodayTab")?.addEventListener("click", event => {
        event.preventDefault();
        event.stopPropagation();
        playUIClickSound();
        loadRanking("today");
    });

    document.getElementById("rankingWeeklyTab")?.addEventListener("click", event => {
        event.preventDefault();
        event.stopPropagation();
        playUIClickSound();
        loadRanking("weekly");
    });

    const rankingPanel = document.getElementById("rankingPanel");
    rankingPanel?.addEventListener("pointerdown", event => {
        if (event.target === rankingPanel) {
            event.preventDefault();
            event.stopPropagation();
            closeRankingPanel();
            return;
        }
        event.stopPropagation();
    });
    rankingPanel?.addEventListener("touchstart", event => event.stopPropagation(), { passive: true });

    document.querySelectorAll("#startMenuOverlay button").forEach(button => {
        button.addEventListener("pointerdown", event => event.stopPropagation());
        button.addEventListener("pointerup", event => event.stopPropagation());
        button.addEventListener("touchstart", event => event.stopPropagation(), { passive: true });
        button.addEventListener("touchend", event => event.stopPropagation(), { passive: true });
    });
}

/* =========================================================
   게스트 이름 입력 (게임 시작 / 2인 대전 진입 때마다)
========================================================= */
const GUEST_LAST_NAME_KEY = "slidingMazeGuestLastName_v1";
let guestNameOpen = false;

async function applyGuestName(name) {
    if (!(guestAccount && guestAccount.nickname === name)) {
        const data = await apiJSON("/api/guest", {
            method: "POST",
            body: JSON.stringify({ nickname: name })
        });
        if (!data?.sessionToken || !data?.user) throw new Error("게스트 계정을 만들지 못했습니다.");
        try { localStorage.setItem(GUEST_TOKEN_KEY, data.sessionToken); } catch (error) {}
        guestAccount = { id: data.user.id, nickname: data.user.nickname };
        name = data.user.nickname;
    }
    try { localStorage.setItem(GUEST_LAST_NAME_KEY, name); } catch (error) {}
}

// 게스트가 아니면 바로 true. 게스트면 이름 입력창을 띄우고, 확인하면 true / 취소하면 false.
function requireGuestName() {
    if (!guestMode || currentAccount) return Promise.resolve(true);
    if (guestNameOpen) return Promise.resolve(false);

    const overlay = document.getElementById("guestNameOverlay");
    const input = document.getElementById("guestNameInput");
    const errorEl = document.getElementById("guestNameError");
    const okBtn = document.getElementById("guestNameOk");
    const cancelBtn = document.getElementById("guestNameCancel");
    if (!overlay || !input) return Promise.resolve(true);

    guestNameOpen = true;
    let last = "";
    try { last = localStorage.getItem(GUEST_LAST_NAME_KEY) || ""; } catch (error) {}
    input.value = last || guestAccount?.nickname || "";   // 직전에 쓴 이름을 먼저 보여줌
    errorEl.textContent = "";
    okBtn.disabled = false;
    overlay.classList.add("visible");
    overlay.setAttribute("aria-hidden", "false");
    setTimeout(() => { input.focus(); input.select(); }, 50);   // 선택돼 있어서 바로 타이핑하면 교체됨

    return new Promise(resolve => {
        let busy = false;

        const close = result => {
            overlay.classList.remove("visible");
            overlay.setAttribute("aria-hidden", "true");
            okBtn.onclick = cancelBtn.onclick = input.onkeydown = null;
            guestNameOpen = false;
            resolve(result);
        };

        const submit = async () => {
            if (busy) return;
            const name = input.value.trim();
            if (name.length < 2 || name.length > 16 || /[\u0000-\u001F\u007F]/.test(name)) {
                errorEl.textContent = "이름은 2~16자로 입력해주세요.";
                return;
            }
            busy = true;
            okBtn.disabled = true;
            errorEl.textContent = "확인 중...";
            try {
                await applyGuestName(name);
                close(true);
            } catch (error) {
                errorEl.textContent = error?.message || "이름을 설정하지 못했습니다.";
                busy = false;
                okBtn.disabled = false;
            }
        };

        okBtn.onclick = submit;
        cancelBtn.onclick = () => { if (!busy) close(false); };
        input.onkeydown = event => {
            if (event.key === "Enter") { event.preventDefault(); submit(); }
            else if (event.key === "Escape" && !busy) close(false);
        };
    });
}

// 시작 동작을 "이름 확인 → 실행" 순서로 감싸는 헬퍼
function withGuestName(action) {
    requireGuestName().then(ok => {
        if (ok && gameState === "start") action();
    });
}

bindEntryAndRankingUI();
showEntryGate();

/* =========================================================
   2인용 경쟁 모드 준비 상태
   - 현재는 방/코드/시드 UI까지 준비
   - 실제 기기 간 연결은 다음 단계에서 WebRTC + 시그널링 서버 연결
========================================================= */
let multiplayerOpen = false;
let multiplayerRole = null;
let multiplayerRoomCode = "";
let multiplayerSeed = 0;
let multiplayerOpponentName = "상대 플레이어";

/* =========================================================
   2인용 서버 실제 연결
========================================================= */
const MULTIPLAYER_SERVER_URL = "wss://sliding-multiplayer-server-1.onrender.com";
let multiplayerSocket = null;
let multiplayerConnected = false;
let multiplayerPeerJoined = false;
let multiplayerMatchActive = false;
let multiplayerResult = null;
let multiplayerResultSoundPlayed = false;
let multiplayerScores = { host: 0, guest: 0 };   // 서버가 보내주는 실시간 점수
let multiplayerFinalScores = null;               // 경기 종료 시 최종 점수
let multiplayerStatus = "서버 연결 중...";
let multiplayerSendAccumulator = 0;
let multiplayerEliminatedSent = false;
let multiplayerSelfDead = false;   // 내 목숨이 0이 되어 결과 대기 중인지
let multiplayerMatchmaking = false;
let multiplayerRound = 0;
let multiplayerRoundTransition = false;
let multiplayerMatchType = null;
let multiplayerPlayerVisible = true;
let multiplayerPeerLeftDeadline = 0;
let multiplayerPeerLeftTimer = null;
let opponentEliminatedRound = 0;
let opponent = {
    x: 0, y: 0,
    targetX: 0, targetY: 0,
    c: 1, r: 1,
    visible: false
};

// 빠른 대전 연결 진단: 게임 로직은 바꾸지 않고 브라우저 콘솔에 상태만 기록합니다.
function logMultiplayerDebug(eventName, details = {}) {
    try {
        console.info("[QUICK CLIENT DEBUG]", JSON.stringify({
            time: new Date().toISOString(),
            event: eventName,
            state: gameState,
            role: multiplayerRole,
            matchType: multiplayerMatchType,
            active: multiplayerMatchActive,
            connected: multiplayerConnected,
            peerJoined: multiplayerPeerJoined,
            socketState: multiplayerSocket ? multiplayerSocket.readyState : null,
            round: multiplayerRound,
            visibility: document.visibilityState,
            ...details
        }));
    } catch (error) {
        console.info("[QUICK CLIENT DEBUG]", eventName, details);
    }
}

window.addEventListener("error", event => {
    logMultiplayerDebug("windowError", {
        message: event.message || "",
        source: event.filename || "",
        line: event.lineno || 0,
        column: event.colno || 0
    });
});
window.addEventListener("unhandledrejection", event => {
    logMultiplayerDebug("unhandledRejection", { reason: String(event.reason || "unknown") });
});
window.addEventListener("pagehide", event => {
    logMultiplayerDebug("pageHide", { persisted: !!event.persisted });
});
document.addEventListener("visibilitychange", () => {
    logMultiplayerDebug("visibilityChange", { visibility: document.visibilityState });
});

function multiplayerSend(data) {
    if (!multiplayerSocket || multiplayerSocket.readyState !== WebSocket.OPEN) {
        logMultiplayerDebug("sendSkipped", { messageType: data && data.type, reason: "socket-not-open" });
        return false;
    }
    try {
        multiplayerSocket.send(JSON.stringify(data));
        if (data && ["matchmake", "matchReady", "matchStart", "position"].includes(data.type) && data.type !== "position") {
            logMultiplayerDebug("sentMessage", { messageType: data.type, round: data.round });
        }
        return true;
    } catch (error) {
        logMultiplayerDebug("sendError", { messageType: data && data.type, error: String(error) });
        return false;
    }
}

function closeMultiplayerSocket() {
    if (multiplayerPeerLeftTimer) {
        clearInterval(multiplayerPeerLeftTimer);
        multiplayerPeerLeftTimer = null;
    }
    multiplayerPeerLeftDeadline = 0;
    multiplayerConnected = false;
    multiplayerPeerJoined = false;
    multiplayerMatchActive = false;
    multiplayerEliminatedSent = false;
    multiplayerSelfDead = false;
    multiplayerMatchmaking = false;
    multiplayerRound = 0;
    multiplayerRoundTransition = false;
    multiplayerMatchType = null;
    hideLoadingScreen();
    if (multiplayerSocket) { try { multiplayerSocket.close(); } catch (error) {} }
    multiplayerSocket = null;
}

function resetOpponent() {
    opponent.x = player.x;
    opponent.y = player.y;
    opponent.targetX = player.x;
    opponent.targetY = player.y;
    opponent.c = player.c;
    opponent.r = player.r;
    opponent.visible = false;
}

function sendMultiplayerPosition(force = false) {
    if (!multiplayerMatchActive || multiplayerSelfDead) return;
    if (!force && multiplayerSendAccumulator < 0.08) return;
    multiplayerSendAccumulator = 0;
    multiplayerSend({
        type: "position",
        round: multiplayerRound,
        c: player.c,
        r: player.r,
        x: player.x,
        y: player.y,
        moving: !!movement
    });
}

function startMultiplayerMatchmaking() {
    closeMultiplayerSocket();
    multiplayerRole = null;
    multiplayerRoomCode = "";
    multiplayerSeed = 0;
    multiplayerMatchmaking = false;
    multiplayerPeerJoined = false;
    multiplayerMatchActive = false;
    multiplayerStatus = "상대를 찾는 중...";
    updateUI();

    connectMultiplayerSocket(() => {
        multiplayerMatchmaking = true;
        multiplayerMatchType = "quick";
        multiplayerStatus = "상대를 찾는 중...";
        multiplayerSend({ type: "matchmake" });
        updateUI();
    });
}

function cancelMultiplayerMatchmaking() {
    multiplayerMatchmaking = false;
    multiplayerStatus = "매칭을 취소했습니다.";
    closeMultiplayerSocket();
    multiplayerOpen = true;
    multiplayerRole = null;
    updateUI();
}

function connectMultiplayerSocket(onConnected) {
    closeMultiplayerSocket();
    multiplayerStatus = "서버 연결 중...";
    let socket;
    try { socket = new WebSocket(MULTIPLAYER_SERVER_URL); }
    catch (error) { multiplayerStatus = "서버 연결에 실패했습니다."; updateUI(); return; }
    multiplayerSocket = socket;

    socket.addEventListener("open", () => {
        logMultiplayerDebug("socketOpen", { socketState: socket.readyState });
        if (multiplayerSocket !== socket) return;
        multiplayerConnected = true;
        multiplayerStatus = "서버 연결 완료";
        onConnected();
        updateUI();
    });
    socket.addEventListener("message", event => {
        let data;
        try { data = JSON.parse(event.data); } catch (error) {
            logMultiplayerDebug("invalidSocketMessage", { error: String(error) });
            return;
        }
        if (data && data.type !== "position") {
            logMultiplayerDebug("receivedMessage", { messageType: data.type, round: data.round, roleFromServer: data.role });
        }
        handleMultiplayerMessage(data);
    });
    socket.addEventListener("error", event => {
        logMultiplayerDebug("socketError", { eventType: event && event.type, socketState: socket.readyState });
        if (multiplayerSocket !== socket) return;
        multiplayerStatus = "서버 연결 오류";
        updateUI();
    });
    socket.addEventListener("close", event => {
        logMultiplayerDebug("socketClose", {
            closeCode: event.code,
            closeReason: event.reason || "",
            wasClean: event.wasClean,
            socketState: socket.readyState,
            activeAtClose: multiplayerMatchActive,
            matchmakingAtClose: multiplayerMatchmaking
        });
        if (multiplayerSocket !== socket) return;
        multiplayerConnected = false;
        multiplayerPeerJoined = false;
        if (multiplayerMatchActive ||
            gameState === "multiplayerWaitingResult" ||
            gameState === "multiplayerWaitingRound") {
            multiplayerMatchActive = false;
            multiplayerResult = "draw";                 // EXP 0, 결과 화면에서 나갈 수 있음
            void submitPlayStats("multiplayer", "draw");
            gameState = "multiplayerResult";
            multiplayerOpen = false;
            movement = null;
            opponent.visible = false;
            pendingExpAward = 0;
            pendingExpReason = "multiplayer_disconnect";
            setMessage("서버 연결이 끊어졌습니다.");
        } else if (multiplayerMatchmaking) {
            multiplayerStatus = "매칭 서버 연결이 종료되었습니다.";
            multiplayerMatchmaking = false;
            multiplayerOpen = true;
            multiplayerRole = null;
        } else {
            multiplayerStatus = "서버 연결 종료";
            if (loadingActive) {
                hideLoadingScreen();
                multiplayerOpen = true;
                multiplayerRole = null;
                gameState = "start";
                setMessage("서버 연결이 종료되었습니다. 다시 시도해 주세요.");
            }
        }
        updateUI();
    });
}

function playMultiplayerResultSound(result) {
    if (multiplayerResultSoundPlayed) return;
    if (result === multiplayerRole) {
        playEffectSound("versusWin", "versus-result");
        multiplayerResultSoundPlayed = true;
    } else if (result && result !== "draw") {
        playEffectSound("versusLose", "versus-result");
        multiplayerResultSoundPlayed = true;
    }
}

function handleMultiplayerMessage(data) {
    if (data.type === "error") {
        multiplayerStatus = data.message || "서버 오류";
        window.alert(multiplayerStatus);
        return;
    }
    if (data.type === "matchFound") {
        logMultiplayerDebug("matchFoundHandling", { serverRole: data.role });
        multiplayerMatchmaking = false;
        multiplayerRole = data.role === "guest" ? "guest" : "host";
        // 빠른 대전은 내부 방 코드를 사용자에게 표시하지 않습니다.
        multiplayerRoomCode = "";
        multiplayerPeerJoined = true;
        multiplayerStatus = "상대 플레이어를 찾았습니다. 경기 준비 중...";
        multiplayerOpen = false;
        if (multiplayerMatchType === "quick") {
            showLoadingScreen(LOADING_MIN_MS, "상대 플레이어와 연결하는 중...");
        }
        updateUI();

        // 빠른 대전에서는 양쪽 클라이언트가 matchFound를 실제로 수신한 뒤
        // 모두 준비 완료를 서버에 알려야 방장이 시작할 수 있습니다.
        // 서로 다른 WebSocket 연결의 메시지 도착 순서가 뒤바뀌는 경쟁 조건을 방지합니다.
        if (multiplayerMatchType === "quick") {
            multiplayerSend({ type: "matchReady" });
            multiplayerStatus = "두 플레이어의 연결을 확인하는 중...";
            updateUI();
        } else if (multiplayerRole === "host") {
            startMultiplayerMatch();
        }
        return;
    }
    if (data.type === "quickMatchTimeout") {
        logMultiplayerDebug("quickMatchTimeoutReceived");
        closeMultiplayerSocket();
        multiplayerMatchmaking = false;
        multiplayerMatchActive = false;
        multiplayerPeerJoined = false;
        multiplayerOpen = true;
        multiplayerRole = null;
        gameState = "start";
        multiplayerStatus = data.message || "빠른 대전 연결 시간이 초과되었습니다. 다시 시도해 주세요.";
        setMessage(multiplayerStatus);
        updateUI();
        return;
    }
    if (data.type === "quickMatchReady") {
        logMultiplayerDebug("quickMatchReadyHandling");
        if (multiplayerMatchType === "quick" && multiplayerRole === "host" && !multiplayerMatchActive) {
            // 로딩 화면(팁)을 최소 시간 동안 보여준 뒤 경기를 시작합니다.
            const token = loadingToken;
            const wait = loadingActive ? Math.max(0, LOADING_MIN_MS - (performance.now() - loadingShownAt)) : 0;
            setTimeout(() => {
                if (token !== loadingToken) return;
                if (multiplayerMatchType === "quick" && multiplayerRole === "host" && !multiplayerMatchActive && multiplayerConnected) {
                    startMultiplayerMatch();
                }
            }, wait);
        }
        return;
    }
    if (data.type === "roomCreated") {
        multiplayerMatchmaking = false;
        multiplayerRoomCode = String(data.room || multiplayerRoomCode);
        multiplayerStatus = "방 생성 완료 · 친구를 기다리는 중";
        multiplayerPeerJoined = false;
        updateUI();
        return;
    }
    if (data.type === "roomJoined") {
        multiplayerMatchmaking = false;
        multiplayerRoomCode = String(data.room || multiplayerRoomCode);
        multiplayerStatus = "방 참가 완료 · 방장의 시작을 기다리는 중";
        updateUI();
        return;
    }
    if (data.type === "peerJoined") {
        multiplayerPeerJoined = true;
        multiplayerPeerLeftDeadline = 0;
        if (multiplayerPeerLeftTimer) {
            clearInterval(multiplayerPeerLeftTimer);
            multiplayerPeerLeftTimer = null;
        }
        if (multiplayerMatchActive || gameState === "multiplayerWaitingResult") {
            multiplayerStatus = "상대 플레이어가 재접속했습니다. 경기를 계속합니다.";
            setMessage("상대 플레이어가 재접속했습니다. 경기를 계속합니다.");
        } else {
            multiplayerStatus = "상대 플레이어가 참가했습니다. 경기 시작을 눌러주세요.";
        }
        updateUI();
        return;
    }
    if (data.type === "peerLeft") {
        multiplayerPeerJoined = false;
        if (data.roomClosed) {
            closeMultiplayerSocket();
            multiplayerRole = null;
            multiplayerRoomCode = "";
            multiplayerOpen = true;
            multiplayerStatus = "방장이 나가서 방이 닫혔습니다.";
        } else {
            multiplayerStatus = "상대 플레이어가 나갔습니다. 다시 기다리는 중...";
        }
        updateUI();
        return;
    }
    if (data.type === "playerLeftTimeout") {
        if (!multiplayerMatchActive &&
            gameState !== "multiplayerWaitingResult" &&
            gameState !== "multiplayerWaitingRound") return;
        multiplayerPeerLeftDeadline = 0;
        if (multiplayerPeerLeftTimer) {
            clearInterval(multiplayerPeerLeftTimer);
            multiplayerPeerLeftTimer = null;
        }
        multiplayerPeerJoined = false;
        multiplayerMatchActive = false;
        multiplayerResult = data.winner || multiplayerResult || "draw";
        onDailyQuestMultiplayerMatchEnd(multiplayerResult);
        playMultiplayerResultSound(multiplayerResult);
        gameState = "multiplayerResult";
        movement = null;
        multiplayerOpen = false;
        pendingExpAward = calculateMultiplayerExperience();
        pendingExpReason = multiplayerResult === multiplayerRole ? "multiplayer_win" : "multiplayer_loss";
        // 경기 종료 시에도 최종 기록을 한 번 더 저장합니다. (저장 실패/마지막 라운드 보완)
        void submitV28Score();
        void submitPlayStats("multiplayer", getMultiplayerOutcome());
        setMessage(
            multiplayerResult === multiplayerRole ? "승리했습니다!" :
            multiplayerResult === "draw" ? "무승부입니다." : "패배했습니다."
        );
        updateUI();
        return;
    }
    if (data.type === "scoreUpdate") {
        if (data.scores) multiplayerScores = data.scores;
        return;
    }
    if (data.type === "opponentEliminated") {
        if (Number(data.round) !== multiplayerRound) return;
        opponentEliminatedRound = multiplayerRound;
        opponent.visible = false;
        return;
    }
    if (data.type === "position") {
        if (!multiplayerMatchActive) return;
        if (data.round !== undefined && Number(data.round) !== multiplayerRound) return;
        if (opponentEliminatedRound === multiplayerRound) return;
        const x = Number(data.x), y = Number(data.y);
        if (!Number.isFinite(x) || !Number.isFinite(y)) return;
        opponent.targetX = x;
        opponent.targetY = y;
        opponent.c = Number.isFinite(Number(data.c)) ? Number(data.c) : 0;
        opponent.r = Number.isFinite(Number(data.r)) ? Number(data.r) : 0;
        // 처음 수신할 때는 이전 라운드 위치에서 이동시키지 않고 즉시 표시합니다.
        if (!opponent.visible) {
            opponent.x = x;
            opponent.y = y;
        }
        opponent.visible = true;
        return;
    }
    if (data.type === "matchStart") {
        logMultiplayerDebug("matchStartReceived", { incomingRound: data.round, incomingSeed: data.seed, isGuest: multiplayerRole === "guest" });
        if (multiplayerRole !== "guest") return;
        // 죽은 참가자는 다음 라운드가 시작돼도 다시 플레이 상태로 돌아가지 않습니다.
        if (multiplayerSelfDead && Number(data.round) > 1) {
            multiplayerRound = Number(data.round) || (multiplayerRound + 1);
            multiplayerRoundTransition = false;
            opponentEliminatedRound = 0;
            opponent.visible = false;
            multiplayerSeed = Number(data.seed) || 0;
            stageStart = data.startPosition && Number.isFinite(Number(data.startPosition.c)) && Number.isFinite(Number(data.startPosition.r))
                ? { c: Number(data.startPosition.c), r: Number(data.startPosition.r) }
                : { c: START.c, r: START.r };
            buildSpectatorMap();
            return;
        }
        multiplayerMatchActive = true;
        multiplayerResult = null;
        multiplayerResultSoundPlayed = false;
        resetOneShotEffects();
        multiplayerEliminatedSent = false;
        multiplayerRoundTransition = false;
        opponentEliminatedRound = 0;
        multiplayerPlayerVisible = true;
        multiplayerSeed = Number(data.seed) || 0;
        multiplayerRound = Number(data.round) || (multiplayerRound + 1);
        multiplayerOpen = false;
        clearTimeout(roundTimer);
        settingsOpen = false;

        const firstRound = multiplayerRound === 1;
        if (firstRound) {
            multiplayerSelfDead = false;
            onDailyQuestMultiplayerMatchStart(multiplayerMatchType || "quick");
            onDailyQuestGameStart();
            lives = MAX_LIVES;
            clearCount = 0;
            clearStreak = 0;
            maxClearStreak = 0;
            lifeLossCount = 0;
            mapSkipCount = 0;
            multiplayerScores = { host: 0, guest: 0 };
            multiplayerFinalScores = null;
            mapSkips = MAX_MAP_SKIPS;
            stageStart = { c: START.c, r: START.r };
            recordSavedForRun = false;
            runStartTime = new Date();
            activateItemForRun();
            resetRecoil();
            flash.alpha = 0;
        }

        gameState = "playing";
        gameplayUIAccumulator = 0;
        onDailyQuestMultiplayerRoundStart();
        remainingTime = getStageTimeLimit() + activeTimeBonus;
        stageStart = data.startPosition && Number.isFinite(Number(data.startPosition.c)) && Number.isFinite(Number(data.startPosition.r))
            ? { c: Number(data.startPosition.c), r: Number(data.startPosition.r) }
            : { c: START.c, r: START.r };
        // 방장에게서 맵 배열을 받지 않습니다. 양쪽이 같은 시드와 시작 위치로
        // 동일한 맵을 각자 생성해 네트워크 전송량과 시작 시 지연을 줄입니다.
        mapTransition.active = false;
        pathGuideUses = 0;
        pathGuidePath = [];
        activeItem = null;
        activeTimeBonus = 0;
        shieldCharges = 0;
        firstAidCharged = false;
        logMultiplayerDebug("guestGameStatePlaying", {
            incomingRound: data.round,
            seed: multiplayerSeed,
            startPosition: stageStart
        });
        resetPlayer();
        mapTransition.active = false;
        pathGuideUses = 0;
        pathGuidePath = [];
        createMapWithSeed(multiplayerSeed);
        if (activeItem === "pathGuide") { showPathGuide(); pathGuideUses = 1; }
        resetOpponent();
        multiplayerPlayerVisible = true;
        multiplayerOpen = false;
        if (firstRound) {
            hideLoadingScreen();
            beginIntroCountdown();
        } else {
            gameState = "playing";
        }
        // 방장이 보낸 맵을 적용하고 플레이어 위치를 초기화한 다음에 첫 위치를 보냅니다.
        sendMultiplayerPosition(true);
        setMessage(multiplayerRound === 1 ? "" : `다음 맵 · ${multiplayerRound}라운드`);
        updateUI();
        return;
    }
    if (data.type === "roundWon") {
        if (data.scores) multiplayerScores = data.scores;
        if (!multiplayerMatchActive) return;
        if (Number(data.round) !== multiplayerRound) return;
        if (multiplayerRoundTransition) return;

        // 죽은 상태: 점수/연속 기록은 건드리지 않고, 방장이면 다음 라운드 진행만 담당
        if (multiplayerSelfDead) {
            if (multiplayerRole === "host") {
                startNextMultiplayerRound(
                    data.nextStart && Number.isFinite(Number(data.nextStart.c)) && Number.isFinite(Number(data.nextStart.r))
                        ? { c: Number(data.nextStart.c), r: Number(data.nextStart.r) }
                        : { c: player.c, r: player.r }
                );
            }
            return;
        }

        multiplayerRoundTransition = true;
        const winner = data.winner || "draw";

        if (winner === multiplayerRole) {
            onDailyQuestMultiplayerRoundWin();
            clearCount++;
            clearStreak++;
            maxClearStreak = Math.max(maxClearStreak, clearStreak);
            allTimeBestStreak = Math.max(allTimeBestStreak, clearStreak);
            coins++;
            saveCoins();
            if (clearCount > maxClearCount) {
                maxClearCount = clearCount;
                localStorage.setItem("slidingMazeMaxClearCount", String(maxClearCount));
            }
            try {
                localStorage.setItem("slideMazeBestStreak", String(allTimeBestStreak));
            } catch (error) {}
            if (activeItem === "energyShield" && clearCount % 2 === 0) {
                shieldCharges++;
            }
            if (activeItem === "firstAid" && clearCount % 4 === 0) {
                firstAidCharged = true;
            }
            // 멀티플레이 라운드에서 클리어 기록이 갱신된 직후 서버에 저장합니다.
            // 단독 플레이 클리어 함수에만 의존하면 멀티플레이 기록이 누락될 수 있습니다.
            void submitV28Score();
        } else if (winner !== "draw") {
            clearStreak = 0;
        }

        movement = null;
        if (multiplayerRole === "host") {
            startNextMultiplayerRound(
                data.nextStart && Number.isFinite(Number(data.nextStart.c)) && Number.isFinite(Number(data.nextStart.r))
                    ? { c: Number(data.nextStart.c), r: Number(data.nextStart.r) }
                    : { c: player.c, r: player.r }
            );
        } else {
            gameState = "multiplayerWaitingRound";
            setMessage(winner === multiplayerRole ? "클리어! 다음 맵을 준비합니다." : "상대가 먼저 클리어했습니다. 다음 맵을 기다리는 중...");
            updateUI();
        }
        return;
    }
    if (data.type === "matchOver") {
        if (!multiplayerMatchActive && gameState !== "multiplayerWaitingResult") return;
        if (data.scores) {
            multiplayerScores = data.scores;
            multiplayerFinalScores = data.scores;
        }
        multiplayerMatchActive = false;
        multiplayerResult = data.winner || "draw";
        onDailyQuestMultiplayerMatchEnd(multiplayerResult);
        playMultiplayerResultSound(multiplayerResult);
        gameState = "multiplayerResult";
        movement = null;
        multiplayerOpen = false;
        pendingExpAward = calculateMultiplayerExperience();
        pendingExpReason = multiplayerResult === multiplayerRole ? "multiplayer_win" : "multiplayer_loss";
        // 멀티플레이의 정상 종료(matchOver)에서도 최종 기록을 저장합니다.
        // 기존에는 라운드 클리어 때만 저장되어, 목숨 소진으로 경기가 끝나면
        // 마지막 기록/랭킹 갱신 요청이 누락될 수 있었습니다.
        void submitV28Score();
        void submitPlayStats("multiplayer", getMultiplayerOutcome());
        setMessage(
            multiplayerResult === multiplayerRole ? "승리했습니다!" :
            multiplayerResult === "draw" ? "무승부입니다." : "패배했습니다."
        );
        updateUI();
    }
}

function startMultiplayerMatch() {
    logMultiplayerDebug("startMultiplayerMatchCalled", { roleAllowed: multiplayerRole === "host", round: multiplayerRound });
    if (multiplayerRole !== "host" || !multiplayerConnected || !multiplayerPeerJoined) {
        logMultiplayerDebug("startMultiplayerMatchSkipped", { reason: "role-or-connection-not-ready" });
        return;
    }
    hideLoadingScreen();
    multiplayerSeed = generateMatchSeed();
    multiplayerRound = 1;
    multiplayerMatchActive = true;
    logMultiplayerDebug("hostGameStarting", { round: multiplayerRound, seed: multiplayerSeed });
    opponentEliminatedRound = 0;
    multiplayerScores = { host: 0, guest: 0 };
    multiplayerFinalScores = null;
    multiplayerResult = null;
    multiplayerResultSoundPlayed = false;
    resetOneShotEffects();
    multiplayerEliminatedSent = false;
    multiplayerSelfDead = false;
    multiplayerRoundTransition = false;
    multiplayerOpen = false;
    startNewGame();   // 끝에서 3초 카운트다운이 시작됩니다.
    gameplayUIAccumulator = 0;
    gameState = countdownActive ? "countdown" : "playing";
    multiplayerOpen = false;
    questOpen = false;
    shopOpen = false;
    inventoryOpen = false;
    skinOpen = false;
    settingsOpen = false;
    onDailyQuestMultiplayerMatchStart(multiplayerMatchType || "quick");
    onDailyQuestMultiplayerRoundStart();
    updateUI();
    // 맵 데이터 배열은 보내지 않고 시드만 전달합니다. 참가자도 같은 맵을 생성합니다.
    multiplayerSend({
        type: "matchStart", round: multiplayerRound, seed: multiplayerSeed,
        startPosition: { c: stageStart.c, r: stageStart.r }
    });
    resetOpponent();
    multiplayerPlayerVisible = true;
    gameState = countdownActive ? "countdown" : "playing";
    updateUI();
    sendMultiplayerPosition(true);
}

// 먼저 죽은 플레이어도 다음 라운드 맵을 만들어 상대를 관전할 수 있게 합니다.
function buildSpectatorMap() {
    movement = null;
    mapTransition.active = false;
    pathGuidePath = [];
    createMapWithSeed(multiplayerSeed);
    // createMap이 gameState를 "transition"으로 바꾸므로 관전 상태로 되돌립니다.
    gameState = "multiplayerWaitingResult";
    remainingTime = getStageTimeLimit();
    setMessage("관전 중 · 상대 플레이어의 경기가 끝나기를 기다립니다.");
    updateUI();
}

function startNextMultiplayerRound(nextStart = { c: player.c, r: player.r }) {
    if (multiplayerRole !== "host" || !multiplayerMatchActive) return;

    clearTimeout(roundTimer);
    multiplayerRound++;
    multiplayerSeed = generateMatchSeed();
    stageStart = {
        c: Number(nextStart.c),
        r: Number(nextStart.r)
    };

    // 죽은 방장은 직접 플레이하지 않고, 상대에게 다음 라운드만 알립니다.
    if (multiplayerSelfDead) {
        multiplayerSend({
            type: "matchStart", round: multiplayerRound, seed: multiplayerSeed,
            startPosition: { c: stageStart.c, r: stageStart.r }
        });
        opponentEliminatedRound = 0;
        opponent.visible = false;
        buildSpectatorMap();
        return;
    }

    multiplayerEliminatedSent = false;
    multiplayerRoundTransition = false;
    multiplayerPlayerVisible = true;

    startRound();
    onDailyQuestMultiplayerRoundStart();

    // 다음 라운드도 맵 배열 대신 새 시드만 전달합니다.
    multiplayerSend({
        type: "matchStart", round: multiplayerRound, seed: multiplayerSeed,
        startPosition: { c: stageStart.c, r: stageStart.r }
    });
    resetOpponent();
    sendMultiplayerPosition(true);
}

function sendMultiplayerEliminated() {
    if (!multiplayerMatchActive || multiplayerEliminatedSent) return;

    // 목숨을 잃으면 해당 라운드에서 캐릭터를 즉시 숨깁니다.
    // 남은 목숨이 있어도 같은 맵에서 부활하지 않고 다음 맵을 기다립니다.
    multiplayerEliminatedSent = true;
    multiplayerPlayerVisible = false;
    movement = null;
    opponent.visible = false;
    multiplayerSend({
        type: "eliminated",
        round: multiplayerRound,
        livesRemaining: Math.max(0, lives),
        position: { c: player.c, r: player.r }
    });

    if (lives <= 0) {
        multiplayerSelfDead = true;
        onDailyQuestMultiplayerElimination();
        multiplayerRoundTransition = false;
        gameState = "multiplayerWaitingResult";
        setMessage("목숨을 모두 잃었습니다. 관전 중 · 상대의 경기가 끝나기를 기다립니다.");
    } else {
        gameState = "multiplayerWaitingRound";
        setMessage(`목숨을 잃었습니다. ${lives}개 남음 · 다음 맵을 기다리는 중...`);
    }
    updateUI();
}

function generateRoomCode() {
    const chars = "ABCDEFGHJKLMNPQRSTUVWXYZ23456789";
    let code = "";
    for (let i = 0; i < 5; i++) {
        code += chars[Math.floor(Math.random() * chars.length)];
    }
    return code;
}

function generateMatchSeed() {
    return Math.floor(Math.random() * 900000) + 100000;
}

function isMultiplayerPending() {
    return multiplayerOpen || multiplayerMatchmaking ||
        (!!multiplayerRole && !!multiplayerSocket && !multiplayerMatchActive && gameState === "start");
}

function openMultiplayerMenu() {
    multiplayerOpen = true;
    multiplayerMatchType = null;
    multiplayerRole = null;
    multiplayerRoomCode = "";
    multiplayerSeed = 0;
}

function closeMultiplayerMenu() {
    multiplayerOpen = false;
    multiplayerRole = null;
    closeMultiplayerSocket();
}

function createMultiplayerRoom() {
    multiplayerRole = "host";
    multiplayerRoomCode = generateRoomCode();
    multiplayerSeed = generateMatchSeed();
    connectMultiplayerSocket(() => {
        multiplayerMatchType = "friend";
        multiplayerSend({ type: "create", room: multiplayerRoomCode });
    });
}

function joinMultiplayerRoom() {
    const code = window.prompt("친구에게 받은 5자리 방 코드를 입력하세요.");
    if (!code) return;

    const normalized = code.trim().toUpperCase();
    if (!/^[A-Z0-9]{5}$/.test(normalized)) {
        window.alert("방 코드는 영문/숫자 5자리입니다.");
        return;
    }

    multiplayerRole = "guest";
    multiplayerRoomCode = normalized;
    multiplayerSeed = 0;
    connectMultiplayerSocket(() => {
        multiplayerMatchType = "friend";
        multiplayerSend({ type: "join", room: multiplayerRoomCode });
    });
}

async function copyMultiplayerRoomCode() {
    const code = String(multiplayerRoomCode || "").trim().toUpperCase();
    if (!code) {
        setMessage("복사할 방 코드가 없습니다.");
        updateUI();
        return;
    }

    try {
        if (navigator.clipboard && typeof navigator.clipboard.writeText === "function") {
            await navigator.clipboard.writeText(code);
        } else {
            const textarea = document.createElement("textarea");
            textarea.value = code;
            textarea.setAttribute("readonly", "");
            textarea.style.position = "fixed";
            textarea.style.left = "-9999px";
            textarea.style.top = "0";
            document.body.appendChild(textarea);
            textarea.focus();
            textarea.select();
            const copied = document.execCommand("copy");
            textarea.remove();
            if (!copied) throw new Error("copy failed");
        }
        setMessage(`방 코드 ${code}가 복사되었습니다.`);
        updateUI();
    } catch (error) {
        window.prompt("방 코드를 복사하세요.", code);
    }
}

function drawMultiplayerMenu() {
    ctx.save();

    ctx.fillStyle = "rgba(5,8,13,0.90)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);

    const panel = { x: 135, y: 80, w: 530, h: 440 };

    ctx.fillStyle = "#151b24";
    ctx.strokeStyle = "#425063";
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.roundRect(panel.x, panel.y, panel.w, panel.h, 22);
    ctx.fill();
    ctx.stroke();

    ctx.textAlign = "center";
    ctx.textBaseline = "middle";

    ctx.fillStyle = "#f3f5f7";
    ctx.font = "bold 30px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("2인 대전", WIDTH / 2, 125);

    if (multiplayerMatchmaking) {
        ctx.fillStyle = "#aeb8c4";
        ctx.font = "15px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("빠른 대전에서 상대 플레이어를 찾고 있습니다.", WIDTH / 2, 180);
        ctx.fillStyle = "#63ff91";
        ctx.font = "bold 24px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("상대를 찾는 중...", WIDTH / 2, 255);
        drawSettingsButton(205, 345, 390, 48, "매칭 취소");
    } else if (!multiplayerRole) {
        ctx.fillStyle = "#aeb8c4";
        ctx.font = "15px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("빠른 대전 또는 방 코드로 상대를 찾을 수 있습니다.", WIDTH / 2, 165);

        drawSettingsButton(205, 205, 390, 52, "⚡ 빠른 대전");
        drawSettingsButton(205, 275, 390, 52, "방 만들기");
        drawSettingsButton(205, 345, 390, 52, "방 참가하기");
        drawSettingsButton(305, 415, 190, 42, "돌아가기");
    } else if (multiplayerRole === "host") {
        ctx.fillStyle = "#7ddcff";
        ctx.font = "600 18px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("HOST · 방장", WIDTH / 2, 170);

        ctx.fillStyle = "#ffffff";
        ctx.font = "bold 48px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(multiplayerRoomCode, WIDTH / 2, 235);

        ctx.fillStyle = "#9ba7b5";
        ctx.font = "14px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("친구에게 이 방 코드를 알려주세요.", WIDTH / 2, 270);

        drawSettingsButton(305, 292, 190, 38, "📋 코드 복사");

        ctx.fillStyle = multiplayerPeerJoined ? "#63ff91" : "#ffbd66";
        ctx.font = "600 14px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(multiplayerPeerJoined ? "상대 플레이어 참가 완료" : multiplayerStatus, WIDTH / 2, 345);

        drawSettingsButton(205, 365, 180, 48, multiplayerPeerJoined ? "경기 시작" : "대기 중...");
        drawSettingsButton(415, 365, 180, 48, "새 방 코드");
        drawSettingsButton(205, 430, 390, 42, "돌아가기");

        ctx.fillStyle = "#687585";
        ctx.font = "13px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(`경기 시드: ${multiplayerSeed}`, WIDTH / 2, 495);
    } else {
        ctx.fillStyle = "#b8f0ff";
        ctx.font = "600 18px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("PLAYER 2 · 참가자", WIDTH / 2, 170);

        ctx.fillStyle = "#ffffff";
        ctx.font = "bold 42px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(multiplayerRoomCode, WIDTH / 2, 235);

        ctx.fillStyle = "#9ba7b5";
        ctx.font = "14px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("입력한 방 코드가 준비되었습니다.", WIDTH / 2, 275);
        ctx.fillStyle = "#63ff91";
        ctx.font = "600 14px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(multiplayerStatus, WIDTH / 2, 305);

        drawSettingsButton(205, 345, 180, 48, "다른 방 참가");
        drawSettingsButton(415, 345, 180, 48, "돌아가기");
    }

    ctx.restore();
}


/* =========================================================
   화면 설정
========================================================= */

const WALL_COLORS = [
    { name: "슬레이트", value: "#2b3441" },
    { name: "강철", value: "#46515f" },
    { name: "심해", value: "#1f4a6e" },
    { name: "자수정", value: "#4b3a6b" },
    { name: "이끼", value: "#2f5a47" },
    { name: "구리", value: "#6b4a35" },
    { name: "로즈", value: "#6b3a4a" }
];

const BACKGROUND_COLORS = [
    { name: "기본", value: "#0d1117" },
    { name: "자정", value: "#0a1226" },
    { name: "보랏빛 밤", value: "#150f24" },
    { name: "숲", value: "#0a1a14" },
    { name: "와인", value: "#1c0e14" },
    { name: "모래빛 밤", value: "#1a1610" },
    { name: "순흑", value: "#05070a" }
];

/* 기존 색상 목록의 마지막에 "사용자 지정"을 추가 */
WALL_COLORS.push({
    name: "사용자 지정",
    value: null,
    custom: true
});

BACKGROUND_COLORS.push({
    name: "사용자 지정",
    value: null,
    custom: true
});


/* =========================================================
   위험 블록 스킨
========================================================= */

const DANGER_SKINS = [
    { name: "기본", value: "solid" },
    { name: "가시", value: "spike" },
    { name: "레이저", value: "laser" },
    { name: "용암", value: "lava" },
    { name: "폭탄", value: "bomb" },
    { name: "전기", value: "electric" },
    { name: "독", value: "toxic" },
    { name: "심연", value: "void" },
    { name: "얼음", value: "ice" },
    { name: "장미 덩굴", value: "thorn" },
    { name: "황금 함정", value: "trap" },
    { name: "네온", value: "neon" }
];


const STREAK_EFFECTS = [
    { name: "없음", value: "none" },
    { name: "오로라", value: "aurora" },
    { name: "불씨", value: "ember" },
    { name: "번개", value: "lightning" },
    { name: "꽃잎", value: "petals" },
    { name: "맥동", value: "pulse" },
    { name: "혜성", value: "comet" },
    { name: "프리즘", value: "prism" },
    { name: "눈보라", value: "snow" },
    { name: "독 포자", value: "spore" },
    { name: "황금 비", value: "goldRain" },
    { name: "네온", value: "neon" },
    { name: "레인보우 네온", value: "rainbowNeon" }
];


/* =========================================================
   플레이어 스킨 / 잔상 효과
========================================================= */

const PLAYER_SKINS = [
    { name: "기본", value: "classic" },
    { name: "둥근", value: "round" },
    { name: "슬라임", value: "slime" },
    { name: "네온", value: "neon" },
    { name: "황금", value: "gold" },
    { name: "로봇", value: "robot" },
    { name: "다이아", value: "diamond" },
    { name: "구슬", value: "orb" },
    { name: "마그마", value: "magma" },
    { name: "얼음 큐브", value: "ice" },
    { name: "벚꽃", value: "blossom" }
];

const PLAYER_TRAILS = [
    { name: "기본", value: "default" },
    { name: "없음", value: "none" },
    { name: "무지개", value: "rainbow" },
    { name: "불꽃", value: "fire" },
    { name: "별가루", value: "sparkle" },
    { name: "네온", value: "neon" },
    { name: "고스트", value: "ghost" },
    { name: "글리치", value: "glitch" },
    { name: "거품", value: "bubble" },
    { name: "서리", value: "frost" },
    { name: "꽃잎", value: "petal" },
    { name: "금화", value: "coin" }
];

const GOAL_SKINS = [
    { name: "기본", value: "classic" },
    { name: "포털", value: "portal" },
    { name: "깃발", value: "flag" },
    { name: "별", value: "star" },
    { name: "수정", value: "crystal" },
    { name: "신호탑", value: "beacon" },
    { name: "보물상자", value: "chest" },
    { name: "레이더", value: "radar" },
    { name: "횃불", value: "torch" },
    { name: "독 가마솥", value: "cauldron" },
    { name: "눈꽃", value: "snowflake" },
    { name: "도리이", value: "torii" },
    { name: "네온", value: "neon" }
];

function getGoalSkinValue() {
    return (GOAL_SKINS[visualSettings.goalSkin] || GOAL_SKINS[0]).value;
}

/* x, y = 그려질 정사각형의 왼쪽 위, size = 한 변 (게임에서는 CELL - 10 = 30) */
function drawGoalSkin(skin, x, y, size = CELL - 10) {
    const t = performance.now() * 0.001;
    ctx.save();
    ctx.translate(x, y);
    ctx.scale(size / 30, size / 30);
    switch (skin) {
        case "portal": {
            ctx.fillStyle = "rgba(15,20,60,0.9)";
            ctx.beginPath(); ctx.arc(15, 15, 14, 0, Math.PI * 2); ctx.fill();
            for (let i = 0; i < 3; i++) {
                ctx.strokeStyle = `hsla(${190 + i * 50},100%,68%,0.95)`;
                ctx.lineWidth = 2.4; ctx.shadowBlur = 7; ctx.shadowColor = ctx.strokeStyle;
                const a0 = t * (i % 2 ? 2.4 : -2.9) + i * 2;
                ctx.beginPath(); ctx.arc(15, 15, 12.5 - i * 3.8, a0, a0 + Math.PI * 1.35); ctx.stroke();
            }
            ctx.shadowBlur = 0;
            ctx.fillStyle = `rgba(255,255,255,${0.6 + Math.sin(t * 5) * 0.3})`;
            ctx.beginPath(); ctx.arc(15, 15, 2.4, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "flag": {
            ctx.fillStyle = "#5d6877"; ctx.beginPath(); ctx.ellipse(9, 29, 10, 3, 0, 0, Math.PI * 2); ctx.fill();
            ctx.fillStyle = "#f0f4f8"; ctx.fillRect(7.5, -1, 3.5, 30);
            ctx.shadowBlur = 8; ctx.shadowColor = "rgba(255,215,106,0.9)";
            ctx.fillStyle = "#ffd76a"; ctx.beginPath(); ctx.arc(9.2, -1.5, 3.4, 0, Math.PI * 2); ctx.fill();
            ctx.shadowBlur = 0;
            ctx.beginPath(); ctx.moveTo(11, 1);
            for (let i = 0; i <= 10; i++) ctx.lineTo(11 + i * 1.9, 1 + Math.sin(t * 6 - i * 0.7) * 2 * (i / 10));
            for (let i = 10; i >= 0; i--) ctx.lineTo(11 + i * 1.9, 15 + Math.sin(t * 6 - i * 0.7) * 2 * (i / 10));
            ctx.closePath();
            const g = ctx.createLinearGradient(11, 0, 30, 0); g.addColorStop(0, "#ff4d63"); g.addColorStop(1, "#ff9d5c");
            ctx.fillStyle = g; ctx.fill();
            ctx.strokeStyle = "rgba(255,255,255,0.55)"; ctx.lineWidth = 1.2; ctx.stroke();
            break;
        }
        case "star": {
            const pulse = 1 + Math.sin(t * 4) * 0.08;
            ctx.translate(15, 15.5); ctx.scale(pulse, pulse); ctx.rotate(Math.sin(t * 1.6) * 0.15);
            ctx.shadowBlur = 10; ctx.shadowColor = "rgba(255,215,106,0.9)";
            const g = ctx.createRadialGradient(0, -2, 1, 0, 0, 15); g.addColorStop(0, "#fff3b0"); g.addColorStop(1, "#ffb81c");
            ctx.fillStyle = g; ctx.beginPath();
            for (let i = 0; i < 10; i++) {
                const r = i % 2 === 0 ? 14.5 : 6.4, a = -Math.PI / 2 + i * Math.PI / 5;
                i ? ctx.lineTo(Math.cos(a) * r, Math.sin(a) * r) : ctx.moveTo(Math.cos(a) * r, Math.sin(a) * r);
            }
            ctx.closePath(); ctx.fill();
            break;
        }
        case "crystal": {
            const bob = Math.sin(t * 2.5) * 1.2;
            ctx.translate(0, bob);
            ctx.shadowBlur = 9; ctx.shadowColor = "rgba(120,220,255,0.8)";
            const pts = [[15, 1], [26, 9], [26, 21], [15, 29], [4, 21], [4, 9]];
            const g = ctx.createLinearGradient(4, 0, 26, 30); g.addColorStop(0, "#d4f7ff"); g.addColorStop(1, "#2f86e0");
            ctx.fillStyle = g; ctx.beginPath(); pts.forEach((p, i) => i ? ctx.lineTo(p[0], p[1]) : ctx.moveTo(p[0], p[1])); ctx.closePath(); ctx.fill();
            ctx.shadowBlur = 0; ctx.strokeStyle = "rgba(255,255,255,0.6)"; ctx.lineWidth = 1.2; ctx.stroke();
            ctx.beginPath(); ctx.moveTo(4, 9); ctx.lineTo(15, 15); ctx.lineTo(26, 9); ctx.moveTo(15, 15); ctx.lineTo(15, 29); ctx.stroke();
            ctx.fillStyle = `rgba(255,255,255,${0.4 + (Math.sin(t * 5) + 1) * 0.25})`;
            ctx.beginPath(); ctx.arc(10, 8, 1.8, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "beacon": {
            const pulse = 0.75 + Math.sin(t * 4) * 0.25;
            const bg = ctx.createLinearGradient(0, 22, 0, -10);
            bg.addColorStop(0, `rgba(120,235,255,${0.95 * pulse})`); bg.addColorStop(1, "rgba(120,235,255,0)");
            ctx.fillStyle = bg; ctx.beginPath(); ctx.moveTo(8, 22); ctx.lineTo(22, 22); ctx.lineTo(27, -10); ctx.lineTo(3, -10); ctx.closePath(); ctx.fill();
            for (let i = 0; i < 2; i++) {
                const p = (t * 0.9 + i * 0.5) % 1;
                ctx.strokeStyle = `rgba(160,245,255,${1 - p})`; ctx.lineWidth = 2;
                ctx.beginPath(); ctx.ellipse(15, 28, 6 + p * 12, 2 + p * 4, 0, 0, Math.PI * 2); ctx.stroke();
            }
            ctx.fillStyle = "#39475a"; ctx.strokeStyle = "#7fdcf0"; ctx.lineWidth = 1.5;
            ctx.beginPath(); ctx.ellipse(15, 28, 13, 3.5, 0, 0, Math.PI * 2); ctx.fill(); ctx.stroke();
            ctx.fillStyle = "#56677f"; ctx.beginPath(); ctx.moveTo(9, 28); ctx.lineTo(21, 28); ctx.lineTo(18, 13); ctx.lineTo(12, 13); ctx.closePath(); ctx.fill();
            ctx.strokeStyle = "#a9ecff"; ctx.stroke();
            ctx.shadowBlur = 14; ctx.shadowColor = "#6fe6ff";
            ctx.fillStyle = `rgba(235,252,255,${0.7 + pulse * 0.3})`; ctx.beginPath(); ctx.arc(15, 10, 5.5, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "chest": {
            const tw = (Math.sin(t * 4) + 1) / 2;
            ctx.shadowBlur = 6 + tw * 6; ctx.shadowColor = "rgba(255,210,90,0.8)";
            ctx.fillStyle = "#8a5a2b"; ctx.beginPath(); ctx.roundRect(2, 12, 26, 16, 3); ctx.fill();
            ctx.fillStyle = "#a86d35"; ctx.beginPath(); ctx.roundRect(2, 3, 26, 11, 5); ctx.fill();
            ctx.shadowBlur = 0;
            ctx.fillStyle = "#f5c232"; ctx.fillRect(12.5, 3, 5, 25);
            ctx.fillStyle = "#fff0b3"; ctx.fillRect(12, 13, 6, 6);
            ctx.strokeStyle = "#4a2d12"; ctx.lineWidth = 1.4; ctx.beginPath(); ctx.roundRect(2, 3, 26, 25, 4); ctx.stroke();
            ctx.fillStyle = `rgba(255,255,255,${0.3 + tw * 0.6})`; ctx.beginPath(); ctx.arc(23, 7, 1.2 + tw, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "radar": {
            ctx.fillStyle = "#08180f"; ctx.beginPath(); ctx.arc(15, 15, 14.5, 0, Math.PI * 2); ctx.fill();
            ctx.strokeStyle = "rgba(90,255,150,0.55)"; ctx.lineWidth = 1;
            [14, 9.5, 5].forEach(r => { ctx.beginPath(); ctx.arc(15, 15, r, 0, Math.PI * 2); ctx.stroke(); });
            ctx.beginPath(); ctx.moveTo(0.5, 15); ctx.lineTo(29.5, 15); ctx.moveTo(15, 0.5); ctx.lineTo(15, 29.5); ctx.stroke();
            const a = t * 3;
            for (let i = 0; i < 14; i++) {
                ctx.fillStyle = `rgba(90,255,150,${0.34 - i * 0.024})`;
                ctx.beginPath(); ctx.moveTo(15, 15); ctx.arc(15, 15, 14, a - (i + 1) * 0.07, a - i * 0.07); ctx.closePath(); ctx.fill();
            }
            ctx.fillStyle = `rgba(220,255,230,${0.6 + Math.sin(t * 6) * 0.4})`;
            ctx.beginPath(); ctx.arc(15, 15, 2.4, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "torch": {
            const glow = ctx.createRadialGradient(15, 6, 2, 15, 6, 22);
            glow.addColorStop(0, `rgba(255,150,40,${0.5 + Math.sin(t * 8) * 0.08})`);
            glow.addColorStop(1, "rgba(255,150,40,0)");
            ctx.fillStyle = glow; ctx.fillRect(-8, -14, 46, 48);
            ctx.fillStyle = "#8a5a2b"; ctx.beginPath(); ctx.roundRect(11, 16, 8, 15, 2); ctx.fill();
            ctx.fillStyle = "#5a381a"; ctx.fillRect(11, 16, 2.6, 15);
            ctx.fillStyle = "#59606b"; ctx.beginPath(); ctx.roundRect(7, 12.5, 16, 5, 2); ctx.fill();
            ctx.strokeStyle = "#aab4c0"; ctx.lineWidth = 1; ctx.beginPath(); ctx.roundRect(7, 12.5, 16, 5, 2); ctx.stroke();
            const cols = ["#ff4a14", "#ff9a24", "#fff0a0"];
            for (let n = 0; n < 3; n++) {
                const f = Math.sin(t * 9 + n * 2) * 1.8, h = 18 - n * 4.5, hw = 8.5 - n * 2.2;
                ctx.fillStyle = cols[n]; ctx.shadowBlur = n === 0 ? 16 : 0; ctx.shadowColor = "#ff7a1f";
                ctx.beginPath(); ctx.moveTo(15 - hw, 13);
                ctx.quadraticCurveTo(15 - hw + f, 13 - h * 0.55, 15 + f * 0.7, 13 - h);
                ctx.quadraticCurveTo(15 + hw + f, 13 - h * 0.55, 15 + hw, 13);
                ctx.closePath(); ctx.fill();
            }
            ctx.shadowBlur = 0;
            for (let n = 0; n < 3; n++) {
                const p = (t * 0.9 + n * 0.33) % 1;
                ctx.fillStyle = `rgba(255,200,90,${1 - p})`;
                ctx.beginPath(); ctx.arc(15 + Math.sin(t * 3 + n * 2) * 6, 4 - p * 12, 1.4, 0, Math.PI * 2); ctx.fill();
            }
            break;
        }
        case "cauldron": {
            const fog = ctx.createRadialGradient(15, 10, 2, 15, 10, 22);
            fog.addColorStop(0, "rgba(110,255,90,0.35)"); fog.addColorStop(1, "rgba(110,255,90,0)");
            ctx.fillStyle = fog; ctx.fillRect(-8, -12, 46, 44);
            ctx.fillStyle = "rgba(0,0,0,0.4)"; ctx.beginPath(); ctx.ellipse(15, 30, 13, 3, 0, 0, Math.PI * 2); ctx.fill();
            ctx.fillStyle = "#59606b"; ctx.fillRect(5, 26, 4, 5); ctx.fillRect(21, 26, 4, 5);
            const bodyG = ctx.createLinearGradient(0, 12, 0, 29); bodyG.addColorStop(0, "#5b6a62"); bodyG.addColorStop(1, "#242b27");
            ctx.fillStyle = bodyG; ctx.beginPath(); ctx.moveTo(2, 12); ctx.quadraticCurveTo(-1, 28, 15, 28); ctx.quadraticCurveTo(31, 28, 28, 12); ctx.closePath(); ctx.fill();
            ctx.strokeStyle = "#a9bdb1"; ctx.lineWidth = 1.6; ctx.stroke();
            ctx.fillStyle = "#6b7b72"; ctx.beginPath(); ctx.ellipse(15, 12, 14, 4.5, 0, 0, Math.PI * 2); ctx.fill(); ctx.stroke();
            ctx.fillStyle = "#86ff5e"; ctx.shadowBlur = 14; ctx.shadowColor = "#6bff4a";
            ctx.beginPath(); ctx.ellipse(15, 12, 11.5, 3.2, 0, 0, Math.PI * 2); ctx.fill();
            ctx.shadowBlur = 0;
            for (let n = 0; n < 4; n++) {
                const p = (t * 0.8 + n * 0.25) % 1;
                ctx.strokeStyle = `rgba(190,255,160,${1 - p})`; ctx.lineWidth = 1.6;
                ctx.beginPath(); ctx.arc(8 + n * 5 + Math.sin(t * 2 + n) * 2, 11 - p * 14, 2 + n % 2 * 1.2, 0, Math.PI * 2); ctx.stroke();
            }
            break;
        }
        case "snowflake": {
            const gl = ctx.createRadialGradient(15, 15, 2, 15, 15, 20);
            gl.addColorStop(0, "rgba(150,225,255,0.38)"); gl.addColorStop(1, "rgba(150,225,255,0)");
            ctx.fillStyle = gl; ctx.fillRect(-8, -8, 46, 46);
            ctx.translate(15, 15); ctx.rotate(t * 0.5);
            ctx.shadowBlur = 12; ctx.shadowColor = "rgba(150,225,255,0.95)";
            ctx.strokeStyle = "#dcf7ff"; ctx.lineWidth = 3; ctx.lineCap = "round";
            for (let a = 0; a < 6; a++) {
                ctx.save(); ctx.rotate(a * Math.PI / 3); ctx.beginPath();
                ctx.moveTo(0, 0); ctx.lineTo(0, -16);
                ctx.moveTo(0, -10); ctx.lineTo(-5, -15);
                ctx.moveTo(0, -10); ctx.lineTo(5, -15);
                ctx.moveTo(0, -5.5); ctx.lineTo(-3.5, -9);
                ctx.moveTo(0, -5.5); ctx.lineTo(3.5, -9);
                ctx.stroke(); ctx.restore();
            }
            ctx.fillStyle = "#fff"; ctx.beginPath(); ctx.arc(0, 0, 3.4, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "torii": {
            const glow = (Math.sin(t * 3) + 1) / 2;
            ctx.shadowBlur = 8 + glow * 8; ctx.shadowColor = "rgba(255,90,110,0.9)";
            ctx.fillStyle = "#e0334a";
            ctx.fillRect(5, 10, 4.6, 20); ctx.fillRect(20.4, 10, 4.6, 20);
            ctx.beginPath(); ctx.moveTo(-3, 3); ctx.quadraticCurveTo(15, 8, 33, 3); ctx.lineTo(31, 10); ctx.quadraticCurveTo(15, 6, -1, 10); ctx.closePath(); ctx.fill();
            ctx.fillRect(3, 14, 24, 3.6);
            ctx.shadowBlur = 0; ctx.fillStyle = "#2a1418"; ctx.fillRect(13, 6, 4, 8);
            ctx.fillStyle = "#6b2330"; ctx.fillRect(2, 29.5, 10, 2.5); ctx.fillRect(18, 29.5, 10, 2.5);
            ctx.fillStyle = "rgba(255,205,220,0.95)";
            for (let n = 0; n < 3; n++) {
                const p = (t * 0.5 + n * 0.33) % 1;
                ctx.beginPath(); ctx.ellipse(6 + n * 9 + Math.sin(t * 2 + n) * 2, 18 + p * 12, 1.8, 1.1, p * 3, 0, Math.PI * 2); ctx.fill();
            }
            break;
        }
        case "neon": {
            const pulse = 0.75 + Math.sin(t * 5) * 0.25;
            const ring = (t % 1.3) / 1.3;
            ctx.translate(15, 15); ctx.scale(1.2, 1.2); ctx.translate(-15, -15);
            ctx.strokeStyle = `rgba(55,245,255,${(1 - ring) * 0.7})`; ctx.lineWidth = 1.5;
            ctx.strokeRect(-ring * 4, -ring * 4, 30 + ring * 8, 30 + ring * 8);
            ctx.fillStyle = "#06181d"; ctx.fillRect(0, 0, 30, 30);
            ctx.strokeStyle = `rgba(55,245,255,${pulse})`; ctx.lineWidth = 2.8;
            ctx.shadowBlur = 12; ctx.shadowColor = "#37f5ff";
            ctx.strokeRect(2, 2, 26, 26);
            ctx.shadowBlur = 0;
            ctx.strokeStyle = "rgba(255,255,255,0.65)"; ctx.lineWidth = 1.2;
            ctx.strokeRect(8, 8, 14, 14);
            break;
        }
        case "classic":
        default: {
            const p = (t % 1.3) / 1.3;
            ctx.strokeStyle = `rgba(120,200,255,${(1 - p) * 0.8})`; ctx.lineWidth = 2;
            ctx.strokeRect(-p * 5, -p * 5, 30 + p * 10, 30 + p * 10);
            const g = ctx.createLinearGradient(0, 0, 30, 30); g.addColorStop(0, "#6cc0ff"); g.addColorStop(1, "#2a7fd6");
            ctx.fillStyle = g; ctx.beginPath(); ctx.roundRect(0, 0, 30, 30, 6); ctx.fill();
            ctx.fillStyle = "rgba(255,255,255,0.25)"; ctx.beginPath(); ctx.roundRect(5, 5, 20, 20, 4); ctx.fill();
            ctx.fillStyle = "#fff"; ctx.beginPath(); ctx.arc(15, 15, 3, 0, Math.PI * 2); ctx.fill();
        }
    }
    ctx.restore();
}

/* 테마 세트: 같은 컨셉의 스킨을 한 번에 장착 */
function skinIdx(list, value) { const i = list.findIndex(s => s.value === value); return i < 0 ? 0 : i; }
const SKIN_THEME_KEYS = ["wall", "background", "dangerSkin", "streakEffect", "playerSkin", "playerTrail", "goalSkin"];
const SKIN_THEMES = [
    { name: "⚪ 기본",   wall: 1, background: 0, dangerSkin: skinIdx(DANGER_SKINS, "spike"), streakEffect: skinIdx(STREAK_EFFECTS, "aurora"), playerSkin: 0, playerTrail: 0, goalSkin: 0 },
    { name: "🔥 화염",   wall: 5, background: 4, dangerSkin: skinIdx(DANGER_SKINS, "lava"),  streakEffect: skinIdx(STREAK_EFFECTS, "ember"),  playerSkin: skinIdx(PLAYER_SKINS, "magma"),   playerTrail: skinIdx(PLAYER_TRAILS, "fire"),   goalSkin: skinIdx(GOAL_SKINS, "torch") },
    { name: "⚡ 사이버", wall: 1, background: 1, dangerSkin: skinIdx(DANGER_SKINS, "laser"), streakEffect: skinIdx(STREAK_EFFECTS, "lightning"), playerSkin: skinIdx(PLAYER_SKINS, "neon"), playerTrail: skinIdx(PLAYER_TRAILS, "glitch"), goalSkin: skinIdx(GOAL_SKINS, "radar") },
    { name: "🌌 우주",   wall: 3, background: 2, dangerSkin: skinIdx(DANGER_SKINS, "void"),  streakEffect: skinIdx(STREAK_EFFECTS, "comet"),  playerSkin: skinIdx(PLAYER_SKINS, "orb"),     playerTrail: skinIdx(PLAYER_TRAILS, "sparkle"), goalSkin: skinIdx(GOAL_SKINS, "portal") },
    { name: "☠ 독 늪",  wall: 4, background: 3, dangerSkin: skinIdx(DANGER_SKINS, "toxic"), streakEffect: skinIdx(STREAK_EFFECTS, "spore"),  playerSkin: skinIdx(PLAYER_SKINS, "slime"),   playerTrail: skinIdx(PLAYER_TRAILS, "bubble"), goalSkin: skinIdx(GOAL_SKINS, "cauldron") },
    { name: "❄ 얼음",   wall: 2, background: 1, dangerSkin: skinIdx(DANGER_SKINS, "ice"),   streakEffect: skinIdx(STREAK_EFFECTS, "snow"),   playerSkin: skinIdx(PLAYER_SKINS, "ice"),     playerTrail: skinIdx(PLAYER_TRAILS, "frost"),  goalSkin: skinIdx(GOAL_SKINS, "snowflake") },
    { name: "🌸 벚꽃",   wall: 6, background: 2, dangerSkin: skinIdx(DANGER_SKINS, "thorn"), streakEffect: skinIdx(STREAK_EFFECTS, "petals"), playerSkin: skinIdx(PLAYER_SKINS, "blossom"), playerTrail: skinIdx(PLAYER_TRAILS, "petal"),  goalSkin: skinIdx(GOAL_SKINS, "torii") },
    { name: "💠 네온",   wall: 1, background: 6, dangerSkin: skinIdx(DANGER_SKINS, "neon"), streakEffect: skinIdx(STREAK_EFFECTS, "neon"), playerSkin: skinIdx(PLAYER_SKINS, "neon"), playerTrail: skinIdx(PLAYER_TRAILS, "neon"), goalSkin: skinIdx(GOAL_SKINS, "neon") },
    { name: "👑 보물",   wall: 5, background: 5, dangerSkin: skinIdx(DANGER_SKINS, "trap"),  streakEffect: skinIdx(STREAK_EFFECTS, "goldRain"), playerSkin: skinIdx(PLAYER_SKINS, "gold"),  playerTrail: skinIdx(PLAYER_TRAILS, "coin"),   goalSkin: skinIdx(GOAL_SKINS, "chest") }
];
const SKIN_THEME_BUTTON = { x: 94, y: 550, w: 220, h: 26 };

function getCurrentSkinThemeIndex() {
    return SKIN_THEMES.findIndex(th => SKIN_THEME_KEYS.every(k => visualSettings[k] === th[k]));
}

function cycleSkinTheme() {
    const next = (getCurrentSkinThemeIndex() + 1) % SKIN_THEMES.length;   // 직접 설정(-1)이면 첫 테마부터
    const th = SKIN_THEMES[next];
    SKIN_THEME_KEYS.forEach(k => { visualSettings[k] = th[k]; });
    visualSettings.customWall = null;
    visualSettings.customBackground = null;
    saveVisualSettings();
    requestSettingsRender();
}

// 스킨 화면의 행 구성 (그리기와 터치 판정이 같은 값을 사용합니다)
const SKIN_PANEL = { x: 70, y: 20, w: 660, h: 560 };
const SKIN_ROWS = [
    { key: "wall",         label: "벽 색상",          list: WALL_COLORS,       centerY: 116 },
    { key: "background",   label: "배경 색상",        list: BACKGROUND_COLORS, centerY: 183 },
    { key: "dangerSkin",   label: "위험 블록 스킨",   list: DANGER_SKINS,      centerY: 250 },
    { key: "streakEffect", label: "연속 클리어 효과", list: STREAK_EFFECTS,    centerY: 317 },
    { key: "playerSkin",   label: "플레이어 스킨",    list: PLAYER_SKINS,      centerY: 384 },
    { key: "playerTrail",  label: "플레이어 잔상",    list: PLAYER_TRAILS,     centerY: 451 },
    { key: "goalSkin",     label: "도착 지점 스킨",   list: GOAL_SKINS,        centerY: 518 }
];

function getPlayerSkinValue() {
    return (PLAYER_SKINS[visualSettings.playerSkin] || PLAYER_SKINS[0]).value;
}

function getPlayerTrailValue() {
    return (PLAYER_TRAILS[visualSettings.playerTrail] || PLAYER_TRAILS[0]).value;
}

/* x, y = 그려질 정사각형의 왼쪽 위, size = 한 변 (게임에서는 CELL - 10 = 30) */
function drawPlayerSkin(skin, x, y, size = CELL - 10) {
    const t = performance.now() * 0.001;

    ctx.save();
    ctx.translate(x, y);
    ctx.scale(size / 30, size / 30);

    switch (skin) {
        case "round": {
            ctx.fillStyle = "#2ec4b6";
            ctx.beginPath();
            ctx.roundRect(0, 0, 30, 30, 10);
            ctx.fill();
            ctx.fillStyle = "rgba(255,255,255,0.30)";
            ctx.beginPath();
            ctx.roundRect(5, 5, 20, 5, 2.5);
            ctx.fill();
            break;
        }

        case "slime": {
            const squish = Math.sin(t * 4) * 0.8;
            ctx.fillStyle = "#7be36b";
            ctx.beginPath();
            ctx.roundRect(0 - squish / 2, 2 + squish, 30 + squish, 28 - squish, 12);
            ctx.fill();
            ctx.fillStyle = "rgba(255,255,255,0.35)";
            ctx.beginPath();
            ctx.ellipse(8, 8 + squish, 4, 2.2, -0.5, 0, Math.PI * 2);
            ctx.fill();
            ctx.fillStyle = "#ffffff";
            ctx.beginPath();
            ctx.arc(10, 15 + squish, 4, 0, Math.PI * 2);
            ctx.arc(20, 15 + squish, 4, 0, Math.PI * 2);
            ctx.fill();
            ctx.fillStyle = "#111820";
            ctx.beginPath();
            ctx.arc(11, 16 + squish, 2, 0, Math.PI * 2);
            ctx.arc(21, 16 + squish, 2, 0, Math.PI * 2);
            ctx.fill();
            break;
        }

        case "neon": {
            const pulse = 0.75 + Math.sin(t * 5) * 0.25;
            ctx.translate(15, 15); ctx.scale(1.2, 1.2); ctx.translate(-15, -15);
            ctx.fillStyle = "#06170c";
            ctx.fillRect(0, 0, 30, 30);
            ctx.strokeStyle = `rgba(70,255,120,${pulse})`;
            ctx.lineWidth = 2.8;
            ctx.shadowBlur = 12;
            ctx.shadowColor = "#39ff6a";
            ctx.strokeRect(2, 2, 26, 26);
            ctx.shadowBlur = 0;
            ctx.strokeStyle = "rgba(200,255,215,0.65)";
            ctx.lineWidth = 1.2;
            ctx.strokeRect(8, 8, 14, 14);
            break;
        }
        case "gold": {
            const g = ctx.createLinearGradient(0, 0, 30, 30);
            g.addColorStop(0, "#fff3a8");
            g.addColorStop(0.5, "#f5c232");
            g.addColorStop(1, "#b8860b");
            ctx.fillStyle = g;
            ctx.fillRect(0, 0, 30, 30);
            ctx.strokeStyle = "#fff0b3";
            ctx.lineWidth = 1.5;
            ctx.strokeRect(0.75, 0.75, 28.5, 28.5);
            ctx.fillStyle = "rgba(255,255,255,0.45)";
            ctx.fillRect(5, 5, 20, 4);
            // 반짝이는 빛줄기
            const sweep = ((t * 0.7) % 1.6) * 50 - 20;
            ctx.save();
            ctx.beginPath();
            ctx.rect(0, 0, 30, 30);
            ctx.clip();
            ctx.fillStyle = "rgba(255,255,255,0.35)";
            ctx.beginPath();
            ctx.moveTo(sweep, 30);
            ctx.lineTo(sweep + 6, 30);
            ctx.lineTo(sweep + 18, 0);
            ctx.lineTo(sweep + 12, 0);
            ctx.closePath();
            ctx.fill();
            ctx.restore();
            break;
        }

        case "robot": {
            ctx.fillStyle = "#aab4c0";
            ctx.beginPath();
            ctx.roundRect(0, 0, 30, 30, 5);
            ctx.fill();
            ctx.fillStyle = "#0d1117";
            ctx.beginPath();
            ctx.roundRect(4, 8, 22, 10, 3);
            ctx.fill();
            const blink = Math.sin(t * 3) > 0.92 ? 1 : 4;
            ctx.fillStyle = "#37f5ff";
            ctx.shadowBlur = 6;
            ctx.shadowColor = "#37f5ff";
            ctx.fillRect(8, 11 + (4 - blink) / 2, 5, blink);
            ctx.fillRect(17, 11 + (4 - blink) / 2, 5, blink);
            ctx.shadowBlur = 0;
            ctx.fillStyle = "#5b6672";
            ctx.fillRect(9, 22, 12, 2);
            break;
        }

        case "diamond": {
            ctx.translate(15, 15);
            ctx.rotate(Math.PI / 4);
            const g = ctx.createLinearGradient(-11, -11, 11, 11);
            g.addColorStop(0, "#c9a8ff");
            g.addColorStop(1, "#7b4dff");
            ctx.fillStyle = g;
            ctx.fillRect(-10.5, -10.5, 21, 21);
            ctx.strokeStyle = "rgba(255,255,255,0.7)";
            ctx.lineWidth = 1.5;
            ctx.strokeRect(-10.5, -10.5, 21, 21);
            ctx.fillStyle = "rgba(255,255,255,0.35)";
            ctx.fillRect(-7, -7, 14, 3);
            break;
        }

        case "orb": {
            const g = ctx.createRadialGradient(11, 10, 1, 15, 15, 16);
            g.addColorStop(0, "#ffe6fa");
            g.addColorStop(0.45, "#ff7be0");
            g.addColorStop(1, "#b0229a");
            ctx.fillStyle = g;
            ctx.beginPath();
            ctx.arc(15, 15, 15, 0, Math.PI * 2);
            ctx.fill();
            ctx.fillStyle = "rgba(255,255,255,0.55)";
            ctx.beginPath();
            ctx.ellipse(10, 9, 4.5, 2.6, -0.6, 0, Math.PI * 2);
            ctx.fill();
            break;
        }

        case "magma": {
            const pulse = 0.6 + Math.sin(t * 4) * 0.4;
            ctx.fillStyle = "#2a0d08"; ctx.beginPath(); ctx.roundRect(0, 0, 30, 30, 6); ctx.fill();
            ctx.strokeStyle = `rgba(255,${Math.floor(120 + pulse * 80)},30,0.95)`; ctx.lineWidth = 2;
            ctx.shadowBlur = 8; ctx.shadowColor = "#ff6a1a";
            ctx.beginPath();
            ctx.moveTo(4, 10); ctx.lineTo(11, 14); ctx.lineTo(9, 22); ctx.lineTo(18, 19); ctx.lineTo(24, 26);
            ctx.moveTo(14, 3); ctx.lineTo(17, 11); ctx.lineTo(25, 9);
            ctx.stroke();
            ctx.shadowBlur = 0; ctx.strokeStyle = "#ff9a2a"; ctx.lineWidth = 1.5;
            ctx.beginPath(); ctx.roundRect(0.75, 0.75, 28.5, 28.5, 6); ctx.stroke();
            break;
        }
        case "ice": {
            const g = ctx.createLinearGradient(0, 0, 30, 30); g.addColorStop(0, "#e8fbff"); g.addColorStop(1, "#6cc4f0");
            ctx.fillStyle = g; ctx.beginPath(); ctx.roundRect(0, 0, 30, 30, 5); ctx.fill();
            ctx.strokeStyle = "rgba(255,255,255,0.85)"; ctx.lineWidth = 1.5; ctx.beginPath(); ctx.roundRect(1, 1, 28, 28, 5); ctx.stroke();
            ctx.fillStyle = "rgba(255,255,255,0.5)"; ctx.beginPath(); ctx.moveTo(4, 4); ctx.lineTo(14, 4); ctx.lineTo(4, 14); ctx.closePath(); ctx.fill();
            ctx.strokeStyle = "rgba(60,140,200,0.5)"; ctx.lineWidth = 1;
            ctx.beginPath(); ctx.moveTo(18, 30); ctx.lineTo(22, 18); ctx.lineTo(30, 14); ctx.stroke();
            const tw = (Math.sin(t * 4) + 1) / 2;
            ctx.fillStyle = `rgba(255,255,255,${0.4 + tw * 0.5})`; ctx.beginPath(); ctx.arc(23, 7, 1.6 + tw, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "blossom": {
            ctx.fillStyle = "#ffd6e6"; ctx.beginPath(); ctx.roundRect(0, 0, 30, 30, 12); ctx.fill();
            ctx.translate(15, 15); ctx.rotate(Math.sin(t * 1.5) * 0.15);
            for (let i = 0; i < 5; i++) {
                ctx.rotate(Math.PI * 2 / 5);
                ctx.fillStyle = "#ff8fb8"; ctx.beginPath(); ctx.ellipse(0, -7, 4.6, 6.2, 0, 0, Math.PI * 2); ctx.fill();
            }
            ctx.fillStyle = "#ffe9a8"; ctx.beginPath(); ctx.arc(0, 0, 3.4, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "classic":
        default: {
            ctx.fillStyle = "#45e77b";
            ctx.fillRect(0, 0, 30, 30);
            ctx.fillStyle = "rgba(255,255,255,0.30)";
            ctx.fillRect(5, 5, 20, 5);
        }
    }

    ctx.restore();
}

/* x, y = 잔상이 남은 칸의 왼쪽 위, k = 0~1 선명도(오래될수록 작음), i = 순서 */
function drawTrailPoint(effect, x, y, k, i, t) {
    if (effect === "none" || k <= 0) return;

    const cx = x + CELL / 2;
    const cy = y + CELL / 2;

    ctx.save();

    switch (effect) {
        case "rainbow": {
            ctx.globalCompositeOperation = "screen";
            ctx.fillStyle = `hsla(${(t * 160 + i * 28) % 360},100%,60%,${k * 0.65})`;
            ctx.beginPath();
            ctx.arc(cx, cy, 4 + 9 * k, 0, Math.PI * 2);
            ctx.fill();
            break;
        }

        case "fire": {
            ctx.globalCompositeOperation = "screen";
            const rise = (1 - k) * 14;
            ctx.fillStyle = `hsla(${8 + 36 * k},100%,55%,${k * 0.6})`;
            ctx.beginPath();
            ctx.arc(cx + Math.sin(i * 2.3 + t * 8) * 3, cy - rise, 3 + 9 * k, 0, Math.PI * 2);
            ctx.fill();
            break;
        }

        case "sparkle": {
            for (let m = 0; m < 2; m++) {
                const a = i * 2.399 + m * 3.1 + x * 0.13;
                const sx = cx + Math.sin(a) * 11;
                const sy = cy + Math.cos(a * 1.7) * 11;
                const s = (2 + 6 * k) * (m ? 0.65 : 1);
                const n = s * 0.28;
                ctx.fillStyle = `rgba(255,240,170,${Math.min(1, k * 1.1)})`;
                ctx.shadowBlur = 6;
                ctx.shadowColor = "rgba(255,230,120,0.9)";
                ctx.beginPath();
                ctx.moveTo(sx, sy - s);
                ctx.lineTo(sx + n, sy - n);
                ctx.lineTo(sx + s, sy);
                ctx.lineTo(sx + n, sy + n);
                ctx.lineTo(sx, sy + s);
                ctx.lineTo(sx - n, sy + n);
                ctx.lineTo(sx - s, sy);
                ctx.lineTo(sx - n, sy - n);
                ctx.closePath();
                ctx.fill();
            }
            break;
        }

        case "neon": {
            const size = 30 * (0.45 + 0.55 * k);
            const hue = (300 + i * 12) % 360;
            ctx.strokeStyle = `hsla(${hue},100%,65%,${k * 0.85})`;
            ctx.lineWidth = 2;
            ctx.shadowBlur = 10;
            ctx.shadowColor = `hsla(${hue},100%,65%,${k})`;
            ctx.beginPath();
            ctx.roundRect(cx - size / 2, cy - size / 2, size, size, 5);
            ctx.stroke();
            break;
        }

        case "ghost": {
            ctx.globalAlpha = k * 0.32;
            drawPlayerSkin(getPlayerSkinValue(), x + 5, y + 5, CELL - 10);
            break;
        }

        case "glitch": {
            ctx.globalCompositeOperation = "screen";
            const j = Math.sin(i * 7.1 + t * 30) * 3;
            ctx.fillStyle = `rgba(255,45,100,${k * 0.5})`;
            ctx.fillRect(cx - 12 + j - 3, cy - 12, 24, 24);
            ctx.fillStyle = `rgba(35,255,220,${k * 0.5})`;
            ctx.fillRect(cx - 12 - j + 3, cy - 12 + 2, 24, 24);
            ctx.fillStyle = `rgba(255,255,255,${k * 0.35})`;
            ctx.fillRect(cx - 14, cy - 3 + j, 28, 2);
            break;
        }

        case "bubble": {
            const rise = (1 - k) * 16;
            const r = 3 + 7 * k * (0.6 + fxHash(i + x * 0.1) * 0.6);
            const bx = cx + Math.sin(i * 2.1 + t * 3) * 6, by = cy - rise;
            ctx.fillStyle = `rgba(120,255,140,${k * 0.16})`; ctx.strokeStyle = `rgba(150,255,150,${k * 0.85})`; ctx.lineWidth = 1.4;
            ctx.beginPath(); ctx.arc(bx, by, r, 0, Math.PI * 2); ctx.fill(); ctx.stroke();
            ctx.fillStyle = `rgba(255,255,255,${k * 0.7})`;
            ctx.beginPath(); ctx.arc(bx - r * 0.35, by - r * 0.35, r * 0.22, 0, Math.PI * 2); ctx.fill();
            break;
        }

        case "frost": {
            ctx.globalCompositeOperation = "screen";
            ctx.strokeStyle = `rgba(190,240,255,${k * 0.85})`; ctx.lineWidth = 1.6;
            ctx.shadowBlur = 6; ctx.shadowColor = "rgba(150,220,255,0.9)";
            const s = 3 + 8 * k, rot = i * 0.7 + t * 0.6;
            for (let a = 0; a < 3; a++) {
                const ang = rot + a * Math.PI / 3;
                ctx.beginPath();
                ctx.moveTo(cx - Math.cos(ang) * s, cy - Math.sin(ang) * s);
                ctx.lineTo(cx + Math.cos(ang) * s, cy + Math.sin(ang) * s);
                ctx.stroke();
            }
            break;
        }

        case "petal": {
            const px = cx + Math.sin(i * 1.9 + t * 2) * 7, py = cy + (1 - k) * 8;
            ctx.translate(px, py); ctx.rotate(i * 1.1 + t * 2);
            ctx.fillStyle = `rgba(255,160,195,${k * 0.85})`;
            ctx.beginPath(); ctx.ellipse(0, 0, 2.5 + 4 * k, 1.6 + 2.2 * k, 0, 0, Math.PI * 2); ctx.fill();
            break;
        }

        case "coin": {
            const sx = Math.abs(Math.cos(i * 1.3 + t * 6)), rise = (1 - k) * 10;
            ctx.shadowBlur = 6; ctx.shadowColor = "rgba(255,210,80,0.9)";
            ctx.fillStyle = `rgba(255,205,70,${k})`;
            ctx.beginPath(); ctx.ellipse(cx + Math.sin(i * 2.7) * 6, cy - rise, (2 + 4.5 * k) * Math.max(0.25, sx), 2 + 4.5 * k, 0, 0, Math.PI * 2); ctx.fill();
            ctx.strokeStyle = `rgba(150,100,10,${k})`; ctx.lineWidth = 1; ctx.stroke();
            break;
        }

        case "default":
        default: {
            ctx.fillStyle = `rgba(91,205,255,${k * 0.18})`;
            ctx.beginPath();
            ctx.arc(cx, cy, 7, 0, Math.PI * 2);
            ctx.fill();
        }
    }

    ctx.restore();
}

/* 스킨 화면용: 선택한 스킨이 움직이며 잔상을 남기는 미리보기 */
function drawTrailPreviewInBox(effect, name, box) {
    const t = performance.now() * 0.001;
    const POINTS = 12;

    ctx.save();

    ctx.fillStyle = "rgba(255,255,255,0.055)";
    ctx.strokeStyle = "rgba(255,255,255,0.16)";
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.roundRect(box.x, box.y, box.w, box.h, 10);
    ctx.fill();
    ctx.stroke();

    ctx.beginPath();
    ctx.roundRect(box.x, box.y, box.w, box.h, 10);
    ctx.clip();

    const phase = (t % 1.8) / 1.8;
    const move = Math.min(1, phase / 0.6);
    const eased = 1 - Math.pow(1 - move, 3);
    const startX = box.x + 6;
    const headX = startX + eased * 190;
    const cellY = box.y + 1;
    const fade = Math.max(0, phase - 0.6) * 3.5;

    for (let j = POINTS - 1; j >= 0; j--) {
        const px = headX - j * 11;
        if (px < startX) continue;
        const life = Math.max(0, 1 - j * 0.07 - fade);
        const i = POINTS - 1 - j;
        const k = ((i + 1) / POINTS) * life;
        drawTrailPoint(effect, px, cellY, k, i, t);
    }

    drawPlayerSkin(getPlayerSkinValue(), headX + 5, cellY + 5, CELL - 10);

    ctx.fillStyle = "rgba(255,255,255,0.94)";
    ctx.font = "600 14px Pretendard, Noto Sans KR, sans-serif";
    ctx.textAlign = "right";
    ctx.textBaseline = "middle";
    ctx.fillText(name, box.x + box.w - 12, box.y + box.h / 2);

    ctx.restore();
}

const SETTINGS_KEY = "slidingMazeVisualSettings_v2";

/* =========================================================
   효과음: 필요할 때만 생성하여 초기 화면 로딩을 방해하지 않음
========================================================= */
const AUDIO_FILES = {
    goal: "goal.m4a",
    versusWin: "versus_win.m4a",
    versusLose: "versus_lose.m4a",
    damage: "damage.m4a",
    itemUse: "item_use.m4a",
    gameOver: "gameover.m4a",
    uiInvalid: "ui_invalid.m4a",
    uiClick: "ui_click.m4a",
    gameStart: "game_start.m4a"
};
const EFFECT_VOLUME_KEY = "slidingMazeEffectVolume_v1";
const MUSIC_VOLUME_KEY = "slidingMazeMusicVolume_v1";
let effectVolume = 0.70;
let musicVolume = 0.70;
const effectAudioCache = new Map();
let audioUnlocked = false;
const oneShotEffectPlayed = new Set();

function resetOneShotEffects() {
    oneShotEffectPlayed.clear();
}

try {
    const saved = Number(localStorage.getItem(EFFECT_VOLUME_KEY));
    if (Number.isFinite(saved)) effectVolume = Math.max(0, Math.min(1, saved));
    const savedMusic = Number(localStorage.getItem(MUSIC_VOLUME_KEY));
    if (Number.isFinite(savedMusic)) musicVolume = Math.max(0, Math.min(1, savedMusic));
} catch (error) {}

function saveEffectVolume() {
    try { localStorage.setItem(EFFECT_VOLUME_KEY, String(effectVolume)); } catch (error) {}
}

function setEffectVolume(value) {
    effectVolume = Math.max(0, Math.min(1, Number(value) || 0));
    for (const audio of effectAudioCache.values()) {
        audio.volume = getSoundVolumeForAudio(audio.__soundType || "");
    }
    saveEffectVolume();
    requestSettingsRender();
}

function getSoundVolume(type) {
    if (type === "uiClick") return effectVolume;
    if (type === "gameStart") return effectVolume * 0.12;
    return effectVolume;
}

function getSoundVolumeForAudio(type) {
    return getSoundVolume(type);
}

// 원본 게임에서 사용하던 오디오 준비 방식입니다.
// 첫 사용자 입력 때 각 효과음을 미리 생성/로드해 두어 모바일 브라우저의
// 자동재생 제한 때문에 게임 중 재생이 막히지 않도록 합니다.
function unlockEffectAudio() {
    if (audioUnlocked) return;
    audioUnlocked = true;

    try {
        for (const type of Object.keys(AUDIO_FILES)) {
            if (effectAudioCache.has(type)) continue;

            const audio = new Audio(AUDIO_FILES[type]);
            audio.preload = "auto";
            audio.__soundType = type;
            audio.volume = getSoundVolume(type);
            audio.setAttribute("playsinline", "");
            audio.addEventListener("error", () => console.warn(`[SOUND] ${type} 파일을 불러오지 못했습니다: ${AUDIO_FILES[type]}`));
            effectAudioCache.set(type, audio);

            try { audio.load(); } catch (error) {}
        }

        // 사용자 제스처 안에서 무음 재생→정지를 해 두어야, 나중에(게임 오버처럼
        // 제스처가 아닌 시점에) 재생해도 브라우저(특히 iOS)가 막지 않습니다.
        for (const audio of effectAudioCache.values()) {
            try {
                audio.muted = true;
                const p = audio.play();
                const done = () => {
                    try { audio.pause(); audio.currentTime = 0; } catch (error) {}
                    audio.muted = false;
                };
                if (p && typeof p.then === "function") p.then(done).catch(() => { audio.muted = false; });
                else done();
            } catch (error) { audio.muted = false; }
        }
    } catch (error) {}
}

function primeEffectSound(type) {
    const src = AUDIO_FILES[type];
    if (!src || effectVolume <= 0) return;

    try {
        let audio = effectAudioCache.get(type);
        if (!audio) {
            audio = new Audio(src);
            audio.preload = "auto";
            audio.__soundType = type;
            audio.setAttribute("playsinline", "");
            effectAudioCache.set(type, audio);
        }

        audio.volume = getSoundVolume(type);
        audio.muted = true;
        audio.currentTime = 0;

        const promise = audio.play();
        if (promise && typeof promise.then === "function") {
            promise.then(() => {
                audio.pause();
                audio.currentTime = 0;
                audio.muted = false;
                audio.volume = getSoundVolume(type);
            }).catch(() => {
                audio.muted = false;
            });
        } else {
            audio.pause();
            audio.currentTime = 0;
            audio.muted = false;
        }
    } catch (error) {}
}

function playEffectSound(type, oneShotKey = null) {
    const src = AUDIO_FILES[type];
    if (!src || effectVolume <= 0) return null;
    if (oneShotKey && oneShotEffectPlayed.has(oneShotKey)) return null;
    if (oneShotKey) oneShotEffectPlayed.add(oneShotKey);

    try {
        let audio = effectAudioCache.get(type);

        if (!audio) {
            audio = new Audio(src);
            audio.preload = "auto";
            audio.__soundType = type;
            audio.volume = getSoundVolume(type);
            audio.setAttribute("playsinline", "");
            effectAudioCache.set(type, audio);
        }

        audio.muted = false;
        audio.volume = getSoundVolume(type);
        try { audio.currentTime = 0; } catch (error) {}

        const promise = audio.play();
        if (promise && typeof promise.catch === "function") {
            promise.catch(error => {
                console.warn(`[SOUND] ${type} 재생 실패 (${src}):`, error && error.name, error && error.message);
                // 캐시된 오디오가 막혔거나 꼬였을 때: 새 Audio 객체로 한 번 더 시도
                try {
                    const retry = new Audio(src);
                    retry.setAttribute("playsinline", "");
                    retry.volume = getSoundVolume(type);
                    const retryPromise = retry.play();
                    if (retryPromise && typeof retryPromise.then === "function") {
                        retryPromise.then(() => effectAudioCache.set(type, retry)).catch(err2 => {
                            console.warn(`[SOUND] ${type} 재시도 실패:`, err2 && err2.name, err2 && err2.message);
                            if (oneShotKey) oneShotEffectPlayed.delete(oneShotKey);
                        });
                    }
                } catch (error2) {
                    if (oneShotKey) oneShotEffectPlayed.delete(oneShotKey);
                }
            });
        }

        return audio;
    } catch (error) {
        if (oneShotKey) oneShotEffectPlayed.delete(oneShotKey);
        return null;
    }
}

// 첫 터치/클릭/키보드 입력을 실제 사용자 제스처로 받아 오디오 재생 준비를 확보합니다.
document.addEventListener("pointerdown", unlockEffectAudio, { once: true, passive: true });
document.addEventListener("touchstart", unlockEffectAudio, { once: true, passive: true });
document.addEventListener("keydown", unlockEffectAudio, { once: true, passive: true });

function playUIClickSound() {
    return playEffectSound("uiClick");
}

function playUIInvalidSound() {
    return playEffectSound("uiInvalid");
}

// 로딩 화면(팁) → 3초 카운트다운 → 게임 시작
function playGameStartSoundAndThenStart() {
    if (loadingActive || gameState !== "start") return;
    playEffectSound("gameStart");
    runLoadingThen(() => {
        if (gameState === "start") startNewGame();
    }, LOADING_MIN_MS, "게임을 준비하는 중...");
}

/* =========================================================
   아이템 시스템
========================================================= */

const ITEM_PRICES = {
    timeClock: 5,
    energyShield: 15,
    pathGuide: 30,
    firstAid: 20,
    energyRecovery: 10
};

const ITEM_DATA = {
    timeClock: {
        name: "시간 조작 시계",
        icon: "🕒",
        description: "활성화한 개수만큼 제한시간 +1초 (최대 5개 사용 가능)"
    },
    energyShield: {
        name: "에너지 보호막 시스템",
        icon: "🔰",
        description: "위험 블록 충돌 1회 방어 · 2스테이지 마다 복구"
    },
    pathGuide: {
        name: "경로 안내 장치",
        icon: "🧭",
        description: "스테이지 시작 자동 안내 · 재사용은 더블 터치(맵 당 1회 제한)"
    },
   firstAid: {
        name: "응급 처치 장치",
        icon: "💊",
        description: "4스테이지마다 충전 · 목숨이 3개 미만일 시 발동"
    },
    energyRecovery: {
        name: "에너지 복구 장치",
        icon: "🔋",
        description: "맵 넘기기 모두 소모 시 한 번만 작동 · (1개 3회복 / 2개 5회복)"
    }
};

const ITEM_STORAGE_KEY = "slidingMazeItems_v1";

let itemInventory = {
    timeClock: 0,
    energyShield: 0,
    pathGuide: 0,
    firstAid: 0,
    energyRecovery: 0
};

let selectedItem = null;
let selectedTimeClocks = 1;
let selectedEnergyRecovery = 1;
let activeEnergyRecoveryChoice = 1;
let shopOpen = false;
let shopPage = 0;
const SHOP_PAGE_SIZE = 3;
let inventoryOpen = false;
let inventoryDetailType = null;
let skinOpen = false;
const purchaseQuantities = {
    timeClock: 1,
    energyShield: 1,
    pathGuide: 1,
    firstAid: 1,
    energyRecovery: 1
};

let activeItem = null;
let activeTimeBonus = 0;
let shieldCharges = 0;
let firstAidCharged = false;
let pathGuideUses = 0;
let pathGuideVisibleUntil = 0;
let pathGuideFadeStart = 0;
let pathGuideAutoFadeAt = 0;
const PATH_GUIDE_FADE_DURATION = 0.18;
let pathGuidePath = [];
let pathGuideZeroWarningShown = false;
let energyRecoveryUsed = false;
let energyRecoveryChoiceOpen = false;
let itemWarningText = "";
let itemWarningUntil = 0;

function loadItemInventory() {
    try {
        const saved = JSON.parse(
            localStorage.getItem(ITEM_STORAGE_KEY) || "null"
        );

        if (saved) {
            itemInventory = {
                timeClock: Math.max(0, Number(saved.timeClock) || 0),
                energyShield: Math.max(0, Number(saved.energyShield) || 0),
                pathGuide: Math.max(0, Number(saved.pathGuide) || 0),
                firstAid: Math.max(0, Number(saved.firstAid) || 0),
                energyRecovery: Math.max(0, Number(saved.energyRecovery) || 0)
            };
        }
    } catch (error) {}
}

function saveItemInventory() {
    try {
        localStorage.setItem(
            ITEM_STORAGE_KEY,
            JSON.stringify(itemInventory)
        );
    } catch (error) {}
}

loadItemInventory();

let visualSettings = {
    wall: 1,
    background: 0,
    dangerSkin: 1,
    streakEffect: 1,
    playerSkin: 0,
    playerTrail: 0,
    goalSkin: 0,
    customWall: null,
    customBackground: null
};

let settingsOpen = false;


function isValidHexColor(value) {
    return (
        typeof value === "string" &&
        /^#[0-9a-fA-F]{6}$/.test(value.trim())
    );
}

function getWallColor() {
    if (isValidHexColor(visualSettings.customWall)) {
        return visualSettings.customWall;
    }

    const selected = WALL_COLORS[visualSettings.wall];

    if (selected && selected.custom) {
        return WALL_COLORS[WALL_COLORS.length - 2].value;
    }

    return selected?.value || WALL_COLORS[0].value;
}

function getBackgroundColor() {
    if (isValidHexColor(visualSettings.customBackground)) {
        return visualSettings.customBackground;
    }

    const selected = BACKGROUND_COLORS[visualSettings.background];

    if (selected && selected.custom) {
        return BACKGROUND_COLORS[BACKGROUND_COLORS.length - 2].value;
    }

    return selected?.value || BACKGROUND_COLORS[0].value;
}

function setCustomColor(key) {
    const isWall = key === "wall";
    const currentColor = isWall
        ? getWallColor()
        : getBackgroundColor();

    const input = window.prompt(
        isWall
            ? "벽 색상 코드를 입력하세요.\n(예: #3f4b5a)"
            : "배경 색상 코드를 입력하세요.\n(예: #0d1117)",
        currentColor
    );

    if (input === null) {
        return false;
    }

    const color = input.trim();

    if (!isValidHexColor(color)) {
        window.alert(
            "색상 코드는 #RRGGBB 형식으로 입력해주세요.\\n예: #3f4b5a"
        );
        return false;
    }

    if (isWall) {
        visualSettings.customWall = color;
        visualSettings.wall = WALL_COLORS.length - 1;
    } else {
        visualSettings.customBackground = color;
        visualSettings.background = BACKGROUND_COLORS.length - 1;
    }

    saveVisualSettings();
    requestSettingsRender();
    return true;
}

function resetCustomColors() {
    visualSettings.customWall = null;
    visualSettings.customBackground = null;
    saveVisualSettings();
    requestSettingsRender();
}

/* =========================================================
   설정 불러오기
========================================================= */

try {
    const savedVisualSettings =
        JSON.parse(
            localStorage.getItem(SETTINGS_KEY) || "null"
        );

    if (savedVisualSettings) {
        visualSettings = {
            wall:
                Number.isInteger(savedVisualSettings.wall)
                    ? savedVisualSettings.wall
                    : 1,

            background:
                Number.isInteger(savedVisualSettings.background)
                    ? savedVisualSettings.background
                    : 0,

            dangerSkin:
                Number.isInteger(savedVisualSettings.dangerSkin)
                    ? savedVisualSettings.dangerSkin
                    : 1,

            streakEffect:
                Number.isInteger(savedVisualSettings.streakEffect)
                    ? savedVisualSettings.streakEffect
                    : 1,

            playerSkin:
                Number.isInteger(savedVisualSettings.playerSkin)
                    ? savedVisualSettings.playerSkin
                    : 0,

            playerTrail:
                Number.isInteger(savedVisualSettings.playerTrail)
                    ? savedVisualSettings.playerTrail
                    : 0,

            goalSkin:
                Number.isInteger(savedVisualSettings.goalSkin)
                    ? savedVisualSettings.goalSkin
                    : 0,

            customWall:
                isValidHexColor(savedVisualSettings.customWall)
                    ? savedVisualSettings.customWall
                    : null,

            customBackground:
                isValidHexColor(savedVisualSettings.customBackground)
                    ? savedVisualSettings.customBackground
                    : null
        };
    }

} catch (error) {}

if (isValidHexColor(visualSettings.customWall)) {
    visualSettings.wall = WALL_COLORS.length - 1;
}

if (isValidHexColor(visualSettings.customBackground)) {
    visualSettings.background = BACKGROUND_COLORS.length - 1;
}


[["wall", WALL_COLORS], ["background", BACKGROUND_COLORS], ["dangerSkin", DANGER_SKINS], ["streakEffect", STREAK_EFFECTS], ["goalSkin", GOAL_SKINS]].forEach(([k, l]) => {
    if (!(visualSettings[k] >= 0 && visualSettings[k] < l.length)) visualSettings[k] = 0;
});

function saveVisualSettings() {
    localStorage.setItem(
        SETTINGS_KEY,
        JSON.stringify(visualSettings)
    );
}


let visualSettingsSaveTimer = null;

// 설정 화면은 효과 미리보기 때문에 매 프레임 렌더링 비용이 큽니다.
// 색상/효과 변경 직후에는 즉시 한 번 갱신하고, 이후에는 낮은 FPS로만 미리보기를 그립니다.
let settingsRenderRequested = true;
let lastSettingsRenderTime = 0;

function saveMusicVolume() {
    try { localStorage.setItem(MUSIC_VOLUME_KEY, String(musicVolume)); } catch (error) {}
}
function setMusicVolume(value) {
    musicVolume = Math.max(0, Math.min(1, Number(value) || 0));
    if (homeMusic) homeMusic.volume = musicVolume;
    if (backgroundMusic) backgroundMusic.volume = musicVolume;
    if (musicVolume <= 0) {
        if (homeMusic) {
            homeMusic.pause();
            try { homeMusic.currentTime = 0; } catch (error) {}
        }
        if (backgroundMusic) {
            backgroundMusic.pause();
            backgroundMusic.currentTime = 0;
            backgroundMusicPlayRequested = false;
        }
    }
    saveMusicVolume();
    requestSettingsRender();
}

/* =========================================================
   홈 화면 음악: 시작(홈) 화면에서만 반복 재생
   GitHub 저장소의 Home.m4a를 직접 불러옵니다.
========================================================= */
const HOME_MUSIC_URL = "https://raw.githubusercontent.com/JOUMI0822/sliding-game/main/Home.m4a";
let homeMusic = null;
let homeMusicBlocked = false;

function getHomeMusic() {
    if (homeMusic) return homeMusic;
    try {
        homeMusic = new Audio(HOME_MUSIC_URL);
        homeMusic.loop = true;
        homeMusic.preload = "auto";
        homeMusic.volume = musicVolume;
        homeMusic.setAttribute("playsinline", "");
        return homeMusic;
    } catch (error) {
        console.warn("홈 음악을 준비하지 못했습니다.", error);
        return null;
    }
}

function isHomeMusicWanted() {
    const pageIsActive = !document.hidden && (typeof document.hasFocus !== "function" || document.hasFocus());
    return pageIsActive && gameAccessGranted && gameState === "start" && !loadingActive && musicVolume > 0;
}

function startHomeMusic() {
    if (!isHomeMusicWanted() || homeMusicBlocked) return;
    const audio = getHomeMusic();
    if (!audio || !audio.paused) return;
    audio.volume = musicVolume;
    const promise = audio.play();
    if (promise && typeof promise.catch === "function") {
        promise.catch(error => {
            if (error && error.name === "NotAllowedError") homeMusicBlocked = true;
            else console.warn("홈 음악 재생에 실패했습니다.", error);
        });
    }
}

function stopHomeMusic(resetPosition = false) {
    if (!homeMusic) return;
    if (!homeMusic.paused) homeMusic.pause();
    if (resetPosition) {
        try { homeMusic.currentTime = 0; } catch (error) {}
    }
}

function syncHomeMusic() {
    if (isHomeMusicWanted()) {
        startHomeMusic();
    } else {
        // 탭 전환 때는 위치를 유지하고, 홈 화면을 벗어나면 처음으로 되감습니다.
        stopHomeMusic(gameState !== "start" || loadingActive);
    }
}

// 자동 재생이 차단된 경우 첫 사용자 입력 뒤 다시 시도할 수 있게 합니다.
["pointerdown", "keydown", "touchend"].forEach(type => {
    document.addEventListener(type, () => { homeMusicBlocked = false; }, { passive: true });
});

/* =========================================================
   배경음악: 실제 미로 플레이 중에만 반복 재생
   GitHub 저장소의 Last.m4a를 직접 불러옵니다.
========================================================= */
const BACKGROUND_MUSIC_URL = "https://raw.githubusercontent.com/JOUMI0822/sliding-game/main/Last.m4a";
let backgroundMusic = null;
let backgroundMusicPlayRequested = false;
let backgroundMusicWasPlaying = false;

function getBackgroundMusic() {
    if (backgroundMusic) return backgroundMusic;
    try {
        backgroundMusic = new Audio(BACKGROUND_MUSIC_URL);
        backgroundMusic.loop = true;
        backgroundMusic.preload = "auto";
        backgroundMusic.volume = musicVolume;
        backgroundMusic.setAttribute("playsinline", "");
        backgroundMusic.addEventListener("pause", () => {
            if (!isGameplayMusicWanted()) backgroundMusicPlayRequested = false;
        });
        return backgroundMusic;
    } catch (error) {
        console.warn("배경음악을 준비하지 못했습니다.", error);
        return null;
    }
}

function isGameplayMusicWanted() {
    // 실제 플레이 중이고, 사이트 탭/창이 활성화되어 있을 때만 BGM을 재생합니다.
    // 다른 탭으로 이동하거나 브라우저 창에서 벗어나면 재생을 멈춥니다.
    const pageIsActive = !document.hidden && (typeof document.hasFocus !== "function" || document.hasFocus());
    return pageIsActive && gameAccessGranted && !["start", "gameover", "expResult", "multiplayerResult", "tutorial"].includes(gameState) && musicVolume > 0;
}

function startBackgroundMusic() {
    if (!isGameplayMusicWanted()) return;
    const audio = getBackgroundMusic();
    if (!audio || backgroundMusicPlayRequested && !audio.paused) return;
    audio.volume = musicVolume;
    backgroundMusicPlayRequested = true;
    const promise = audio.play();
    if (promise && typeof promise.catch === "function") {
        promise.catch(error => {
            backgroundMusicPlayRequested = false;
            // 브라우저가 자동 재생을 막으면 다음 사용자 입력 때 다시 시도합니다.
            if (error && error.name !== "NotAllowedError") {
                console.warn("배경음악 재생에 실패했습니다.", error);
            }
        });
    }
}

function stopBackgroundMusic(resetPosition = false) {
    if (!backgroundMusic) {
        backgroundMusicPlayRequested = false;
        backgroundMusicWasPlaying = false;
        return;
    }
    if (!backgroundMusic.paused) {
        backgroundMusic.pause();
    }
    // 재생 위치 초기화는 게임 오버 화면에 진입할 때만 수행합니다.
    if (resetPosition) {
        try { backgroundMusic.currentTime = 0; } catch (error) {}
    }
    backgroundMusicPlayRequested = false;
    backgroundMusicWasPlaying = false;
}

function syncBackgroundMusic() {
    // 홈 화면 음악은 시작 화면에서만 재생하고, 게임 음악과 겹치지 않게 관리합니다.
    syncHomeMusic();
    // 홈/시작 화면으로 돌아오면 BGM을 정지하되, 재생 위치는 유지합니다.
    // 재생 위치를 0초로 초기화하는 것은 게임 오버 진입 또는 새 게임 시작 때만 합니다.
    // 2인 대전 승/패/무승부 결과 화면에서는 음악을 끄고 처음 위치로 되돌립니다.
    if (gameState === "multiplayerResult") {
        if (backgroundMusic && (!backgroundMusic.paused || backgroundMusic.currentTime !== 0)) {
            stopBackgroundMusic(true);
        } else {
            backgroundMusicPlayRequested = false;
            backgroundMusicWasPlaying = false;
        }
        return;
    }

    if (gameState === "start" || gameState === "expResult") {
        // 홈 화면과 EXP 결과 화면에서는 음악을 재생하지 않습니다.
        // EXP 화면에서는 재생 위치를 초기화하지 않습니다.
        stopBackgroundMusic(false);
        return;
    }

    // 게임 오버 화면에 진입하면 BGM을 정지하고 재생 위치를 0초로 초기화합니다.
    if (gameAccessGranted && gameState === "gameover") {
        if (backgroundMusic) {
            if (!backgroundMusic.paused || backgroundMusic.currentTime !== 0) {
                stopBackgroundMusic(true);
            } else {
                backgroundMusicPlayRequested = false;
                backgroundMusicWasPlaying = false;
            }
        } else {
            backgroundMusicPlayRequested = false;
            backgroundMusicWasPlaying = false;
        }
        return;
    }

    const wanted = isGameplayMusicWanted();
    if (wanted) {
        const audio = getBackgroundMusic();
        // 플레이 중 상태가 바뀌어도 재생 중인 음악은 건드리지 않습니다.
        // 외부 요인으로 일시 정지된 경우에만 재생을 재개합니다.
        if (audio && audio.paused) {
            startBackgroundMusic();
        } else if (audio && !audio.paused) {
            backgroundMusicWasPlaying = true;
        }
    }
    // 홈/시작 화면으로 이동했다는 이유만으로는 정지하지 않습니다.
}

// 사이트 탭이 숨겨지거나 브라우저 창에서 벗어나면 BGM을 즉시 멈춥니다.
// 다시 사이트로 돌아왔을 때 실제 게임 플레이 중이면 이어서 재생합니다.
function handleBackgroundMusicPageInactive() {
    if (document.hidden || (typeof document.hasFocus === "function" && !document.hasFocus())) {
        stopBackgroundMusic(false);
    }
}

document.addEventListener("visibilitychange", () => {
    if (document.hidden) {
        stopBackgroundMusic(false);
    } else if (isGameplayMusicWanted()) {
        startBackgroundMusic();
    }
});

window.addEventListener("blur", () => {
    stopBackgroundMusic(false);
});

window.addEventListener("focus", () => {
    if (isGameplayMusicWanted()) startBackgroundMusic();
});

// 모바일 브라우저에서 재생 권한이 필요한 경우, 실제 사용자 입력에서 재시도합니다.
document.addEventListener("pointerdown", () => {
    if (isGameplayMusicWanted()) startBackgroundMusic();
}, { passive: true });
document.addEventListener("keydown", () => {
    if (isGameplayMusicWanted()) startBackgroundMusic();
}, { passive: true });

const volumeTouchArea = document.createElement("div");
volumeTouchArea.id = "volumeTouchArea";
Object.assign(volumeTouchArea.style, {
    position: "fixed",
    zIndex: "60",
    display: "none",
    margin: "0",
    padding: "0",
    background: "transparent",
    border: "0",
    outline: "0",
    touchAction: "none",
    userSelect: "none",
    WebkitUserSelect: "none"
});
document.body.appendChild(volumeTouchArea);

let volumeTouchPointerId = null;

function positionVolumeTouchArea() {
    if (!volumeTouchArea || !canvas) return;
    if (!settingsOpen || skinOpen) {
        volumeTouchArea.style.display = "none";
        if (typeof positionMusicVolumeTouchArea === "function") positionMusicVolumeTouchArea();
        return;
    }

    const rect = canvas.getBoundingClientRect();
    const scaleX = rect.width / WIDTH;
    const scaleY = rect.height / HEIGHT;
    const bar = { x: WIDTH / 2 - 130, y: 195, w: 260, h: 8 };

    // A modest touch target around the original thin graphic slider.
    volumeTouchArea.style.display = "block";
    volumeTouchArea.style.left = `${rect.left + (bar.x - 16) * scaleX}px`;
    volumeTouchArea.style.top = `${rect.top + (bar.y - 22) * scaleY}px`;
    volumeTouchArea.style.width = `${(bar.w + 32) * scaleX}px`;
    volumeTouchArea.style.height = `${52 * scaleY}px`;
    if (typeof positionMusicVolumeTouchArea === "function") positionMusicVolumeTouchArea();
}

function setVolumeFromClientX(clientX) {
    const rect = canvas.getBoundingClientRect();
    const bar = { x: WIDTH / 2 - 130, w: 260 };
    const x = (clientX - rect.left) * (WIDTH / rect.width);
    setEffectVolume((x - bar.x) / bar.w);
    requestSettingsRender();
}

volumeTouchArea.addEventListener("pointerdown", event => {
    if (!settingsOpen) return;
    volumeTouchPointerId = event.pointerId;
    try { volumeTouchArea.setPointerCapture(event.pointerId); } catch (error) {}
    setVolumeFromClientX(event.clientX);
    event.preventDefault();
    event.stopPropagation();
}, { passive: false });

volumeTouchArea.addEventListener("pointermove", event => {
    if (volumeTouchPointerId !== event.pointerId) return;
    setVolumeFromClientX(event.clientX);
    event.preventDefault();
    event.stopPropagation();
}, { passive: false });

function endVolumePointer(event) {
    if (volumeTouchPointerId !== event.pointerId) return;
    setVolumeFromClientX(event.clientX);
    try { volumeTouchArea.releasePointerCapture(event.pointerId); } catch (error) {}
    volumeTouchPointerId = null;
    event.preventDefault();
    event.stopPropagation();
}
volumeTouchArea.addEventListener("pointerup", endVolumePointer, { passive: false });
volumeTouchArea.addEventListener("pointercancel", endVolumePointer, { passive: false });

["touchstart","touchmove","touchend","touchcancel"].forEach(type => {
    volumeTouchArea.addEventListener(type, event => {
        event.stopPropagation();
    }, { passive: false });
});

const musicVolumeTouchArea = document.createElement("div");
musicVolumeTouchArea.id = "musicVolumeTouchArea";
Object.assign(musicVolumeTouchArea.style, {
    position: "fixed", zIndex: "60", display: "none", margin: "0", padding: "0",
    background: "transparent", border: "0", outline: "0", touchAction: "none",
    userSelect: "none", WebkitUserSelect: "none"
});
document.body.appendChild(musicVolumeTouchArea);
let musicVolumeTouchPointerId = null;

function positionMusicVolumeTouchArea() {
    if (!musicVolumeTouchArea || !canvas) return;
    if (!settingsOpen || skinOpen) {
        musicVolumeTouchArea.style.display = "none";
        return;
    }
    const rect = canvas.getBoundingClientRect();
    const scaleX = rect.width / WIDTH;
    const scaleY = rect.height / HEIGHT;
    // 음악 슬라이더의 실제 캔버스 위치와 정확히 일치하는 터치 영역
    const bar = { x: WIDTH / 2 - 130, y: 275, w: 260 };
    musicVolumeTouchArea.style.display = "block";
    musicVolumeTouchArea.style.left = `${rect.left + (bar.x - 18) * scaleX}px`;
    musicVolumeTouchArea.style.top = `${rect.top + (bar.y - 24) * scaleY}px`;
    musicVolumeTouchArea.style.width = `${(bar.w + 36) * scaleX}px`;
    musicVolumeTouchArea.style.height = `${56 * scaleY}px`;
}

function setMusicVolumeFromClientX(clientX) {
    const rect = canvas.getBoundingClientRect();
    const bar = { x: WIDTH / 2 - 130, w: 260 };
    const x = (clientX - rect.left) * (WIDTH / rect.width);
    setMusicVolume((x - bar.x) / bar.w);
}

musicVolumeTouchArea.addEventListener("pointerdown", event => {
    if (!settingsOpen || skinOpen) return;
    musicVolumeTouchPointerId = event.pointerId;
    try { musicVolumeTouchArea.setPointerCapture(event.pointerId); } catch (error) {}
    setMusicVolumeFromClientX(event.clientX);
    event.preventDefault();
    event.stopPropagation();
}, { passive: false });

musicVolumeTouchArea.addEventListener("pointermove", event => {
    if (musicVolumeTouchPointerId !== event.pointerId) return;
    setMusicVolumeFromClientX(event.clientX);
    event.preventDefault();
    event.stopPropagation();
}, { passive: false });

function endMusicVolumePointer(event) {
    if (musicVolumeTouchPointerId !== event.pointerId) return;
    setMusicVolumeFromClientX(event.clientX);
    try { musicVolumeTouchArea.releasePointerCapture(event.pointerId); } catch (error) {}
    musicVolumeTouchPointerId = null;
    event.preventDefault();
    event.stopPropagation();
}
musicVolumeTouchArea.addEventListener("pointerup", endMusicVolumePointer, { passive: false });
musicVolumeTouchArea.addEventListener("pointercancel", endMusicVolumePointer, { passive: false });
["touchstart","touchmove","touchend","touchcancel"].forEach(type => {
    musicVolumeTouchArea.addEventListener(type, event => event.stopPropagation(), { passive: false });
});

window.addEventListener("resize", positionVolumeTouchArea);
window.addEventListener("orientationchange", positionVolumeTouchArea);

function requestSettingsRender() {
    settingsRenderRequested = true;
    positionVolumeTouchArea();
}

function saveVisualSettingsDelayed() {
    if (visualSettingsSaveTimer) {
        clearTimeout(visualSettingsSaveTimer);
    }

    visualSettingsSaveTimer = setTimeout(() => {
        saveVisualSettings();
        visualSettingsSaveTimer = null;
    }, 120);
}


function cycleSetting(key, list, direction) {

    let index =
        Number(visualSettings[key]) || 0;

    index =
        (
            index +
            direction +
            list.length
        ) % list.length;

    visualSettings[key] = index;

    // 클릭한 순간 다음 설정 화면 프레임을 강제로 갱신합니다.
    // 저장(localStorage)은 별도로 지연 처리하여 UI를 막지 않습니다.
    requestSettingsRender();

    const selected = list[index];

    if (key === "wall") {
        visualSettings.customWall = null;
    } else if (key === "background") {
        visualSettings.customBackground = null;
    }

    saveVisualSettingsDelayed();
}


/* =========================================================
   게임 데이터
========================================================= */

let lives = MAX_LIVES;

let clearCount = 0;
let clearStreak = 0;
let maxClearStreak = 0;
let allTimeBestStreak = 0;

let coins = 0;

function loadCoins() {
    try {
        coins = Math.max(0, Number(localStorage.getItem("slidingMazeCoins_v1")) || 0);
    } catch (error) {
        coins = 0;
    }
}

function saveCoins() {
    try {
        localStorage.setItem("slidingMazeCoins_v1", String(coins));
    } catch (error) {}
}

loadCoins();


/* =========================================================
   기록
========================================================= */

function getLocalDateKey() {

    const now = new Date();

    const year = now.getFullYear();

    const month =
        String(
            now.getMonth() + 1
        ).padStart(2, "0");

    const day =
        String(
            now.getDate()
        ).padStart(2, "0");

    return `${year}-${month}-${day}`;
}


const DAILY_RECORD_DATE_KEY =
    "slidingMazeDailyRecordDate";

const RECORD_RESET_VERSION =
    "slidingMazeRecordReset_v3";


if (
    !localStorage.getItem(
        RECORD_RESET_VERSION
    )
) {

    localStorage.removeItem(
        "slidingMazeMaxClearCount"
    );

    localStorage.removeItem(
        "slideMazeBestStreak"
    );

    localStorage.removeItem(
        "slideMazeRecentRecords"
    );

    localStorage.removeItem(
        "slidingMazeDailyRecordDate"
    );

    localStorage.setItem(
        RECORD_RESET_VERSION,
        "done"
    );
}


const todayRecordDate =
    getLocalDateKey();

const savedRecordDate =
    localStorage.getItem(
        DAILY_RECORD_DATE_KEY
    );


if (
    savedRecordDate !==
    todayRecordDate
) {

    localStorage.setItem(
        DAILY_RECORD_DATE_KEY,
        todayRecordDate
    );

    localStorage.removeItem(
        "slidingMazeMaxClearCount"
    );

    localStorage.removeItem(
        "slideMazeBestStreak"
    );
}


let maxClearCount =
    Number(
        localStorage.getItem(
            "slidingMazeMaxClearCount"
        ) || 0
    );


let remainingTime = TIME_LIMIT;

let mapSkips = MAX_MAP_SKIPS;


let player = {
    c: stageStart.c,
    r: stageStart.r,
    x: stageStart.c * CELL,
    y: stageStart.r * CELL
};


let goal = null;

let walls = new Set();

let dangers = new Set();

let movement = null;

let trail = [];


let mapTransition = {
    active: false,
    elapsed: 0,
    duration: 0.55,
    oldWalls: new Set(),
    newWalls: new Set()
};


let shake = {
    power: 0,
    time: 0
};


let recoil = {
    x: 0,
    y: 0,
    vx: 0,
    vy: 0,
    damping: 0.82
};


let flash = {
    color: "#fff",
    alpha: 0
};


let messageText = "";

let recentRecords = [];

let previousLayouts = [];

let roundTimer = null;

let recordSavedForRun = false;

let runStartTime = null;

let lastTime = performance.now();


/* =========================================================
   저장 데이터
========================================================= */

try {

    allTimeBestStreak =
        Number(
            localStorage.getItem(
                "slideMazeBestStreak"
            )
        ) || 0;

} catch (error) {

    allTimeBestStreak = 0;
}


try {

    const storedRecords =
        JSON.parse(
            localStorage.getItem(
                "slideMazeRecentRecords"
            )
        );

    if (Array.isArray(storedRecords)) {
        recentRecords =
            storedRecords.slice(0, 5);
    }

} catch (error) {

    recentRecords = [];
}


/* =========================================================
   공통 함수
========================================================= */

function clamp(value, min, max) {
    return Math.max(
        min,
        Math.min(max, value)
    );
}


function keyOf(c, r) {
    return `${c},${r}`;
}


function parseKey(key) {

    const [
        c,
        r
    ] =
        key
            .split(",")
            .map(Number);

    return {
        c,
        r
    };
}


function isInside(c, r) {
    return (
        c >= 0 &&
        c < COLS &&
        r >= 0 &&
        r < ROWS
    );
}


function isBoundary(c, r) {
    return (
        c === 0 ||
        r === 0 ||
        c === COLS - 1 ||
        r === ROWS - 1
    );
}


function randomInt(min, max) {
    return Math.floor(
        Math.random() *
        (max - min + 1)
    ) + min;
}


function setMessage(text) {
    messageText = text;
}

function showItemWarning(text) {
    itemWarningText = text;
    itemWarningUntil = performance.now() + 2600;
}

function getSelectedItemLabel() {
    if (!selectedItem) {
        return "아이템 없음";
    }

    const data = ITEM_DATA[selectedItem];

    if (selectedItem === "timeClock") {
        return `${data.icon} ${data.name} × ${selectedTimeClocks}`;
    }

    if (selectedItem === "pathGuide" || selectedItem === "energyRecovery") {
        return `${data.icon} ${data.name} · 보유 ${itemInventory[selectedItem]}`;
    }

    return `${data.icon} ${data.name}`;
}

function consumeEquippedItem(type, amount = 1) {
    if (!type || !Object.prototype.hasOwnProperty.call(itemInventory, type)) {
        return false;
    }

    const current = Math.max(0, Number(itemInventory[type]) || 0);
    const consumeAmount = Math.max(1, Math.floor(Number(amount) || 1));

    if (current < consumeAmount) {
        return false;
    }

    itemInventory[type] = current - consumeAmount;

    // 인벤토리가 0개가 되면 장착 상태도 즉시 해제합니다.
    // 단, 현재 실행 중인 activeItem은 이번 게임에 이미 투입된 아이템이므로
    // activeItem 자체는 유지합니다. selectedItem만 해제합니다.
    if (itemInventory[type] <= 0) {
        itemInventory[type] = 0;
        if (selectedItem === type) {
            selectedItem = null;
        }
    }

    saveItemInventory();
    updateUI();
    return true;
}

function activateItemForRun() {
    // 2인용 경쟁에서는 아이템 효과와 소모를 모두 비활성화합니다.
    // 방장/참가자 모두 동일하게 적용하여 아이템으로 제한시간이나 맵 표시가 달라지지 않게 합니다.
    if (multiplayerMatchActive) {
        activeItem = null;
        activeTimeBonus = 0;
        activeEnergyRecoveryChoice = 1;
        shieldCharges = 0;
        firstAidCharged = false;
        pathGuideUses = 0;
        pathGuidePath = [];
        return;
    }
    /*
       아이템 소비 규칙
       - 시간 조작 시계: 선택한 개수만큼 게임 시작 시 즉시 소비
       - 에너지 보호막: 게임 시작 시 1개 소비
       - 경로 안내 장치: 게임 시작 시 1개 소비
         → 같은 맵에서 더블 터치 재사용은 별도 아이템 1개를 추가 소비하는 것이 아니라,
           '시작 시 투입된 1개'의 재사용 횟수입니다.
         → 따라서 시작 소비 후 인벤토리가 0이면 재사용할 수 없습니다.
       - 응급 처치 장치: 게임 시작 시 1개 소비
       - 에너지 복구 장치: 게임 시작 시 소비하지 않음. 실제 복구 사용 시에만 소비
    */
    activeItem = selectedItem;

    activeTimeBonus = 0;
    activeEnergyRecoveryChoice = 1;

    if (activeItem === "timeClock") {
        const available = Math.max(0, Number(itemInventory.timeClock) || 0);
        selectedTimeClocks = Math.max(
            0,
            Math.min(5, Number(selectedTimeClocks) || 0, available)
        );

        if (selectedTimeClocks <= 0) {
            activeItem = null;
            selectedItem = null;
            selectedTimeClocks = 1;
        } else if (!consumeEquippedItem("timeClock", selectedTimeClocks)) {
            activeItem = null;
            selectedItem = null;
            selectedTimeClocks = 1;
        } else {
            activeTimeBonus = selectedTimeClocks;
        }
    } else if (activeItem === "energyShield") {
        if (!consumeEquippedItem("energyShield", 1)) {
            activeItem = null;
            selectedItem = null;
        }
    } else if (activeItem === "pathGuide") {
        if (!consumeEquippedItem("pathGuide", 1)) {
            activeItem = null;
            selectedItem = null;
        }
    } else if (activeItem === "firstAid") {
        if (!consumeEquippedItem("firstAid", 1)) {
            activeItem = null;
            selectedItem = null;
        }
    } else if (activeItem === "energyRecovery") {
        // 에너지 복구 장치는 실제 복구를 누를 때만 소비합니다.
        selectedEnergyRecovery = Math.max(
            1,
            Math.min(2, Number(selectedEnergyRecovery) || 1)
        );

        if (itemInventory.energyRecovery <= 0) {
            activeItem = null;
            selectedItem = null;
        } else {
            selectedEnergyRecovery = Math.min(
                selectedEnergyRecovery,
                itemInventory.energyRecovery
            );
            activeEnergyRecoveryChoice = selectedEnergyRecovery;
        }
    } else {
        activeItem = null;
    }

    if (activeItem) {
        playEffectSound("itemUse");
    }

    shieldCharges = 0;
    firstAidCharged = false;
    pathGuideUses = 0;
    pathGuideVisibleUntil = 0;
    pathGuideFadeStart = 0;
    pathGuideAutoFadeAt = 0;
    pathGuidePath = [];
    pathGuideZeroWarningShown = false;
    energyRecoveryUsed = false;
    energyRecoveryChoiceOpen = false;
    itemWarningText = "";
    itemWarningUntil = 0;
}

function deactivateItemForRun() {
    activeItem = null;
    activeTimeBonus = 0;
    shieldCharges = 0;
    firstAidCharged = false;
    pathGuideUses = 0;
    pathGuideVisibleUntil = 0;
    pathGuideFadeStart = 0;
    pathGuideAutoFadeAt = 0;
    pathGuidePath = [];
    pathGuideZeroWarningShown = false;
    energyRecoveryUsed = false;
    energyRecoveryChoiceOpen = false;
    itemWarningText = "";
    itemWarningUntil = 0;
}

function openEnergyRecoveryChoice() {
    if (
        activeItem !== "energyRecovery" ||
        energyRecoveryUsed ||
        energyRecoveryChoiceOpen ||
        mapSkips > 0 ||
        itemInventory.energyRecovery <= 0
    ) {
        return false;
    }

    energyRecoveryChoiceOpen = true;
    return true;
}

function useEnergyRecovery(amount) {
    if (
        activeItem !== "energyRecovery" ||
        energyRecoveryUsed ||
        !energyRecoveryChoiceOpen ||
        mapSkips > 0
    ) {
        return false;
    }

    amount = Math.max(1, Math.min(2, amount));

    if (itemInventory.energyRecovery < amount) {
        return false;
    }

    const recovered = amount === 1 ? 3 : 5;

    itemInventory.energyRecovery -= amount;
    if (itemInventory.energyRecovery <= 0) {
        itemInventory.energyRecovery = 0;
        if (selectedItem === "energyRecovery") {
            selectedItem = null;
        }
    }
    mapSkips = Math.min(MAX_MAP_SKIPS, recovered);
    energyRecoveryUsed = true;
    onDailyQuestEnergyRecoveryUse();
    energyRecoveryChoiceOpen = false;

    saveItemInventory();
    showItemWarning(`에너지 복구 장치 ${amount}개 사용 · 맵 넘기기 ${mapSkips}개 회복`);
    updateUI();
    return true;
}

function getMaxAffordableQuantity(type) {
    const price = ITEM_PRICES[type];
    if (!price || coins < price) return 0;
    return Math.floor(coins / price);
}

function getPurchaseQuantity(type) {
    const max = getMaxAffordableQuantity(type);
    if (max <= 0) return 0;
    purchaseQuantities[type] = Math.max(1, Math.min(max, purchaseQuantities[type] || 1));
    return purchaseQuantities[type];
}

function adjustPurchaseQuantity(type, direction) {
    const max = getMaxAffordableQuantity(type);
    if (max <= 0) {
        purchaseQuantities[type] = 0;
        return;
    }
    purchaseQuantities[type] = Math.max(1, Math.min(max, (purchaseQuantities[type] || 1) + direction));
}

function buyItem(type) {
    const price = ITEM_PRICES[type];
    const quantity = getPurchaseQuantity(type);
    if (!quantity || coins < price * quantity) {
        showItemWarning("재화가 부족합니다.");
        playUIInvalidSound();
        return;
    }

    const totalCost = price * quantity;
    coins -= totalCost;
    itemInventory[type] += quantity;
    saveItemInventory();
    saveCoins();

    if (type === "timeClock" && !selectedItem) {
        selectedTimeClocks = Math.min(5, Math.max(1, itemInventory.timeClock));
    }

    showItemWarning(`${ITEM_DATA[type].name} ${quantity}개 구매 완료 · ${coins}코인 남음`);
    purchaseQuantities[type] = Math.min(purchaseQuantities[type], Math.max(1, getMaxAffordableQuantity(type) || 1));
}

// 상점 구매: 잘못 누르는 것을 막기 위해 최종 확인창을 거칩니다.
async function requestBuyItem(type) {
    if (logoutConfirmOpen) return;

    const price = ITEM_PRICES[type];
    const quantity = getPurchaseQuantity(type);
    if (!quantity || coins < price * quantity) {
        showItemWarning("재화가 부족합니다.");
        playUIInvalidSound();
        return;
    }

    const total = price * quantity;
    const ok = await openLogoutConfirm({
        title: "구매 확인",
        message: `${ITEM_DATA[type].icon} ${ITEM_DATA[type].name} ${quantity}개를\n🪙 ${total}코인에 구매할까요?\n(구매 후 ${coins - total}코인 남음)`,
        confirmLabel: "구매",
        danger: false
    });

    if (!ok || !shopOpen) return;
    buyItem(type);
}

function equipItem(type) {
    if (itemInventory[type] <= 0) {
        showItemWarning("해당 아이템이 없습니다.");
        playUIInvalidSound();
        return;
    }

    if (selectedItem === type) {
        selectedItem = null;
        return;
    }

    selectedItem = type;
    if (type === "timeClock") {
        selectedTimeClocks = Math.max(1, Math.min(5, itemInventory.timeClock));
    }
    if (type === "energyRecovery") {
        selectedEnergyRecovery =
            Math.max(1, Math.min(2, itemInventory.energyRecovery));
    }
}

function unequipItem() {
    selectedItem = null;
}

function adjustSelectedTimeClocks(direction) {
    if (itemInventory.timeClock <= 0) return;
    selectedTimeClocks = Math.max(1, Math.min(5, selectedTimeClocks + direction));
    selectedItem = "timeClock";
}

function adjustSelectedEnergyRecovery(direction) {
    if (itemInventory.energyRecovery <= 0) return;
    selectedEnergyRecovery = Math.max(1, Math.min(2, selectedEnergyRecovery + direction));
    selectedEnergyRecovery = Math.min(selectedEnergyRecovery, itemInventory.energyRecovery);
    selectedItem = "energyRecovery";
}

function openInventoryDetail(type) {
    inventoryDetailType = type;
    inventoryOpen = true;
}

function closeInventoryDetail() {
    inventoryDetailType = null;
}

function getGuidePath() {
    if (!goal) {
        return [];
    }

    const graph = buildSlideGraph(walls);
    const startKey = keyOf(player.c, player.r);
    const goalKey = keyOf(goal.c, goal.r);

    const queue = [startKey];
    const previous = new Map([[startKey, null]]);

    while (queue.length) {
        const current = queue.shift();
        if (current === goalKey) break;

        for (const next of graph.get(current) || []) {
            if (dangers.has(next) || previous.has(next)) continue;
            previous.set(next, current);
            queue.push(next);
        }
    }

    if (!previous.has(goalKey)) {
        return [];
    }

    const result = [];
    let current = goalKey;

    while (current !== null) {
        result.push(parseKey(current));
        current = previous.get(current);
    }

    return result.reverse();
}

function showPathGuide() {
    if (gameState !== "playing" && gameState !== "transition") {
        return false;
    }

    pathGuidePath = getGuidePath();
    if (!pathGuidePath.length) {
        return false;
    }

    const guideNow = performance.now();
    pathGuideVisibleUntil = guideNow + 1500;
    pathGuideFadeStart = 0;
    pathGuideAutoFadeAt = guideNow + 1320;
    return true;
}

function useSecondPathGuide() {
    if (activeItem !== "pathGuide") {
        return false;
    }

    if (pathGuideUses >= 2) {
        return false;
    }

    if (pathGuideUses === 0) {
        return false;
    }

    if (itemInventory.pathGuide <= 0) {
        if (!pathGuideZeroWarningShown) {
            pathGuideZeroWarningShown = true;
            showItemWarning("경로 안내 장치 보유량 0");
        }
        return false;
    }

    if (showPathGuide()) {
        // 경로 안내 장치는 게임 시작 시 1개를 이미 소비했습니다.
        // 따라서 같은 게임에서의 두 번째 안내에는 인벤토리에서 다시 차감하지 않습니다.
        pathGuideUses = 2;
        playEffectSound("itemUse");
        return true;
    }

    return false;
}

function tryAutoFirstAid() {
    if (activeItem !== "firstAid" || !firstAidCharged || lives >= MAX_LIVES) {
        return false;
    }

    lives = Math.min(MAX_LIVES, lives + 1);
    firstAidCharged = false;
    playEffectSound("itemUse");
    showItemWarning("응급 처치 장치 발동 · 목숨 +1");
    updateUI();
    return true;
}


/* =========================================================
   반동 / 흔들림
========================================================= */

function applyRecoil(
    dirX,
    dirY,
    strength,
    shakePower,
    duration
) {

    recoil.vx =
        -dirX * strength;

    recoil.vy =
        -dirY * strength;

    shake.power =
        Math.max(
            shake.power,
            shakePower
        );

    shake.time =
        Math.max(
            shake.time,
            duration
        );
}


function applyImpactRecoil(
    strength,
    shakePower,
    duration
) {

    const angle =
        Math.random() *
        Math.PI * 2;

    recoil.vx =
        Math.cos(angle) *
        strength;

    recoil.vy =
        Math.sin(angle) *
        strength;

    shake.power =
        Math.max(
            shake.power,
            shakePower
        );

    shake.time =
        Math.max(
            shake.time,
            duration
        );
}


function updateRecoil(delta) {

    recoil.x +=
        recoil.vx *
        delta;

    recoil.y +=
        recoil.vy *
        delta;

    const damping =
        Math.pow(
            recoil.damping,
            delta * 60
        );

    recoil.vx *= damping;
    recoil.vy *= damping;

    recoil.vx +=
        -recoil.x *
        0.55 *
        delta *
        60;

    recoil.vy +=
        -recoil.y *
        0.55 *
        delta *
        60;

    recoil.x =
        clamp(
            recoil.x,
            -18,
            18
        );

    recoil.y =
        clamp(
            recoil.y,
            -18,
            18
        );
}


function resetRecoil() {

    recoil.x = 0;
    recoil.y = 0;
    recoil.vx = 0;
    recoil.vy = 0;
}


function getShakeOffset() {

    if (shake.time <= 0) {
        return {
            x: 0,
            y: 0
        };
    }

    const amount =
        shake.power *
        Math.min(
            1,
            shake.time / 0.2
        );

    return {
        x:
            (Math.random() * 2 - 1) *
            amount,

        y:
            (Math.random() * 2 - 1) *
            amount
    };
}


/* =========================================================
   벽 생성
========================================================= */

function createBoundaryWalls() {

    const result =
        new Set();

    for (
        let r = 0;
        r < ROWS;
        r++
    ) {

        for (
            let c = 0;
            c < COLS;
            c++
        ) {

            if (
                isBoundary(c, r)
            ) {
                result.add(
                    keyOf(c, r)
                );
            }
        }
    }

    return result;
}


function canPlaceRectangle(
    wallSet,
    x,
    y,
    w,
    h
) {

    const protectedCells = [
        [
            stageStart.c,
            stageStart.r
        ],

        [
            stageStart.c + 1,
            stageStart.r
        ],

        [
            stageStart.c,
            stageStart.r + 1
        ]
    ];

    for (
        let r = y;
        r < y + h;
        r++
    ) {

        for (
            let c = x;
            c < x + w;
            c++
        ) {

            if (
                !isInside(c, r)
            ) {
                return false;
            }

            if (
                isBoundary(c, r)
            ) {
                return false;
            }

            if (
                protectedCells.some(
                    ([pc, pr]) =>
                        pc === c &&
                        pr === r
                )
            ) {
                return false;
            }

            if (
                wallSet.has(
                    keyOf(c, r)
                )
            ) {
                return false;
            }
        }
    }

    return true;
}


function isWalkableAreaFullyConnected(wallSet) {

    const startKey =
        keyOf(
            stageStart.c,
            stageStart.r
        );

    if (wallSet.has(startKey)) {
        return false;
    }

    const visited =
        new Set([startKey]);

    const queue = [startKey];

    while (
        queue.length > 0
    ) {

        const current =
            queue.shift();

        const { c, r } =
            parseKey(current);

        const neighbors = [
            [c + 1, r],
            [c - 1, r],
            [c, r + 1],
            [c, r - 1]
        ];

        for (
            const [nc, nr] of neighbors
        ) {

            if (
                nc <= 0 ||
                nr <= 0 ||
                nc >= COLS - 1 ||
                nr >= ROWS - 1
            ) {
                continue;
            }

            const nextKey =
                keyOf(nc, nr);

            if (
                wallSet.has(nextKey) ||
                visited.has(nextKey)
            ) {
                continue;
            }

            visited.add(nextKey);
            queue.push(nextKey);
        }
    }

    const totalOpenCells =
        (COLS - 2) *
        (ROWS - 2) -
        [...wallSet].filter(key => {
            const { c, r } = parseKey(key);
            return !isBoundary(c, r);
        }).length;

    return visited.size === totalOpenCells;
}


function createRandomWalls() {

    // 맵 구조는 클리어 횟수와 무관하게 일정한 범위에서 생성합니다.
    // 난이도 상승은 기존의 제한시간 시스템만 담당합니다.
    const minRectangles = 20;
    const maxRectangles = 31;
    const maxDensity = 0.40;

    const result =
        createBoundaryWalls();

    const rectangleCount =
        randomInt(
            minRectangles,
            maxRectangles
        );

    for (
        let attempt = 0;
        attempt < rectangleCount * 15;
        attempt++
    ) {

        if (
            result.size >
            COLS * ROWS * maxDensity
        ) {
            break;
        }

        const w =
            randomInt(1, 4);

        const h =
            randomInt(1, 3);

        const x =
            randomInt(
                1,
                COLS - w - 2
            );

        const y =
            randomInt(
                1,
                ROWS - h - 2
            );

        if (
            canPlaceRectangle(
                result,
                x,
                y,
                w,
                h
            )
        ) {

            for (
                let r = y;
                r < y + h;
                r++
            ) {

                for (
                    let c = x;
                    c < x + w;
                    c++
                ) {

                    result.add(
                        keyOf(c, r)
                    );
                }
            }
        }
    }

    // 벽으로 둘러싸여 의미 없이 갇힌 빈 공간이 생기지 않도록
    // 모든 내부 빈 칸이 하나의 연결된 영역인지 확인합니다.
    if (
        !isWalkableAreaFullyConnected(result)
    ) {
        return null;
    }

    return result;
}


/* =========================================================
   슬라이딩 이동 계산
========================================================= */

function getSlideDestination(
    c,
    r,
    dc,
    dr,
    wallSet = walls
) {

    let nc = c;
    let nr = r;

    while (true) {

        const nextC =
            nc + dc;

        const nextR =
            nr + dr;

        if (
            !isInside(
                nextC,
                nextR
            ) ||
            wallSet.has(
                keyOf(
                    nextC,
                    nextR
                )
            )
        ) {
            break;
        }

        nc = nextC;
        nr = nextR;
    }

    return {
        c: nc,
        r: nr
    };
}


function getSlideMoves(
    c,
    r,
    wallSet = walls
) {

    const directions = [
        {
            dc: 0,
            dr: -1
        },
        {
            dc: 0,
            dr: 1
        },
        {
            dc: -1,
            dr: 0
        },
        {
            dc: 1,
            dr: 0
        }
    ];

    const result = [];

    for (
        const direction
        of directions
    ) {

        const destination =
            getSlideDestination(
                c,
                r,
                direction.dc,
                direction.dr,
                wallSet
            );

        if (
            destination.c !== c ||
            destination.r !== r
        ) {

            result.push({
                from: {
                    c,
                    r
                },

                to: destination,

                dc: direction.dc,
                dr: direction.dr
            });
        }
    }

    return result;
}


/* =========================================================
   슬라이딩 그래프
========================================================= */

function buildSlideGraph(
    wallSet = walls
) {

    const graph =
        new Map();

    for (
        let r = 1;
        r < ROWS - 1;
        r++
    ) {

        for (
            let c = 1;
            c < COLS - 1;
            c++
        ) {

            const current =
                keyOf(c, r);

            if (
                wallSet.has(current)
            ) {
                continue;
            }

            const moves =
                getSlideMoves(
                    c,
                    r,
                    wallSet
                );

            graph.set(
                current,
                moves.map(
                    move =>
                        keyOf(
                            move.to.c,
                            move.to.r
                        )
                )
            );
        }
    }

    return graph;
}


function getReachableStates(
    graph,
    startKey
) {

    const visited =
        new Set();

    const queue = [
        startKey
    ];

    visited.add(startKey);

    while (
        queue.length > 0
    ) {

        const current =
            queue.shift();

        const neighbors =
            graph.get(current) || [];

        for (
            const next
            of neighbors
        ) {

            if (
                visited.has(next)
            ) {
                continue;
            }

            visited.add(next);
            queue.push(next);
        }
    }

    return visited;
}


function buildReverseGraph(
    graph
) {

    const reverse =
        new Map();

    for (
        const [
            from,
            destinations
        ]
        of graph.entries()
    ) {

        if (
            !reverse.has(from)
        ) {
            reverse.set(
                from,
                []
            );
        }

        for (
            const destination
            of destinations
        ) {

            if (
                !reverse.has(
                    destination
                )
            ) {

                reverse.set(
                    destination,
                    []
                );
            }

            reverse
                .get(destination)
                .push(from);
        }
    }

    return reverse;
}


function getStatesThatCanReachGoal(
    graph,
    goalKey
) {

    const reverse =
        buildReverseGraph(
            graph
        );

    const visited =
        new Set();

    const queue = [
        goalKey
    ];

    visited.add(goalKey);

    while (
        queue.length > 0
    ) {

        const current =
            queue.shift();

        const previousStates =
            reverse.get(current) || [];

        for (
            const previous
            of previousStates
        ) {

            if (
                visited.has(previous)
            ) {
                continue;
            }

            visited.add(previous);
            queue.push(previous);
        }
    }

    return visited;
}


function isMapFullyEscapable(
    graph,
    goalKey
) {

    const startKey =
        keyOf(
            stageStart.c,
            stageStart.r
        );

    const reachable =
        getReachableStates(
            graph,
            startKey
        );

    const canReachGoal =
        getStatesThatCanReachGoal(
            graph,
            goalKey
        );

    if (
        !canReachGoal.has(
            startKey
        )
    ) {

        return {
            valid: false,
            reason:
                "시작점에서 목표로 갈 수 없음"
        };
    }

    for (
        const state
        of reachable
    ) {

        if (
            !canReachGoal.has(
                state
            )
        ) {

            return {
                valid: false,
                reason:
                    `탈출 불가능 상태: ${state}`
            };
        }
    }

    return {
        valid: true,
        reachableCount:
            reachable.size
    };
}


/* =========================================================
   경로 탐색
========================================================= */

function getPathTo(
    graph,
    startKey,
    goalKey
) {

    const queue = [
        startKey
    ];

    const previous =
        new Map();

    previous.set(
        startKey,
        null
    );

    while (
        queue.length > 0
    ) {

        const current =
            queue.shift();

        if (
            current === goalKey
        ) {
            break;
        }

        const neighbors =
            graph.get(current) || [];

        for (
            const next
            of neighbors
        ) {

            if (
                previous.has(next)
            ) {
                continue;
            }

            previous.set(
                next,
                current
            );

            queue.push(next);
        }
    }

    if (
        !previous.has(
            goalKey
        )
    ) {
        return null;
    }

    const path = [];

    let current =
        goalKey;

    while (
        current !== null
    ) {

        path.push(current);

        current =
            previous.get(
                current
            );
    }

    path.reverse();

    return path;
}


/* =========================================================
   맵 분석
========================================================= */

function analyzeMap(
    graph,
    startKey
) {

    const reachable =
        getReachableStates(
            graph,
            startKey
        );

    let branchingStates = 0;
    let deadEndStates = 0;
    let maxDegree = 0;

    for (
        const state
        of reachable
    ) {

        const degree =
            (
                graph.get(state) ||
                []
            ).length;

        maxDegree =
            Math.max(
                maxDegree,
                degree
            );

        if (
            degree >= 2
        ) {
            branchingStates++;
        }

        if (
            degree === 0
        ) {
            deadEndStates++;
        }
    }

    return {
        reachable,
        reachableCount:
            reachable.size,
        branchingStates,
        deadEndStates,
        maxDegree
    };
}


/* =========================================================
   목표 후보
========================================================= */

function getGoalCandidates(
    graph,
    reachable,
    startKey
) {

    const candidates = [];

    for (
        const state
        of reachable
    ) {

        if (
            state === startKey
        ) {
            continue;
        }

        const path =
            getPathTo(
                graph,
                startKey,
                state
            );

        if (!path) {
            continue;
        }

        if (
            path.length - 1 >=
            MIN_PATH_LENGTH
        ) {

            candidates.push({
                key: state,
                pathLength:
                    path.length - 1
            });
        }
    }

    candidates.sort(
        (a, b) =>
            b.pathLength -
            a.pathLength
    );

    return candidates;
}


/* =========================================================
   위험 블록 생성
========================================================= */

function createDanger(
    graph,
    goalKey,
    safePath
) {

    const result =
        new Set();

    const safePathSet =
        new Set(
            safePath
        );

    const candidates = [];

    for (
        const state
        of graph.keys()
    ) {

        if (
            state ===
            keyOf(
                stageStart.c,
                stageStart.r
            )
        ) {
            continue;
        }

        if (
            state === goalKey
        ) {
            continue;
        }

        if (
            safePathSet.has(
                state
            )
        ) {
            continue;
        }

        candidates.push(state);
    }

    // 위험 블록은 항상 5~10개 범위에서만 생성합니다.
    const dangerCount =
        randomInt(5, 10);

    for (
        let i = 0;
        i < dangerCount &&
        candidates.length > 0;
        i++
    ) {

        const index =
            randomInt(
                0,
                candidates.length - 1
            );

        const chosen =
            candidates.splice(
                index,
                1
            )[0];

        result.add(chosen);
    }

    return result;
}


function verifySafeGoalPath(
    graph,
    goalKey,
    dangers
) {

    const startKey =
        keyOf(
            stageStart.c,
            stageStart.r
        );

    const queue = [
        startKey
    ];

    const visited =
        new Set();

    visited.add(
        startKey
    );

    while (
        queue.length > 0
    ) {

        const current =
            queue.shift();

        if (
            current === goalKey
        ) {
            return true;
        }

        const neighbors =
            graph.get(current) || [];

        for (
            const next
            of neighbors
        ) {

            if (
                dangers.has(next)
            ) {
                continue;
            }

            if (
                visited.has(next)
            ) {
                continue;
            }

            visited.add(next);
            queue.push(next);
        }
    }

    return false;
}


/* =========================================================
   맵 서명
========================================================= */

function getLayoutSignature(
    wallSet,
    goalKey,
    dangerSet
) {

    const wallsPart =
        [...wallSet]
            .sort()
            .join("|");

    const dangersPart =
        [...dangerSet]
            .sort()
            .join("|");

    return (
        wallsPart +
        "::" +
        goalKey +
        "::" +
        dangersPart
    );
}


/* =========================================================
   맵 생성
========================================================= */

function createMap() {

    const oldWallSnapshot =
        new Set(walls);

    let repeatedMapCandidate = null;

    for (
        let attempt = 0;
        attempt < MAX_MAP_ATTEMPTS;
        attempt++
    ) {

        const candidateWalls =
            createRandomWalls();

        // 연결되지 않은 빈 공간이 만들어진 맵은 즉시 폐기합니다.
        if (!candidateWalls) {
            continue;
        }

        const graph =
            buildSlideGraph(
                candidateWalls
            );

        const startKey =
            keyOf(
                stageStart.c,
                stageStart.r
            );

        const analysis =
            analyzeMap(
                graph,
                startKey
            );

        // 맵 구조 조건은 고정합니다.
        if (
            analysis.reachableCount <
            MIN_REACHABLE_STATES
        ) {
            continue;
        }

        if (
            analysis.branchingStates <
            MIN_BRANCHING_STATES
        ) {
            continue;
        }

        const candidates =
            getGoalCandidates(
                graph,
                analysis.reachable,
                startKey
            );

        if (
            candidates.length === 0
        ) {
            continue;
        }

        const candidatePool =
            candidates.slice(
                0,
                Math.min(
                    8,
                    candidates.length
                )
            );

        const goalCandidate =
            candidatePool[
                randomInt(
                    0,
                    candidatePool.length - 1
                )
            ];

        const goalKey =
            goalCandidate.key;

        const escapeCheck =
            isMapFullyEscapable(
                graph,
                goalKey
            );

        if (!escapeCheck.valid) {
            continue;
        }

        const safePath =
            getPathTo(
                graph,
                startKey,
                goalKey
            );

        if (
            !safePath ||
            safePath.length - 1 <
            MIN_PATH_LENGTH
        ) {
            continue;
        }

        const candidateDangers =
            createDanger(
                graph,
                goalKey,
                safePath
            );

        // 위험 블록은 최소 5개가 실제로 배치된 맵만 사용합니다.
        if (
            candidateDangers.size < 5
        ) {
            continue;
        }

        if (
            !verifySafeGoalPath(
                graph,
                goalKey,
                candidateDangers
            )
        ) {
            continue;
        }

        const signature =
            getLayoutSignature(
                candidateWalls,
                goalKey,
                candidateDangers
            );

        if (
            !multiplayerMatchActive &&
            previousLayouts.includes(
                signature
            )
        ) {
            if (!repeatedMapCandidate) {
                repeatedMapCandidate = {
                    walls: new Set(candidateWalls),
                    goalKey,
                    dangers: new Set(candidateDangers),
                    signature
                };
            }
            continue;
        }

        walls =
            candidateWalls;

        beginMapTransition(
            oldWallSnapshot,
            candidateWalls
        );

        goal =
            parseKey(
                goalKey
            );

        dangers =
            candidateDangers;

        previousLayouts.push(
            signature
        );

        if (
            previousLayouts.length >
            MAX_PREVIOUS_LAYOUTS
        ) {
            previousLayouts.shift();
        }

        return true;
    }

    if (repeatedMapCandidate) {
        walls =
            repeatedMapCandidate.walls;

        beginMapTransition(
            oldWallSnapshot,
            repeatedMapCandidate.walls
        );

        goal =
            parseKey(
                repeatedMapCandidate.goalKey
            );

        dangers =
            repeatedMapCandidate.dangers;

        return true;
    }

    return createFallbackMap(
        oldWallSnapshot
    );
}

// 멀티플레이에서는 각 클라이언트가 같은 시드로 맵을 직접 생성합니다.
// createMap 내부의 기존 난수 기반 생성 로직을 그대로 사용하되, 생성 중에만
// Math.random을 시드 기반 난수로 바꿔 양쪽 맵이 동일하게 나오도록 합니다.
function createMapWithSeed(seed) {
    const originalRandom = Math.random;
    let state = (Number(seed) >>> 0) || 1;
    Math.random = function seededRandom() {
        state = (Math.imul(state, 1664525) + 1013904223) >>> 0;
        return state / 4294967296;
    };
    try {
        return createMap();
    } finally {
        Math.random = originalRandom;
    }
}


/* =========================================================
   fallback 맵
========================================================= */

function createFallbackMap(
    oldWallSnapshot = new Set(walls)
) {

    const fallbackWalls =
        createBoundaryWalls();

    const addWall = (
        c,
        r
    ) => {

        if (
            !isBoundary(c, r) &&
            !(
                c === stageStart.c &&
                r === stageStart.r
            )
        ) {
            fallbackWalls.add(
                keyOf(c, r)
            );
        }
    };

    for (
        let r = 2;
        r <= 5;
        r++
    ) {
        addWall(5, r);
    }

    for (
        let r = 8;
        r <= 12;
        r++
    ) {
        addWall(10, r);
    }

    for (
        let r = 2;
        r <= 6;
        r++
    ) {
        addWall(14, r);
    }

    for (
        let c = 7;
        c <= 10;
        c++
    ) {
        addWall(c, 5);
    }

    for (
        let c = 12;
        c <= 16;
        c++
    ) {
        addWall(c, 9);
    }

    const graph =
        buildSlideGraph(
            fallbackWalls
        );

    const startKey =
        keyOf(
            stageStart.c,
            stageStart.r
        );

    const reachable =
        getReachableStates(
            graph,
            startKey
        );

    const candidates =
        getGoalCandidates(
            graph,
            reachable,
            startKey
        );

    for (
        const candidate
        of candidates
    ) {

        const escapeCheck =
            isMapFullyEscapable(
                graph,
                candidate.key
            );

        if (
            !escapeCheck.valid
        ) {
            continue;
        }

        const safePath =
            getPathTo(
                graph,
                startKey,
                candidate.key
            );

        if (!safePath) {
            continue;
        }

        const fallbackDangers =
            createDanger(
                graph,
                candidate.key,
                safePath
            );

        if (
            !verifySafeGoalPath(
                graph,
                candidate.key,
                fallbackDangers
            )
        ) {
            continue;
        }

        walls =
            fallbackWalls;

        beginMapTransition(
            oldWallSnapshot,
            fallbackWalls
        );

        goal =
            parseKey(
                candidate.key
            );

        dangers =
            fallbackDangers;

        return true;
    }

    walls =
        createBoundaryWalls();

    beginMapTransition(
        oldWallSnapshot,
        walls
    );

    const simpleGraph =
        buildSlideGraph(
            walls
        );

    const simpleReachable =
        getReachableStates(
            simpleGraph,
            startKey
        );

    const simpleCandidates =
        getGoalCandidates(
            simpleGraph,
            simpleReachable,
            startKey
        );

    if (
        simpleCandidates.length > 0
    ) {

        goal =
            parseKey(
                simpleCandidates[0].key
            );

    } else {

        goal = {
            c: COLS - 2,
            r: ROWS - 2
        };
    }

    const fallbackSafePath =
        getPathTo(
            simpleGraph,
            startKey,
            keyOf(goal.c, goal.r)
        ) || [];

    dangers =
        createDanger(
            simpleGraph,
            keyOf(goal.c, goal.r),
            fallbackSafePath
        );

    return true;
}


/* =========================================================
   맵 전환
========================================================= */

function beginMapTransition(
    oldWallSet,
    newWallSet
) {

    mapTransition.oldWalls =
        new Set(
            oldWallSet
        );

    mapTransition.newWalls =
        new Set(
            newWallSet
        );

    mapTransition.elapsed = 0;

    mapTransition.active = true;

    gameState = "transition";
}


function updateMapTransition(
    delta
) {

    if (
        !mapTransition.active
    ) {
        return;
    }

    mapTransition.elapsed +=
        delta;

    if (
        mapTransition.elapsed >=
        mapTransition.duration
    ) {

        mapTransition.elapsed =
            mapTransition.duration;

        mapTransition.active =
            false;

        gameState =
            tutorialActive ? "tutorial" : countdownActive ? "countdown" : (multiplayerSelfDead && multiplayerMatchActive) ? "multiplayerWaitingResult" : "playing";
    }
}


function getWallScaleForTransition(
    isNewWall
) {

    if (
        !mapTransition.active
    ) {
        return 1;
    }

    const p =
        clamp(
            mapTransition.elapsed /
            mapTransition.duration,
            0,
            1
        );

    return isNewWall
        ? 1 - Math.pow(1 - p, 3)
        : Math.pow(1 - p, 3);
}


/* =========================================================
   플레이어 초기화
========================================================= */

function resetPlayer() {

    player.c =
        stageStart.c;

    player.r =
        stageStart.r;

    player.x =
        stageStart.c * CELL;

    player.y =
        stageStart.r * CELL;

    movement = null;

    trail = [];
}



/* =========================================================
   일일 퀘스트 시스템
========================================================= */

const DAILY_QUEST_STORAGE_KEY = "slidingMazeDailyQuest_v2";
const DAILY_QUEST_COUNT = 3;
const DAILY_QUEST_REROLL_COUNT = 5;

const DAILY_QUEST_POOL = [
    { id:1, name:"슬라이딩 입문자", description:"맵 3개 클리어", reward:3 },
    { id:2, name:"슬라이딩 숙련자", description:"맵 10개 클리어", reward:6 },
    { id:3, name:"슬라이딩 마스터", description:"맵 20개 클리어", reward:10 },
    { id:4, name:"연속 질주", description:"5맵 연속 클리어", reward:5 },
    { id:5, name:"멈추지 않는 질주", description:"10맵 연속 클리어", reward:10 },
    { id:6, name:"시간과의 싸움", description:"제한시간 10초 이하 상태에서 3맵 클리어", reward:7 },
    { id:7, name:"마지막 순간", description:"맵 시작 후 5초 이내에 1맵 클리어", reward:8 },
    { id:8, name:"완벽한 출발", description:"목숨을 한 번도 잃지 않고 5맵 클리어", reward:6 },
    { id:9, name:"생존왕", description:"목숨 3개를 유지한 상태로 10맵 클리어", reward:10 },
    { id:10, name:"위험 회피자", description:"목숨을 잃지 않고 10맵 클리어", reward:10 },
    { id:11, name:"위험 구역 돌파", description:"위험 블록이 있는 맵 5개 클리어", reward:6 },
    { id:12, name:"아슬아슬", description:"위험 블록이 있는 맵을 3개 클리어", reward:5 },
    { id:13, name:"꾸준한 도전", description:"맵 8개 클리어", reward:5 },
    { id:14, name:"맵 정복자", description:"맵 12개 클리어", reward:7 },
    { id:15, name:"시간 조작", description:"시간 조작 시계 사용 상태로 3맵 클리어", reward:5 },
    { id:16, name:"철벽 방어", description:"에너지 보호막으로 충돌 1회 방어", reward:5 },
    { id:17, name:"길잡이", description:"경로 안내 사용 상태로 3맵 클리어", reward:5 },
    { id:18, name:"응급 구조", description:"응급 처치 발동 후 맵 1개 클리어", reward:6 },
    { id:19, name:"에너지 관리", description:"에너지 복구 장치 사용", reward:4 },
    { id:20, name:"아이템 없이", description:"아이템 없이 5맵 클리어", reward:6 },
    { id:21, name:"첫 대결", description:"2인 경쟁 경기 1회 완료", reward:3 },
    { id:22, name:"경쟁자", description:"2인 경쟁에서 1회 승리", reward:5 },
    { id:23, name:"연승 행진", description:"2인 경쟁 3연승", reward:8 },
    { id:24, name:"라이벌", description:"2인 경쟁 라운드 5회 진행", reward:6 },
    { id:25, name:"끝까지 살아남기", description:"상대보다 먼저 탈락하지 않고 경기 종료", reward:6 },
    { id:26, name:"역전극", description:"목숨 1개 상태에서 라운드 승리", reward:8 },
    { id:27, name:"무너지지 않는 자", description:"한 번도 탈락하지 않고 경기 승리", reward:7 },
    { id:28, name:"라운드 정복자", description:"2인 경쟁에서 5라운드 승리", reward:10 },
    { id:31, name:"끈기의 달인", description:"맵 넘기기를 사용하지 않고 10맵 클리어", reward:7 },
    { id:32, name:"다시 일어나기", description:"맵 넘기기를 3회 이상 사용한 뒤 3맵 연속 클리어", reward:6 },
    { id:33, name:"불굴의 의지", description:"목숨을 1개 잃은 맵을 클리어하고 이후 2맵 추가 클리어", reward:6 },
    { id:34, name:"아슬아슬한 생존", description:"목숨 1개 상태에서 3맵 연속 클리어", reward:8 },
    { id:35, name:"빠르게 빠르게", description:"제한시간의 50% 이상을 남기고 3맵 클리어", reward:7 },
    { id:36, name:"장거리 여행", description:"누적 20맵 클리어", reward:8 },
    { id:37, name:"여러 번 도전", description:"서로 다른 게임 3회 시작하고 각 게임에서 2맵 이상 클리어", reward:6 },
    { id:38, name:"오늘도 달린다", description:"하루 동안 15맵 클리어", reward:8 },
    { id:39, name:"시간과의 싸움", description:"제한시간 10초 이하 상태에서 5맵 클리어", reward:10 },
    { id:40, name:"흔들리지 않는 마음", description:"목숨을 한 번도 잃지 않고 10맵 연속 클리어", reward:10 },
    { id:41, name:"마지막 기회", description:"맵 넘기기를 3회 이상 사용한 뒤 5맵 클리어", reward:9 },
    { id:42, name:"끝까지 살아남기", description:"목숨 1개 상태로 5맵 연속 클리어", reward:10 },
    { id:43, name:"극한 질주", description:"제한시간의 50% 이상을 남기고 5맵 클리어", reward:10 }
];

let dailyQuestState = null;

function createDailyQuestProgress() {
    return {
        dailyClears: 0,
        noDeathStreak: 0,
        oneLifeStreak: 0,
        noSkipStreak: 0,
        postSkipStreak: 0,
        fastClears: 0,
        lowTimeClears: 0,
        lastMomentClears: 0,
        quickMapClears: 0,
        noItemClears: 0,
        dangerMapClears: 0,
        timeClockClears: 0,
        pathGuideClears: 0,
        firstAidClears: 0,
        shieldBlocks: 0,
        energyRecoveryUses: 0,
        skipsUsed: 0,
        fullLifeClears: 0,
        lostLifeMapActive: false,
        lostLifeMapCleared: false,
        postLostLifeClears: 0,
        gamesStarted: 0,
        qualifiedGames: 0,
        currentGameHadDeath: false,
        currentGameHadSkip: false,
        gameStartCounted: false,
        multiplayerMatchesCompleted: 0,
        multiplayerWins: 0,
        multiplayerWinStreak: 0,
        multiplayerRoundsPlayed: 0,
        multiplayerRoundsWon: 0,
        multiplayerMatchHadElimination: false,
        multiplayerMatchRoundWins: 0,
        multiplayerMatchActive: false,
        multiplayerMatchType: null,
        rerollHistory: []
    };
}

function shuffleArray(array) {
    const a = array.slice();
    for (let i = a.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [a[i], a[j]] = [a[j], a[i]];
    }
    return a;
}

function getQuestDateKey() { return getLocalDateKey(); }
function getQuestById(id) { return DAILY_QUEST_POOL.find(q => q.id === id) || null; }

function createFreshDailyQuestState() {
    const ids = shuffleArray(DAILY_QUEST_POOL.map(q => q.id));
    return {
        date: getQuestDateKey(),
        quests: ids.slice(0, DAILY_QUEST_COUNT),
        completed: [],
        rewardClaimed: [],
        rerolls: DAILY_QUEST_REROLL_COUNT,
        progress: createDailyQuestProgress()
    };
}

function saveDailyQuestState() {
    try { localStorage.setItem(DAILY_QUEST_STORAGE_KEY, JSON.stringify(dailyQuestState)); } catch (error) {}
}

function mergeQuestProgressDefaults(progress) {
    const defaults = createDailyQuestProgress();
    if (!progress || typeof progress !== "object") return defaults;
    Object.keys(defaults).forEach(key => {
        if (!(key in progress)) progress[key] = defaults[key];
    });
    return progress;
}

function loadDailyQuestState() {
    let saved = null;
    try { saved = JSON.parse(localStorage.getItem(DAILY_QUEST_STORAGE_KEY) || "null"); } catch (error) {}
    if (!saved || saved.date !== getQuestDateKey() || !Array.isArray(saved.quests) || saved.quests.length !== DAILY_QUEST_COUNT) {
        dailyQuestState = createFreshDailyQuestState();
        saveDailyQuestState();
        return;
    }
    dailyQuestState = saved;
    if (!Array.isArray(dailyQuestState.completed)) dailyQuestState.completed = [];
    if (!Array.isArray(dailyQuestState.rewardClaimed)) dailyQuestState.rewardClaimed = [];

    // 삭제된 멀티플레이 퀘스트 29, 30은 기존 저장 데이터에서도 제거합니다.
    dailyQuestState.quests = Array.isArray(dailyQuestState.quests)
        ? dailyQuestState.quests.filter(id => id !== 29 && id !== 30)
        : [];
    dailyQuestState.completed = dailyQuestState.completed.filter(id => id !== 29 && id !== 30);
    dailyQuestState.rewardClaimed = dailyQuestState.rewardClaimed.filter(id => id !== 29 && id !== 30);

    dailyQuestState.progress = mergeQuestProgressDefaults(dailyQuestState.progress);

    // 기존 목록에서 삭제된 퀘스트 때문에 슬롯이 부족하면 현재 퀘스트 풀에서 보충합니다.
    if (dailyQuestState.quests.length < DAILY_QUEST_COUNT) {
        const existing = new Set(dailyQuestState.quests);
        const candidates = shuffleArray(DAILY_QUEST_POOL.map(q => q.id))
            .filter(id => !existing.has(id));
        while (dailyQuestState.quests.length < DAILY_QUEST_COUNT && candidates.length) {
            dailyQuestState.quests.push(candidates.shift());
        }
    }
    // 새 「마지막 순간」 규칙은 별도 카운터를 사용하므로 기존 3초 규칙의
    // lastMomentClears 기록이 새 퀘스트 진행도에 섞이지 않습니다.
    if (typeof dailyQuestState.progress.quickMapClears !== "number") {
        dailyQuestState.progress.quickMapClears = 0;
    }
    if (typeof dailyQuestState.rerolls !== "number") dailyQuestState.rerolls = DAILY_QUEST_REROLL_COUNT;
    saveDailyQuestState();
}

function refreshDailyQuestIfNeeded() {
    if (!dailyQuestState || dailyQuestState.date !== getQuestDateKey()) {
        dailyQuestState = createFreshDailyQuestState();
        saveDailyQuestState();
        return true;
    }
    return false;
}

loadDailyQuestState();
function isDailyQuestCompleted(id) { return dailyQuestState.completed.includes(id); }
function completeDailyQuest(id) {
    if (isDailyQuestCompleted(id)) return;
    const quest = getQuestById(id);
    if (!quest) return;
    dailyQuestState.completed.push(id);
    saveDailyQuestState();
    setMessage(`퀘스트 완료! ${quest.name} · 보상을 받을 수 있습니다.`);
    updateUI();
}
function isDailyQuestRewardClaimed(id) { return dailyQuestState.rewardClaimed.includes(id); }
function claimDailyQuestReward(id) {
    if (!isDailyQuestCompleted(id) || isDailyQuestRewardClaimed(id)) return false;
    const quest = getQuestById(id);
    if (!quest) return false;
    dailyQuestState.rewardClaimed.push(id);
    coins += quest.reward;
    saveCoins();
    saveDailyQuestState();
    setMessage(`퀘스트 보상 수령! ${quest.name} · 🪙 +${quest.reward}`);
    updateUI();
    return true;
}

function rerollDailyQuests() {
    refreshDailyQuestIfNeeded();
    if (dailyQuestState.rerolls <= 0) { setMessage("오늘의 퀘스트 뽑기를 모두 사용했습니다."); return false; }
    const incompleteSlots = dailyQuestState.quests.map((id, index) => ({ id, index })).filter(item => !isDailyQuestCompleted(item.id));
    if (incompleteSlots.length === 0) { setMessage("모든 일일 퀘스트를 완료했습니다."); return false; }
    const fixedCompletedIds = new Set(dailyQuestState.quests.filter(id => isDailyQuestCompleted(id)));
    const candidates = shuffleArray(DAILY_QUEST_POOL.map(q => q.id)).filter(id => !isDailyQuestCompleted(id) && !fixedCompletedIds.has(id));
    if (candidates.length < incompleteSlots.length) { setMessage("뽑을 수 있는 다른 퀘스트가 부족합니다."); return false; }
    incompleteSlots.forEach((slot, index) => { dailyQuestState.quests[slot.index] = candidates[index]; });
    dailyQuestState.rerolls--;
    dailyQuestState.progress.rerollHistory.push(...candidates.slice(0, incompleteSlots.length));
    saveDailyQuestState();
    setMessage(`미완료 퀘스트 ${incompleteSlots.length}개를 다시 뽑았습니다.`);
    return true;
}

function resetQuestRunProgress() {
    const p = dailyQuestState.progress;
    p.noDeathStreak = 0;
    p.oneLifeStreak = 0;
    p.noSkipStreak = 0;
    p.postSkipStreak = 0;
    p.lostLifeMapActive = false;
    p.lostLifeMapCleared = false;
    p.postLostLifeClears = 0;
    p.currentGameHadDeath = false;
    p.currentGameHadSkip = false;
    p.gameStartCounted = false;
}

function onDailyQuestGameStart() {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    p.gamesStarted++;
    p.currentGameHadDeath = false;
    p.currentGameHadSkip = false;
    p.gameStartCounted = true;
    saveDailyQuestState();
}

function onDailyQuestMapSkip() {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    p.skipsUsed++;
    p.currentGameHadSkip = true;
    p.noSkipStreak = 0;
    p.postSkipStreak = 0;
    saveDailyQuestState();
}

function onDailyQuestDeath() {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    p.currentGameHadDeath = true;
    p.lostLifeMapActive = true;
    p.lostLifeMapCleared = false;
    p.postLostLifeClears = 0;
    p.noDeathStreak = 0;
    p.oneLifeStreak = 0;
    saveDailyQuestState();
}

function getDisplayedRemainingTime() {
    return Number(Math.max(0, remainingTime).toFixed(1));
}

function onDailyQuestClear() {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    const stageLimit = getStageTimeLimit() + activeTimeBonus;
    const displayedTime = getDisplayedRemainingTime();
    const elapsedTime = Math.max(0, stageLimit - remainingTime);

    p.dailyClears++;
    p.noDeathStreak++;
    p.noSkipStreak++;

    if (p.skipsUsed >= 3) p.postSkipStreak++;

    if (lives === 1) p.oneLifeStreak++;
    else p.oneLifeStreak = 0;

    if (remainingTime >= stageLimit * 0.5) p.fastClears++;
    if (remainingTime <= 10) p.lowTimeClears++;
    // 「마지막 순간」은 이제 남은 시간이 아니라 맵 시작 후 실제 경과 시간으로 판정합니다.
    // 정확히 5.0초 이내에 골인하면 성공입니다.
    if (elapsedTime <= 5.0) p.quickMapClears++;
    if (!activeItem) p.noItemClears++;
    if (dangers.size > 0) p.dangerMapClears++;
    if (activeItem === "timeClock") p.timeClockClears++;
    if (activeItem === "pathGuide") p.pathGuideClears++;
    if (activeItem === "firstAid" && firstAidCharged) p.firstAidClears++;
    if (lives === MAX_LIVES) p.fullLifeClears++;

    if (p.lostLifeMapActive) {
        p.lostLifeMapCleared = true;
        p.lostLifeMapActive = false;
        p.postLostLifeClears = 0;
    } else if (p.lostLifeMapCleared) {
        p.postLostLifeClears++;
    }

    if (p.dailyClears >= 3) completeDailyQuest(1);
    if (p.dailyClears >= 10) completeDailyQuest(2);
    if (p.dailyClears >= 20) completeDailyQuest(3);
    if (p.noDeathStreak >= 5) completeDailyQuest(4);
    if (p.noDeathStreak >= 10) completeDailyQuest(5);
    if (p.lowTimeClears >= 3) completeDailyQuest(6);
    if (p.quickMapClears >= 1) completeDailyQuest(7);
    if (p.noDeathStreak >= 5) completeDailyQuest(8);
    if (p.fullLifeClears >= 10) completeDailyQuest(9);
    if (p.noDeathStreak >= 10) completeDailyQuest(10);
    if (p.dangerMapClears >= 5) completeDailyQuest(11);
    if (p.dangerMapClears >= 3) completeDailyQuest(12);
    if (p.dailyClears >= 8) completeDailyQuest(13);
    if (p.dailyClears >= 12) completeDailyQuest(14);
    if (p.timeClockClears >= 3) completeDailyQuest(15);
    if (p.shieldBlocks >= 1) completeDailyQuest(16);
    if (p.pathGuideClears >= 3) completeDailyQuest(17);
    if (p.firstAidClears >= 1) completeDailyQuest(18);
    if (p.energyRecoveryUses >= 1) completeDailyQuest(19);
    if (p.noItemClears >= 5) completeDailyQuest(20);
    if (p.noSkipStreak >= 10) completeDailyQuest(31);
    if (p.postSkipStreak >= 3) completeDailyQuest(32);
    if (p.lostLifeMapCleared && p.postLostLifeClears >= 2) completeDailyQuest(33);
    if (p.oneLifeStreak >= 3) completeDailyQuest(34);
    if (p.fastClears >= 3) completeDailyQuest(35);
    if (p.dailyClears >= 20) completeDailyQuest(36);
    if (p.qualifiedGames >= 3) completeDailyQuest(37);
    if (p.dailyClears >= 15) completeDailyQuest(38);
    if (p.lowTimeClears >= 5) completeDailyQuest(39);
    if (p.noDeathStreak >= 10) completeDailyQuest(40);
    if (p.postSkipStreak >= 5) completeDailyQuest(41);
    if (p.oneLifeStreak >= 5) completeDailyQuest(42);
    if (p.fastClears >= 5) completeDailyQuest(43);

    saveDailyQuestState();
}

function onDailyQuestMultiplayerMatchStart(type) {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    p.multiplayerMatchActive = true;
    p.multiplayerMatchType = type || multiplayerMatchType || "quick";
    p.multiplayerMatchHadElimination = false;
    p.multiplayerMatchRoundWins = 0;
    saveDailyQuestState();
}

function onDailyQuestMultiplayerRoundStart() {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    if (!p.multiplayerMatchActive) return;
    p.multiplayerRoundsPlayed++;
    if (p.multiplayerRoundsPlayed >= 5) completeDailyQuest(24);
    saveDailyQuestState();
}

function onDailyQuestMultiplayerRoundWin() {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    if (!p.multiplayerMatchActive) return;
    p.multiplayerRoundsWon++;
    p.multiplayerMatchRoundWins++;
    if (lives === 1) completeDailyQuest(26);
    if (p.multiplayerRoundsWon >= 5) completeDailyQuest(28);
    saveDailyQuestState();
}

function onDailyQuestMultiplayerElimination() {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    if (!p.multiplayerMatchActive) return;
    p.multiplayerMatchHadElimination = true;
    saveDailyQuestState();
}

function onDailyQuestMultiplayerMatchEnd(result) {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    if (!p.multiplayerMatchActive) return;

    const won = result === multiplayerRole;
    const completed = Boolean(result);

    if (completed) p.multiplayerMatchesCompleted++;
    if (won) {
        p.multiplayerWins++;
        p.multiplayerWinStreak++;
        if (p.multiplayerWinStreak >= 3) completeDailyQuest(23);
        completeDailyQuest(22);
        if (!p.multiplayerMatchHadElimination) completeDailyQuest(27);
        if (!p.multiplayerMatchHadElimination) completeDailyQuest(25);
    } else {
        p.multiplayerWinStreak = 0;
    }

    if (p.multiplayerMatchesCompleted >= 1) completeDailyQuest(21);

    p.multiplayerMatchActive = false;
    p.multiplayerMatchType = null;
    p.multiplayerMatchHadElimination = false;
    p.multiplayerMatchRoundWins = 0;
    saveDailyQuestState();
}

function onDailyQuestGameEnd() {
    refreshDailyQuestIfNeeded();
    const p = dailyQuestState.progress;
    if (p.gameStartCounted && clearCount >= 2) {
        p.qualifiedGames++;
        if (p.qualifiedGames >= 3) completeDailyQuest(37);
    }
    p.gameStartCounted = false;
    saveDailyQuestState();
}

function onDailyQuestEnergyRecoveryUse() {
    refreshDailyQuestIfNeeded();
    dailyQuestState.progress.energyRecoveryUses++;
    completeDailyQuest(19);
    saveDailyQuestState();
}

function onDailyQuestShieldBlock() {
    refreshDailyQuestIfNeeded();
    dailyQuestState.progress.shieldBlocks++;
    completeDailyQuest(16);
    saveDailyQuestState();
}

function getSkinButton() { return { x: 168, y: window.innerWidth <= 520 ? 112 : 74, w: 42, h: 42 }; }

function drawSkinButton() {
    const b = getSkinButton();
    ctx.save();
    ctx.fillStyle = "rgba(9,12,17,0.68)";
    ctx.strokeStyle = "rgba(255,255,255,0.14)";
    ctx.lineWidth = 1;
    ctx.beginPath(); ctx.roundRect(b.x,b.y,b.w,b.h,12); ctx.fill(); ctx.stroke();
    drawClearEmoji("👔", b.x+b.w/2, b.y+b.h/2+1, 25);
    ctx.restore();
}

function getQuestButton() {
    return { x: 220, y: window.innerWidth <= 520 ? 112 : 74, w: 42, h: 42 };
}

function drawQuestButton() {
    const b = getQuestButton();
    ctx.save();
    ctx.fillStyle = "rgba(9,12,17,0.68)";
    ctx.strokeStyle = "rgba(255,255,255,0.14)";
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.roundRect(b.x, b.y, b.w, b.h, 12);
    ctx.fill();
    ctx.stroke();
    ctx.fillStyle = "#f0f3f6";
    ctx.font = "bold 22px Arial, sans-serif";
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    drawClearEmoji("📜", b.x + b.w / 2, b.y + b.h / 2 + 1, 25);
    ctx.restore();
}

let questOpen = false;

function getDailyQuestProgressInfo(quest) {
    const p = dailyQuestState.progress || createDailyQuestProgress();
    let current = 0;
    let target = quest.target || 0;

    switch (quest.id) {
        case 1: current = p.dailyClears; target = 3; break;
        case 2: current = p.dailyClears; target = 10; break;
        case 3: current = p.dailyClears; target = 20; break;
        case 4: current = p.noDeathStreak; target = 5; break;
        case 5: current = p.noDeathStreak; target = 10; break;
        case 6: current = p.lowTimeClears; target = 3; break;
        case 7: current = p.quickMapClears; target = 1; break;
        case 8: current = p.noDeathStreak; target = 5; break;
        case 9: current = p.fullLifeClears; target = 10; break;
        case 10: current = p.noDeathStreak; target = 10; break;
        case 11: current = p.dangerMapClears; target = 5; break;
        case 12: current = p.dangerMapClears; target = 3; break;
        case 13: current = p.dailyClears; target = 8; break;
        case 14: current = p.dailyClears; target = 12; break;
        case 15: current = p.timeClockClears; target = 3; break;
        case 16: current = p.shieldBlocks; target = 1; break;
        case 17: current = p.pathGuideClears; target = 3; break;
        case 18: current = p.firstAidClears; target = 1; break;
        case 19: current = p.energyRecoveryUses; target = 1; break;
        case 20: current = p.noItemClears; target = 5; break;
        case 21: current = p.multiplayerMatchesCompleted; target = 1; break;
        case 22: current = p.multiplayerWins; target = 1; break;
        case 23: current = p.multiplayerWinStreak; target = 3; break;
        case 24: current = p.multiplayerRoundsPlayed; target = 5; break;
        case 25: current = isDailyQuestCompleted(25) ? 1 : 0; target = 1; break;
        case 26: current = isDailyQuestCompleted(26) ? 1 : 0; target = 1; break;
        case 27: current = isDailyQuestCompleted(27) ? 1 : 0; target = 1; break;
        case 28: current = p.multiplayerRoundsWon; target = 5; break;
        case 31: current = p.noSkipStreak; target = 10; break;
        case 32: current = p.postSkipStreak; target = 3; break;
        case 33: current = p.lostLifeMapCleared ? 1 + p.postLostLifeClears : 0; target = 3; break;
        case 34: current = p.oneLifeStreak; target = 3; break;
        case 35: current = p.fastClears; target = 3; break;
        case 36: current = p.dailyClears; target = 20; break;
        case 37: current = p.qualifiedGames; target = 3; break;
        case 38: current = p.dailyClears; target = 15; break;
        case 39: current = p.lowTimeClears; target = 5; break;
        case 40: current = p.noDeathStreak; target = 10; break;
        case 41: current = p.postSkipStreak; target = 5; break;
        case 42: current = p.oneLifeStreak; target = 5; break;
        case 43: current = p.fastClears; target = 5; break;
        default: current = 0; target = quest.target || 1;
    }

    if (isDailyQuestCompleted(quest.id)) current = target;
    current = Math.max(0, Math.min(target, current));
    return { current, target, percent: target > 0 ? Math.round((current / target) * 100) : 0 };
}

let questRewardOverlaySignature = "";

function claimQuestRewardFromOverlay(id, button) {
    if (!questOpen || !dailyQuestState || !button || button.disabled) return;

    refreshDailyQuestIfNeeded();

    const claimedNow = claimDailyQuestReward(id);
    if (!claimedNow) {
        syncQuestRewardOverlay(true);
        return;
    }

    playUIClickSound();
    button.disabled = true;
    button.textContent = "수령 완료 ✓";
    updateUI();
    syncQuestRewardOverlay(true);
}

function syncQuestRewardOverlay(force = false) {
    if (!questRewardOverlay) return;

    const shouldShow = (
        gameState === "start" &&
        questOpen &&
        !!dailyQuestState
    );

    if (!shouldShow) {
        if (questRewardOverlaySignature !== "hidden") {
            questRewardOverlay.innerHTML = "";
            questRewardOverlaySignature = "hidden";
        }
        questRewardOverlay.style.display = "none";
        questRewardOverlay.setAttribute("aria-hidden", "true");
        return;
    }

    refreshDailyQuestIfNeeded();

    // 게임 루프는 매 프레임 syncQuestRewardOverlay()를 호출합니다.
    // 매 프레임 innerHTML을 비우고 버튼을 새로 만들면 모바일 Safari에서
    // pointerdown과 click 사이에 기존 버튼이 사라져 click이 끊길 수 있습니다.
    // 실제 퀘스트 상태가 바뀐 경우에만 DOM을 다시 만듭니다.
    const signature = JSON.stringify({
        gameState,
        questOpen,
        quests: dailyQuestState.quests,
        completed: dailyQuestState.completed,
        rewardClaimed: dailyQuestState.rewardClaimed
    });

    if (!force && questRewardOverlaySignature === signature) {
        return;
    }

    questRewardOverlay.innerHTML = "";

    let buttonCount = 0;

    for (let i = 0; i < DAILY_QUEST_COUNT; i++) {
        const id = dailyQuestState.quests[i];
        const q = getQuestById(id);
        if (!q) continue;

        if (!isDailyQuestCompleted(id) || isDailyQuestRewardClaimed(id)) {
            continue;
        }

        const rowY = 122 + i * 77;
        const button = document.createElement("button");

        button.type = "button";
        button.className = "quest-reward-button";
        button.dataset.questId = String(id);
        button.id = `quest-reward-button-${id}`;
        button.setAttribute(
            "aria-label",
            `${q.name} 보상 받기 · ${q.reward}코인`
        );

        // Canvas와 동일한 위치에 딱 하나만 올립니다.
        button.style.left = `${(565 / WIDTH) * 100}%`;
        button.style.top = `${((rowY + 22) / HEIGHT) * 100}%`;
        button.style.width = `${(153 / WIDTH) * 100}%`;
        button.style.height = `${(30 / HEIGHT) * 100}%`;
        button.textContent = "보상 받기  ›";

        // iPad Safari의 touch/pointer 이벤트가 Canvas로 내려가지 않도록
        // 버튼에서만 이벤트를 소비합니다.
        const stopEvent = event => {
            event.stopPropagation();
        };

        button.addEventListener("pointerdown", stopEvent, { passive: true });
        button.addEventListener("pointerup", stopEvent, { passive: true });
        button.addEventListener("touchstart", stopEvent, { passive: true });
        button.addEventListener("touchend", stopEvent, { passive: true });

        button.addEventListener("click", event => {
            event.preventDefault();
            event.stopPropagation();

            // 이미 다른 이벤트에서 수령된 경우 중복 지급을 막습니다.
            if (button.disabled) return;

            claimQuestRewardFromOverlay(id, button);
        });

        questRewardOverlay.appendChild(button);
        buttonCount++;
    }

    questRewardOverlay.style.display = buttonCount > 0 ? "block" : "none";
    questRewardOverlay.setAttribute(
        "aria-hidden",
        buttonCount > 0 ? "false" : "true"
    );
    questRewardOverlaySignature = signature;
}
function drawQuestPanel() {
    refreshDailyQuestIfNeeded();
    syncQuestRewardOverlay();
    ctx.save();
    ctx.fillStyle = "rgba(0,0,0,0.78)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);

    const panel = { x: 35, y: 25, w: 730, h: 550 };
    ctx.fillStyle = "#171c25";
    ctx.strokeStyle = "#394352";
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.roundRect(panel.x, panel.y, panel.w, panel.h, 20);
    ctx.fill();
    ctx.stroke();

    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    ctx.fillStyle = "#f3f5f7";
    ctx.font = "bold 28px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("📜 일일 퀘스트", WIDTH / 2, 65);

    ctx.fillStyle = "#ffd76a";
    ctx.font = "600 14px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(`🪙 ${coins}코인`, WIDTH / 2, 97);

    for (let i = 0; i < DAILY_QUEST_COUNT; i++) {
        const id = dailyQuestState.quests[i];
        const q = getQuestById(id);
        if (!q) continue;

        const completed = isDailyQuestCompleted(id);
        const claimed = completed && isDailyQuestRewardClaimed(q.id);
        const info = getDailyQuestProgressInfo(q);
        const y = 122 + i * 77;

        ctx.fillStyle = claimed
            ? "rgba(255,255,255,0.018)"
            : completed
                ? "rgba(100,210,130,0.13)"
                : "rgba(255,255,255,0.045)";
        ctx.strokeStyle = claimed
            ? "rgba(255,255,255,0.055)"
            : completed
                ? "rgba(100,220,140,0.45)"
                : "rgba(255,255,255,0.12)";
        ctx.lineWidth = 1;
        ctx.beginPath();
        ctx.roundRect(58, y, 684, 64, 12);
        ctx.fill();
        ctx.stroke();

        ctx.textAlign = "left";
        ctx.fillStyle = claimed
            ? "rgba(243,245,247,0.38)"
            : completed
                ? "#7dff9d"
                : "#f3f5f7";
        ctx.font = "bold 15px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(`${i + 1}. ${q.name}`, 75, y + 15);

        ctx.fillStyle = claimed ? "rgba(159,170,183,0.38)" : "#9faab7";
        ctx.font = "11px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(q.description, 75, y + 31);

        // 현재 달성치 / 목표치를 % 막대 위에 표시
        ctx.textAlign = "right";
        ctx.fillStyle = claimed
            ? "rgba(220,229,239,0.34)"
            : completed
                ? "#7dff9d"
                : "#dce5ef";
        ctx.font = "600 11px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(`${info.current}/${info.target} · ${info.percent}%`, 535, y + 44);

        // 진행도 % 바
        const barX = 75;
        const barY = y + 51;
        const barW = 455;
        const barH = 7;
        ctx.fillStyle = claimed ? "rgba(255,255,255,0.055)" : "rgba(255,255,255,0.10)";
        ctx.beginPath();
        ctx.roundRect(barX, barY, barW, barH, 4);
        ctx.fill();
        ctx.fillStyle = claimed
            ? "rgba(110,232,139,0.20)"
            : completed
                ? "#6ee88b"
                : "#5eb7ff";
        ctx.beginPath();
        ctx.roundRect(barX, barY, barW * (info.percent / 100), barH, 4);
        ctx.fill();

        if (claimed) {
            ctx.textAlign = "center";
            ctx.fillStyle = "rgba(125,255,157,0.42)";
            ctx.font = "600 11px Pretendard, Noto Sans KR, sans-serif";
            ctx.fillText(`🪙 +${q.reward}코인`, 641.5, y + 12);

            // 수령 완료 상태는 Canvas가 표시합니다.
            // 실제 미수령 보상 버튼은 HTML <button> 하나만 표시합니다.
            ctx.fillStyle = "rgba(110,232,139,0.10)";
            ctx.strokeStyle = "rgba(110,232,139,0.34)";
            ctx.lineWidth = 1.5;
            ctx.beginPath();
            ctx.roundRect(565, y + 22, 153, 30, 7);
            ctx.fill();
            ctx.stroke();

            ctx.textAlign = "center";
            ctx.fillStyle = "rgba(125,255,157,0.78)";
            ctx.font = "bold 12px Pretendard, Noto Sans KR, sans-serif";
            ctx.fillText("보상 수령 완료 ✓", 641.5, y + 39);
        } else {
            ctx.textAlign = "center";
            ctx.fillStyle = completed ? "#ffd76a" : "rgba(255,215,106,0.38)";
            ctx.font = "600 11px Pretendard, Noto Sans KR, sans-serif";
            ctx.fillText(`🪙 +${q.reward}코인`, 641.5, y + 12);

            if (!completed) {
                // 미달성 상태만 Canvas에 비활성 보상 표시.
                ctx.fillStyle = "rgba(99,184,255,0.08)";
                ctx.strokeStyle = "rgba(99,184,255,0.18)";
                ctx.lineWidth = 1;
                ctx.beginPath();
                ctx.roundRect(565, y + 22, 153, 30, 7);
                ctx.fill();
                ctx.stroke();

                ctx.textAlign = "center";
                ctx.fillStyle = "rgba(255,255,255,0.28)";
                ctx.font = "bold 12px Pretendard, Noto Sans KR, sans-serif";
                ctx.fillText("보상 받기", 641.5, y + 39);
            }
            // completed + unclaimed 상태의 "보상 받기"는
            // 아래 syncQuestRewardOverlay()가 만드는 실제 HTML 버튼만 담당합니다.
        }
    }

    const canReroll = dailyQuestState.rerolls > 0 && dailyQuestState.quests.some(id => !isDailyQuestCompleted(id));
    ctx.globalAlpha = canReroll ? 1 : 0.45;
    drawSettingsButton(WIDTH / 2 - 105, 410, 210, 38, `퀘스트 다시 뽑기 ${dailyQuestState.rerolls}/${DAILY_QUEST_REROLL_COUNT}`);
    ctx.globalAlpha = 1;

    drawSettingsButton(WIDTH / 2 - 80, 465, 160, 32, "닫기");
    ctx.restore();
    syncQuestRewardOverlay();
}

/* =========================================================
   새 게임
========================================================= */

function startNewGame() {

    // 새 게임은 언제나 배경음악의 처음부터 시작합니다.
    stopBackgroundMusic(true);

    // iPad/iOS에서는 게임 중 타이머가 끝난 뒤 발생하는 play()가
    // 사용자 제스처로 인정되지 않을 수 있으므로, 게임 시작 터치/키 입력 때
    // gameover.m4a를 미리 무음 재생하여 해당 오디오 요소를 활성화합니다.
    unlockEffectAudio();
    primeEffectSound("gameOver");

    resetOneShotEffects();
    refreshDailyQuestIfNeeded();
    questOpen = false;
    settingsOpen = false;

    clearTimeout(
        roundTimer
    );

    gameState = "playing";

    lives =
        MAX_LIVES;

    clearCount = 0;

    clearStreak = 0;

    maxClearStreak = 0;

    lifeLossCount = 0;
    mapSkipCount = 0;

    mapSkips =
        MAX_MAP_SKIPS;

    stageStart = {
        c: START.c,
        r: START.r
    };

    recordSavedForRun =
        false;

    runStartTime =
        new Date();

    onDailyQuestGameStart();
    activateItemForRun();

    resetRecoil();

    flash.alpha = 0;

    startRound();

    // 로딩이 끝나 게임 화면이 켜지면 바로 시작하지 않고 3초 카운트다운 후 시작합니다.
    beginIntroCountdown();
}


/* =========================================================
   라운드 시작
========================================================= */

function startRound() {

    clearTimeout(
        roundTimer
    );

    resetOneShotEffects();

    gameState = "playing";

    remainingTime =
        getStageTimeLimit() + activeTimeBonus;

    resetPlayer();

    pathGuideUses = 0;
    pathGuidePath = [];

    if (multiplayerMatchActive) {
        createMapWithSeed(multiplayerSeed);
    } else {
        createMap();
    }

    if (activeItem === "pathGuide") {
        showPathGuide();
        pathGuideUses = 1;
    }

    if (activeItem === "firstAid") {
        tryAutoFirstAid();
    }

    setMessage("");

    flash.alpha = 0;

    shake.power = 0;
    shake.time = 0;

    updateUI();
}


/* =========================================================
   맵 넘기기
========================================================= */

function skipMap() {

    // 튜토리얼 중에는 실제 게임 상태를 건드리지 않고 튜토리얼 전용 동작만 실행합니다.
    if (tutorialActive) {
        tutorialSkipAction();
        return;
    }

    // 2인용 대전 중 더블 터치(G 키)는 맵 넘기기 대신 포기 확인 창을 엽니다.
    if (multiplayerMatchActive) {
        if (gameState !== "multiplayerResult" && gameState !== "expResult") openGamePopup("multi");
        return;
    }

    if (countdownActive || loadingActive || gamePopupOpen) {
        return;
    }

    if (gameState === "multiplayerResult" || gameState === "expResult") {
        return;
    }

    if (
        gameState === "start" ||
        gameState === "gameover"
    ) {
        return;
    }

    if (
        mapSkips <= 0
    ) {
        if (openEnergyRecoveryChoice()) {
            showItemWarning("에너지 복구 장치를 사용할 수 있습니다.");
        } else {
            // 맵 넘기기를 모두 소진한 뒤 더블 터치 → 게임 종료 확인 창
            openGamePopup("solo");
        }

        return;
    }

    clearTimeout(
        roundTimer
    );

    mapSkips--;
    mapSkipCount++;
    onDailyQuestMapSkip();

    if (mapSkips === 0) {
        openEnergyRecoveryChoice();
    }

    gameState =
        "playing";

    remainingTime =
        getStageTimeLimit() + activeTimeBonus;

    resetPlayer();

    pathGuideUses = 0;
    pathGuidePath = [];

    createMap();

    if (activeItem === "pathGuide") {
        showPathGuide();
        pathGuideUses = 1;
    }

    if (activeItem === "firstAid") {
        tryAutoFirstAid();
    }

    applyImpactRecoil(
        90,
        5,
        0.18
    );

    flash.color =
        "#b995ff";

    flash.alpha =
        0.12;

    setMessage(
        `맵을 넘겼습니다. 남은 횟수 ${mapSkips}회`
    );

    updateUI();
}


/* =========================================================
   이동 시작
========================================================= */

function startMove(
    dc,
    dr
) {

    if (gameState === "tutorial") {
        const tutorialStepData = TUTORIAL_STEPS[tutorialStep];
        if (tutorialLocked || !tutorialStepData || tutorialStepData.type === "info") {
            return;
        }
    } else if (
        gameState !== "playing"
    ) {
        return;
    }

    if (movement) {
        return;
    }

    const destination =
        getSlideDestination(
            player.c,
            player.r,
            dc,
            dr
        );

    if (
        destination.c === player.c &&
        destination.r === player.r
    ) {

        applyRecoil(
            dc,
            dr,
            55,
            3,
            0.12
        );

        return;
    }

    const startX =
        player.c * CELL;

    const startY =
        player.r * CELL;

    const targetX =
        destination.c * CELL;

    const targetY =
        destination.r * CELL;

    const distance =
        Math.abs(
            destination.c -
            player.c
        ) +
        Math.abs(
            destination.r -
            player.r
        );

    const duration =
        Math.max(
            0.075,
            distance * 0.010
        );

    // 경로 안내가 아직 실제로 표시 중일 때만 한 번 페이드아웃합니다.
    // 이미 자연스럽게 사라지는 중이거나 완전히 사라진 뒤에는 다시 시작하지 않습니다.
    const guideNow = performance.now();
    if (
        activeItem === "pathGuide" &&
        pathGuidePath.length > 1 &&
        guideNow < pathGuideVisibleUntil &&
        guideNow < pathGuideAutoFadeAt &&
        pathGuideFadeStart === 0
    ) {
        pathGuideFadeStart = guideNow;
        pathGuideVisibleUntil =
            guideNow +
            PATH_GUIDE_FADE_DURATION * 1000;
    }

    movement = {
        startX,
        startY,
        targetX,
        targetY,
        duration,
        elapsed: 0,
        fromC: player.c,
        fromR: player.r,
        toC: destination.c,
        toR: destination.r,
        dc,
        dr
    };
}


/* =========================================================
   이동 업데이트
========================================================= */

function updateMovement(
    delta
) {

    if (!movement) {
        return;
    }

    movement.elapsed +=
        delta;

    const progress =
        clamp(
            movement.elapsed /
            movement.duration,
            0,
            1
        );

    const eased =
        1 -
        Math.pow(
            1 - progress,
            3
        );

    player.x =
        movement.startX +
        (
            movement.targetX -
            movement.startX
        ) *
        eased;

    player.y =
        movement.startY +
        (
            movement.targetY -
            movement.startY
        ) *
        eased;

    if (
        trail.length === 0 ||
        Math.hypot(
            player.x -
            trail[
                trail.length - 1
            ].x,

            player.y -
            trail[
                trail.length - 1
            ].y
        ) > 8
    ) {

        trail.push({
            x: player.x,
            y: player.y,
            life: 1
        });

        if (
            trail.length > 12
        ) {
            trail.shift();
        }
    }

    if (
        progress >= 1
    ) {

        player.c =
            movement.toC;

        player.r =
            movement.toR;

        player.x =
            movement.targetX;

        player.y =
            movement.targetY;

        const finishedMovement =
            movement;

        movement = null;

        // 벽 충돌은 시각적 반동만 적용하고 효과음은 재생하지 않습니다.

        applyRecoil(
            finishedMovement.dc,
            finishedMovement.dr,
            10,
            1,
            0.10
        );

        sendMultiplayerPosition(true);
        checkTile();
    }
}


/* =========================================================
   칸 검사
========================================================= */

function checkTile() {

    if (tutorialActive) {
        tutorialCheckTile();
        return;
    }

    const current =
        keyOf(
            player.c,
            player.r
        );

    if (
        dangers.has(current)
    ) {

        dieGame();

        return;
    }

    if (
        goal &&
        player.c === goal.c &&
        player.r === goal.r
    ) {

        clearGame();
    }
}


/* =========================================================
   클리어
========================================================= */

function clearGame() {

    if (
        gameState !== "playing"
    ) {
        return;
    }

    if (multiplayerMatchActive) {
        movement = null;
        gameState = "multiplayerWaitingRound";
        multiplayerRoundTransition = false;
        multiplayerSend({ type: "finish", round: multiplayerRound, position: { c: player.c, r: player.r } });
        setMessage("클리어! 상대 결과를 확인하는 중...");
        updateUI();
        return;
    }

    stageStart = {
        c: player.c,
        r: player.r
    };

    gameState =
        "cleared";

    playEffectSound("goal", "goal");

    movement = null;

    clearCount++;
    onDailyQuestClear();

    if (
        clearCount >
        maxClearCount
    ) {

        maxClearCount =
            clearCount;

        localStorage.setItem(
            "slidingMazeMaxClearCount",
            String(maxClearCount)
        );
    }

    clearStreak++;

    coins++;
    saveCoins();

    if (activeItem === "energyShield" && clearCount % 2 === 0) {
        shieldCharges++;
        showItemWarning(`에너지 보호 시스템 재정비 완료 · 보호막 ${shieldCharges}개`);
    }

    if (activeItem === "firstAid" && clearCount % 4 === 0) {
        firstAidCharged = true;
        tryAutoFirstAid();
    }

    maxClearStreak =
        Math.max(
            maxClearStreak,
            clearStreak
        );

    allTimeBestStreak =
        Math.max(
            allTimeBestStreak,
            clearStreak
        );

    try {

        localStorage.setItem(
            "slideMazeBestStreak",
            String(
                allTimeBestStreak
            )
        );

    } catch (error) {}

    // 클리어가 확정된 순간 최신 점수를 랭킹에 반영합니다.
    // 게임 오버까지 기다리지 않아도 현재 기록이 서버에 저장됩니다.
    submitV28Score();

    applyImpactRecoil(
        150,
        12,
        0.32
    );

    flash.color =
        "#63ff91";

    flash.alpha =
        0.25;

    setMessage(
        `클리어! ${clearCount}회`
    );

    updateUI();

    roundTimer =
        setTimeout(
            () => {

                if (
                    gameState ===
                    "cleared"
                ) {
                    startRound();
                }

            },
            700
        );
}


/* =========================================================
   사망
========================================================= */

function dieGame() {

    if (
        gameState !== "playing"
    ) {
        return;
    }

    movement = null;
    playEffectSound("damage");

    const dangerKey = keyOf(player.c, player.r);

    if (activeItem === "energyShield" && shieldCharges > 0) {
        shieldCharges--;
        playEffectSound("itemUse");
        onDailyQuestShieldBlock();
        dangers.delete(dangerKey);
        applyImpactRecoil(130, 9, 0.25);
        flash.color = "#69c8ff";
        flash.alpha = 0.20;
        setMessage(`에너지 보호막 시스템 발동 · 보호막 ${shieldCharges}개 남음`);
        tryAutoFirstAid();
        updateUI();
        return;
    }

    lives--;
    lifeLossCount++;
    onDailyQuestDeath();

    if (tryAutoFirstAid()) {
        gameState = "playing";
        clearStreak = 0;
        updateUI();
        return;
    }

    clearStreak = 0;

    applyImpactRecoil(
        190,
        14,
        0.40
    );

    flash.color =
        "#ff3e4d";

    flash.alpha =
        0.32;

    if (multiplayerMatchActive) {
        sendMultiplayerEliminated();
        return;
    }

    gameState = "dead";

    if (
        lives > 0
    ) {

        setMessage(
            `위험 블록! 목숨 ${lives}개 남음`
        );

        updateUI();

        roundTimer =
            setTimeout(
                () => {

                    if (
                        gameState ===
                        "dead"
                    ) {
                        startRound();
                    }

                },
                850
            );

    } else {

        if (multiplayerMatchActive) {
            sendMultiplayerEliminated();
            return;
        }

        setMessage(
            "목숨을 모두 잃었습니다."
        );

        updateUI();

        roundTimer =
            setTimeout(
                () => {

                    if (
                        gameState ===
                        "dead"
                    ) {
                        finishGameOver();
                    }

                },
                850
            );
    }
}


/* =========================================================
   시간 초과
========================================================= */

function timeoutGame() {

    if (
        gameState !== "playing"
    ) {
        return;
    }

    movement = null;

    remainingTime = 0;

    lives--;
    lifeLossCount++;

    if (tryAutoFirstAid()) {
        gameState = "playing";
        clearStreak = 0;
        remainingTime = getStageTimeLimit() + activeTimeBonus;
        updateUI();
        return;
    }

    clearStreak = 0;

    applyImpactRecoil(
        130,
        10,
        0.30
    );

    flash.color =
        "#ff9d3b";

    flash.alpha =
        0.32;

    if (multiplayerMatchActive) {
        sendMultiplayerEliminated();
        return;
    }

    gameState =
        "timeout";

    if (
        lives > 0
    ) {

        setMessage(
            `시간 초과! 목숨 ${lives}개 남음`
        );

    } else {

        if (multiplayerMatchActive) {
            sendMultiplayerEliminated();
            return;
        }

        setMessage(
            "시간 초과! 목숨을 모두 잃었습니다."
        );
    }

    updateUI();

    roundTimer =
        setTimeout(
            () => {

                if (
                    gameState !==
                    "timeout"
                ) {
                    return;
                }

                if (
                    lives > 0
                ) {

                    startRound();

                } else {

                    finishGameOver();
                }

            },
            850
        );
}


/* =========================================================
   게임 오버
========================================================= */

function finishGameOver() {

    clearTimeout(
        roundTimer
    );

    if (multiplayerMatchActive) {
        sendMultiplayerEliminated();
        return;
    }

    gameState =
        "gameover";

    playEffectSound("gameOver");

    onDailyQuestGameEnd();

    movement = null;

    deactivateItemForRun();

    applyImpactRecoil(
        240,
        18,
        0.55
    );

    flash.color =
        "#ff263d";

    flash.alpha =
        0.28;

    saveRecentRecord();
    submitV28Score();
    submitPlayStats("solo");
    pendingExpAward = calculateSoloExperience();
    pendingExpReason = "solo";

    setMessage(
        `게임 오버 — ${clearCount}회 클리어 / ${maxClearStreak}회 연속 클리어`
    );

    updateUI();
}


/* =========================================================
   기록 저장
========================================================= */

function saveRecentRecord() {

    if (
        recordSavedForRun
    ) {
        return;
    }

    recordSavedForRun =
        true;

    const now =
        new Date();

    const formatRecordTime =
        date =>
            date.toLocaleTimeString(
                "ko-KR",
                {
                    hour: "numeric",
                    minute: "2-digit",
                    hour12: true
                }
            );

    const startTime =
        runStartTime ||
        now;

    const record = {
        startTime:
            formatRecordTime(
                startTime
            ),

        endTime:
            formatRecordTime(
                now
            ),

        clears:
            clearCount,

        maxStreak:
            maxClearStreak
    };

    recentRecords.unshift(
        record
    );

    recentRecords =
        recentRecords.slice(
            0,
            5
        );

    try {

        localStorage.setItem(
            "slideMazeRecentRecords",
            JSON.stringify(
                recentRecords
            )
        );

    } catch (error) {}
}


/* =========================================================
   UI 업데이트
========================================================= */

function updateUI() {

    updateStartMenuOverlay();

    document.getElementById(
        "time"
    ).textContent =
        `시간 ${remainingTime.toFixed(1)}초`;

    let hearts = "";

    for (
        let i = 0;
        i < MAX_LIVES;
        i++
    ) {

        hearts +=
            i < lives
                ? "♥"
                : "♡";

        if (
            i <
            MAX_LIVES - 1
        ) {
            hearts += " ";
        }
    }

    document.getElementById(
        "lives"
    ).textContent =
        `목숨 ${hearts}`;

    document.getElementById(
        "clears"
    ).textContent =
        `클리어 ${clearCount}회`;

    const scoreElement = document.getElementById("score");
    if (scoreElement) {
        scoreElement.textContent =
            `점수 ${calculateV28Score().toLocaleString("ko-KR")}`;
    }

    let skipIcons = "";

    for (
        let i = 0;
        i < MAX_MAP_SKIPS;
        i++
    ) {

        skipIcons +=
            i < mapSkips
                ? "●"
                : "○";

        if (
            i <
            MAX_MAP_SKIPS - 1
        ) {
            skipIcons += " ";
        }
    }

    const mapSkipsElement = document.getElementById("mapSkips");
    mapSkipsElement.textContent = `맵 넘기기 ${skipIcons}`;
    mapSkipsElement.style.display = (multiplayerMatchActive || gameState === "multiplayerWaitingRound" || gameState === "multiplayerWaitingResult" || gameState === "multiplayerResult") ? "none" : "block";

    const itemInfo = document.getElementById("itemInfo");
    const itemWarning = document.getElementById("itemWarning");

    if (activeItem) {
        itemInfo.textContent =
            `${ITEM_DATA[activeItem].icon} ${ITEM_DATA[activeItem].name}`;
    } else {
        itemInfo.textContent = "아이템 미사용";
    }

    itemWarning.textContent =
        performance.now() < itemWarningUntil
            ? itemWarningText
            : "";
}


/* =========================================================
   EXP 결과 화면
========================================================= */
function startExperienceResult() {
    if (expResultData) return;
    const amount=Math.max(0,Math.floor(pendingExpAward||0));
    const before=normalizeProgress(playerLevel,playerExp), target=buildLocalProgressAfterAward(amount);
    expResultData={beforeLevel:before.level,beforeExp:before.exp,targetLevel:target.level,targetExp:target.exp,amount,displayLevel:before.level,displayExp:before.exp,saved:true};
    expAnimation={start:performance.now(),duration:1800,done:false};
    gameState="expResult"; updateStartMenuOverlay();
    const stats=pendingExpReason==="solo"?{mode:"solo",clears:clearCount,maxStreak:maxClearStreak}:{mode:"multiplayer",result:multiplayerResult,role:multiplayerRole,clears:clearCount,maxStreak:maxClearStreak,livesRemaining:lives};
    lastExpAwardPromise=submitExperienceAward(amount,pendingExpReason,stats).then(data=>{ if(!expResultData)return; expResultData.saved=data?.saved!==false; expResultData.targetLevel=Number(data?.level??expResultData.targetLevel); expResultData.targetExp=Number(data?.exp??expResultData.targetExp); });
}
function finishExperienceResult() {
    if(!expResultData || !expAnimation?.done) return;
    setPlayerProgress(expResultData.targetLevel,expResultData.targetExp);
    closeMultiplayerSocket(); multiplayerOpen=false; multiplayerRole=null; multiplayerResult=null;
    pendingExpAward=0; pendingExpReason=""; expResultData=null; expAnimation=null; gameState="start"; setMessage(""); updateStartMenuOverlay(); updateUI();
    Promise.resolve(lastExpAwardPromise).then(()=>claimLevelRewards());
}
function updateExpAnimation(now) {
    if(gameState!=="expResult"||!expResultData||!expAnimation)return;
    const t=Math.min(1,Math.max(0,(now-expAnimation.start)/expAnimation.duration));
    const eased=1-Math.pow(1-t,3); const start=expResultData.beforeLevel, target=expResultData.targetLevel;
    let total=expResultData.beforeExp + (expResultData.targetExp + Array.from({length:Math.max(0,target-start)},(_,i)=>getLevelRequiredExp(start+i)).reduce((a,b)=>a+b,0)-expResultData.beforeExp)*eased;
    let lv=start, xp=total; while(lv<target&&xp>=getLevelRequiredExp(lv)){xp-=getLevelRequiredExp(lv);lv++;}
    expResultData.displayLevel=lv; expResultData.displayExp=Math.max(0,xp); if(t>=1){expResultData.displayLevel=target;expResultData.displayExp=expResultData.targetExp;expAnimation.done=true;setPlayerProgress(target,expResultData.targetExp);}
}
function drawExpProgressBar(x,y,w,h,level,exp){const ratio=level>=MAX_LEVEL?1:Math.max(0,Math.min(1,exp/getLevelRequiredExp(level)));ctx.fillStyle="rgba(255,255,255,.09)";ctx.beginPath();ctx.roundRect(x,y,w,h,h/2);ctx.fill();ctx.fillStyle="#63b8ff";ctx.beginPath();ctx.roundRect(x,y,w*ratio,h,h/2);ctx.fill();}
function drawExperienceResultScreen(now=performance.now()) { updateExpAnimation(now); ctx.fillStyle="#090b10";ctx.fillRect(0,0,WIDTH,HEIGHT);ctx.save();ctx.textAlign="center";ctx.textBaseline="middle";ctx.fillStyle=expResultData?.targetLevel>expResultData?.beforeLevel?"#ffd76a":"#f3f5f7";ctx.font="bold 46px Pretendard,Noto Sans KR,sans-serif";ctx.fillText(expResultData?.targetLevel>expResultData?.beforeLevel?"LEVEL UP!":"EXP 획득",WIDTH/2,140);ctx.fillStyle="#7ddcff";ctx.font="bold 30px Pretendard,Noto Sans KR,sans-serif";ctx.fillText(`+${formatExp(expResultData?.amount||0)} EXP`,WIDTH/2,215);const lv=expResultData?.displayLevel||playerLevel,xp=expResultData?.displayExp||0;ctx.fillStyle="#fff";ctx.font="bold 30px Pretendard,Noto Sans KR,sans-serif";ctx.fillText(`Lv. ${lv}`,WIDTH/2,285);drawExpProgressBar(170,330,460,22,lv,xp);ctx.fillStyle="#aeb8c4";ctx.font="600 15px Pretendard,Noto Sans KR,sans-serif";ctx.fillText(lv>=MAX_LEVEL?"MAX LEVEL":`EXP ${formatExp(xp)} / ${formatExp(getLevelRequiredExp(lv))}`,WIDTH/2,375);ctx.fillStyle="#8d98a6";ctx.font="14px Pretendard,Noto Sans KR,sans-serif";ctx.fillText(expAnimation?.done?"R / SPACE 또는 화면 터치 : 홈으로":"EXP가 올라가는 중...",WIDTH/2,490);ctx.restore(); }

/* =========================================================
   PC 키보드
========================================================= */

window.addEventListener(
    "keydown",
    event => {

        if (!gameAccessGranted) {
            return;
        }

        if (guestNameOpen) return;

        if (loadingActive) return;

        if (gamePopupOpen) {
            if (event.key === "Escape") closeGamePopup();
            return;
        }

        if (rewardListOpen) {
            if (event.key === "Escape" && !logoutConfirmOpen) closeRewardList();
            return;
        }

        const key =
            event.key.toLowerCase();

        if (energyRecoveryChoiceOpen && !event.repeat) {
            if (key === "1") {
                useEnergyRecovery(1);
                return;
            }
            if (key === "2") {
                useEnergyRecovery(2);
                return;
            }
            return;
        }

        if (
            key === "g" &&
            !event.repeat
        ) {

            event.preventDefault();

            if (
                gameState === "start"
            ) {

                if (isMultiplayerPending()) return;
                withGuestName(playGameStartSoundAndThenStart);

            } else if (
                gameState !==
                "gameover"
            ) {

                skipMap();
            }

            return;
        }

        if (
            (
                key === "r" ||
                event.code === "Space"
            ) &&
            !event.repeat
        ) {

            event.preventDefault();

            // 스페이스 더블 입력 = 더블 터치 (게임 시작 / 맵 넘기기 / 포기 등)
            if (event.code === "Space" &&
                !["gameover", "multiplayerResult", "expResult"].includes(gameState)) {
                const spaceNow = performance.now();
                if (spaceNow - lastSpacePressTime <= DOUBLE_TAP_DELAY) {
                    lastSpacePressTime = 0;
                    performDoubleAction();
                    return;
                }
                lastSpacePressTime = spaceNow;
            }

            if (gameState === "gameover") { startExperienceResult(); return; }
            if (gameState === "multiplayerResult") { startExperienceResult(); return; }
            if (gameState === "expResult") { finishExperienceResult(); return; }
            if (gameState === "multiplayerWaitingResult") { return; }

            if (false) {
                gameState = "start";
                updateStartMenuOverlay();

                settingsOpen =
                    false;

                resetRecoil();

                flash.alpha = 0;

                setMessage("");

                updateUI();
            }

            return;
        }

        if (
            gameState === "start"
        ) {

            if (
                event.repeat
            ) {
                return;
            }

            if (isMultiplayerPending()) return;

            withGuestName(playGameStartSoundAndThenStart);

            return;
        }

        if (
            gameState ===
            "gameover"
        ) {
            return;
        }

        if (
            key === "w" ||
            key === "a" ||
            key === "s" ||
            key === "d"
        ) {

            event.preventDefault();

            if (
                event.repeat
            ) {
                return;
            }

            if (
                key === "w"
            ) {
                startMove(0, -1);
            }

            if (
                key === "a"
            ) {
                startMove(-1, 0);
            }

            if (
                key === "s"
            ) {
                startMove(0, 1);
            }

            if (
                key === "d"
            ) {
                startMove(1, 0);
            }
        }
    }
);


/* =========================================================
   모바일
========================================================= */

let touchStartX = 0;
let touchStartY = 0;
let touchStartTime = 0;
let lastTapTime = 0;

const DOUBLE_TAP_DELAY = 350;
const SWIPE_MIN_DISTANCE = 25;
const TAP_MAX_DURATION = 250;


function addGameTouchListener(type, handler, options) {
    document.addEventListener(type, event => {
        const t = event.target;
        // 게임 영역 또는 게임 밖 빈 배경에서 시작된 터치만 처리 (로그인창/팝업/입력창은 제외)
        if (t === document.body || t === document.documentElement || gameWrapper.contains(t)) {
            handler(event);
        }
    }, options);
}

addGameTouchListener(
    "touchstart",
    event => {

        event.preventDefault();

        if (
            event.touches.length !== 1
        ) {
            return;
        }

        const touch =
            event.touches[0];

        touchStartX =
            touch.clientX;

        touchStartY =
            touch.clientY;

        touchStartTime =
            performance.now();

    },
    {
        passive: false
    }
);


addGameTouchListener(
    "touchmove",
    event => {


        event.preventDefault();

    },
    {
        passive: false
    }
);


addGameTouchListener(
    "touchend",
    event => {

        if (!gameAccessGranted || document.getElementById("rankingPanel")?.hidden === false) {
            return;
        }

        event.preventDefault();

        if (
            event.changedTouches.length !== 1
        ) {
            return;
        }

        const touch =
            event.changedTouches[0];

        const endX =
            touch.clientX;

        const endY =
            touch.clientY;

        const dx =
            endX -
            touchStartX;

        const dy =
            endY -
            touchStartY;

        const distance =
            Math.hypot(
                dx,
                dy
            );

        const duration =
            performance.now() -
            touchStartTime;

        if (energyRecoveryChoiceOpen) {
            if (distance < SWIPE_MIN_DISTANCE && duration <= TAP_MAX_DURATION) {
                const rect = canvas.getBoundingClientRect();
                const x = (touch.clientX - rect.left) * (WIDTH / rect.width);
                const y = (touch.clientY - rect.top) * (HEIGHT / rect.height);

                if (isInsideRect(x, y, { x: 205, y: 310, w: 160, h: 42 })) {
                    useEnergyRecovery(1);
                } else if (isInsideRect(x, y, { x: 435, y: 310, w: 160, h: 42 })) {
                    useEnergyRecovery(2);
                }
            }
            return;
        }

        if (gameState === "multiplayerResult") {
            if (distance < SWIPE_MIN_DISTANCE && duration <= TAP_MAX_DURATION) startExperienceResult();
            return;
        }
        if (gameState === "multiplayerWaitingResult") {
            // 먼저 탈락해 관전 중이어도 더블 터치로 포기할 수 있습니다.
            if (multiplayerMatchActive && !gamePopupOpen && distance < SWIPE_MIN_DISTANCE && duration <= TAP_MAX_DURATION) {
                const spectateNow = performance.now();
                if (spectateNow - lastTapTime <= DOUBLE_TAP_DELAY) {
                    lastTapTime = 0;
                    openGamePopup("multi");
                } else {
                    lastTapTime = spectateNow;
                }
            }
            return;
        }
        if (gameState === "expResult") {
            if (distance < SWIPE_MIN_DISTANCE && duration <= TAP_MAX_DURATION) finishExperienceResult();
            return;
        }

        if (
            gameState === "start"
        ) {

            if (
                performance.now() -
                lastSettingsPointerTime <
                450
            ) {

                lastTapTime = 0;

                return;
            }

            const rect =
                canvas.getBoundingClientRect();

            const x =
                (
                    touch.clientX -
                    rect.left
                ) *
                (
                    WIDTH /
                    rect.width
                );

            const y =
                (
                    touch.clientY -
                    rect.top
                ) *
                (
                    HEIGHT /
                    rect.height
                );

            // 모바일에서는 pointerup/touchend 순서와 관계없이 보상 수령을 먼저 처리합니다.
            if (questOpen && handleQuestRewardTap(x, y)) {
                lastTapTime = 0;
                lastSettingsPointerTime = performance.now();
                return;
            }

            if (
                handleSettingsTap(
                    x,
                    y
                )
            ) {
                playUIClickSound();
                lastTapTime = 0;
                return;
            }

            if (
                settingsOpen
            ) {

                lastTapTime = 0;

                return;
            }

            if (isMultiplayerPending()) { lastTapTime = 0; return; }

            const now =
                performance.now();

            if (
                now -
                lastTapTime <=
                DOUBLE_TAP_DELAY
            ) {

                lastTapTime = 0;

                withGuestName(playGameStartSoundAndThenStart);

            } else {

                lastTapTime =
                    now;
            }

            return;
        }

        if (
            gameState === "gameover"
        ) {

            if (
                distance >=
                SWIPE_MIN_DISTANCE ||
                duration >
                TAP_MAX_DURATION
            ) {

                lastTapTime = 0;

                return;
            }

            // 게임 오버 화면 → EXP 결과 화면
            startExperienceResult();
            lastTapTime = 0;
            return;
        }

        if (
            distance >=
            SWIPE_MIN_DISTANCE
        ) {

            lastTapTime = 0;

            if (
                gameState !==
                "playing" ||
                movement
            ) {
                return;
            }

            if (
                Math.abs(dx) >
                Math.abs(dy)
            ) {

                if (
                    dx > 0
                ) {

                    applyRecoil(
                        1,
                        0,
                        28,
                        2,
                        0.09
                    );

                    startMove(
                        1,
                        0
                    );

                } else {

                    applyRecoil(
                        -1,
                        0,
                        28,
                        2,
                        0.09
                    );

                    startMove(
                        -1,
                        0
                    );
                }

            } else {

                if (
                    dy > 0
                ) {

                    applyRecoil(
                        0,
                        1,
                        28,
                        2,
                        0.09
                    );

                    startMove(
                        0,
                        1
                    );

                } else {

                    applyRecoil(
                        0,
                        -1,
                        28,
                        2,
                        0.09
                    );

                    startMove(
                        0,
                        -1
                    );
                }
            }

            return;
        }

        if (
            duration >
            TAP_MAX_DURATION
        ) {

            lastTapTime = 0;

            return;
        }

        const now =
            performance.now();

        if (
            now -
            lastTapTime <=
            DOUBLE_TAP_DELAY
        ) {

            lastTapTime = 0;

            if (multiplayerMatchActive) {
                // 2인 대전: 더블 터치 → 포기 확인 창
                if (gameState !== "multiplayerResult") openGamePopup("multi");
            } else if (
                gameState !== "gameover" &&
                gameState !== "multiplayerWaitingRound" &&
                gameState !== "multiplayerWaitingResult" &&
                gameState !== "multiplayerResult"
            ) {
                if (!useSecondPathGuide()) {
                    skipMap();
                }
            }

        } else {

            lastTapTime =
                now;
        }

    },
    {
        passive: false
    }
);



/* =========================================================
   레벨 보상 수령 (서버가 보상표/수령 여부를 관리)
========================================================= */
let lastExpAwardPromise = null;
let levelRewardClaiming = false;

function showLevelRewardModal(entries, coinsGained, itemsGained) {
    const overlay = document.getElementById("levelRewardOverlay");
    if (!overlay) return;

    const first = entries[0].level;
    const last = entries[entries.length - 1].level;
    document.getElementById("levelRewardSubtitle").textContent =
        first === last ? `Lv.${last} 달성 보상이 지급되었습니다!` : `Lv.${first} ~ Lv.${last} 달성 보상이 지급되었습니다!`;

    const rows = [];
    if (last >= MAX_LEVEL) rows.push(`<div class="level-reward-row special">🏆 최고 레벨 달성을 축하합니다!</div>`);
    if (coinsGained > 0) rows.push(`<div class="level-reward-row">🪙 코인 +${coinsGained.toLocaleString("ko-KR")}</div>`);
    Object.keys(ITEM_DATA).forEach(type => {
        const amount = itemsGained[type] || 0;
        if (amount > 0) rows.push(`<div class="level-reward-row">${ITEM_DATA[type].icon} ${escapeHTML(ITEM_DATA[type].name)} ×${amount}</div>`);
    });
    document.getElementById("levelRewardList").innerHTML = rows.join("");

    overlay.classList.add("visible");
    overlay.setAttribute("aria-hidden", "false");
}

function closeLevelRewardModal() {
    const overlay = document.getElementById("levelRewardOverlay");
    if (!overlay) return;
    overlay.classList.remove("visible");
    overlay.setAttribute("aria-hidden", "true");
}

document.getElementById("levelRewardOkButton")?.addEventListener("click", () => {
    playUIClickSound();
    closeLevelRewardModal();
});

async function claimLevelRewards() {
    if (!currentAccount || guestMode || !gameAccessGranted || levelRewardClaiming) return;
    levelRewardClaiming = true;

    try {
        const data = await apiJSON("/api/progress/claim-rewards", { method: "POST", body: "{}" });
        const entries = Array.isArray(data?.entries) ? data.entries : [];
        if (!entries.length) return;

        let coinsGained = 0;
        const itemsGained = {};

        for (const entry of entries) {
            coinsGained += Math.max(0, Math.floor(Number(entry.coins) || 0));
            for (const [type, count] of Object.entries(entry.items || {})) {
                if (!Object.prototype.hasOwnProperty.call(itemInventory, type)) continue;
                const amount = Math.max(0, Math.floor(Number(count) || 0));
                itemInventory[type] += amount;
                itemsGained[type] = (itemsGained[type] || 0) + amount;
            }
        }

        coins += coinsGained;
        saveCoins();
        saveItemInventory();
        updateUI();
        showLevelRewardModal(entries, coinsGained, itemsGained);
    } catch (error) {
        console.warn("레벨 보상 수령 실패", error);
    } finally {
        levelRewardClaiming = false;
    }
}

/* =========================================================
   레벨 보상표 (프로필 박스 클릭)
   - 서버 GET /api/progress/rewards 로 Lv.2~100 보상을 받아 표시합니다.
========================================================= */
let rewardListOpen = false;

function renderRewardList(data) {
    const body = document.getElementById("rewardListBody");
    const subtitle = document.getElementById("rewardListSubtitle");
    if (!body) return;

    const level = Math.max(1, Number(data?.level) || playerLevel || 1);
    const maxLevel = Number(data?.maxLevel) || MAX_LEVEL;
    const rewards = Array.isArray(data?.rewards) ? data.rewards : [];

    const need = level >= maxLevel ? 0 : (Number(data?.requiredExp) || getLevelRequiredExp(level));
    const exp = level >= maxLevel ? 0 : Math.max(0, Math.min(need, Number(data?.exp ?? playerExp) || 0));
    const frac = level >= maxLevel || need <= 0 ? 1 : Math.max(0, Math.min(1, exp / need));

    if (subtitle) {
        subtitle.textContent = level >= maxLevel
            ? "최고 레벨에 도달했습니다! 🏆"
            : `Lv.${level} → Lv.${level + 1} · EXP ${formatExp(exp)} / ${formatExp(need)} (${Math.floor(frac * 100)}%)`;
    }

    if (!rewards.length) {
        body.innerHTML = `<div class="reward-list-message">표시할 보상이 없습니다.</div>`;
        return;
    }

    // 아래(Lv.1)에서 위(Lv.100)로 올라가도록 높은 레벨을 위쪽에 둡니다.
    const entries = [{ level: 1, start: true }, ...rewards].sort((a, b) => b.level - a.level);

    const rowsHTML = entries.map(entry => {
        const lv = Number(entry.level) || 0;
        let cls = "reward-list-row";
        let state = "";
        let inner = "";

        if (entry.start) {
            cls += " start done";
            state = lv === level ? "현재 레벨" : "시작";
            inner = `<span>여기서 시작해요</span>`;
        } else {
            const coinsAmount = Math.max(0, Math.floor(Number(entry.coins) || 0));
            const parts = [];
            if (coinsAmount > 0) parts.push(`<span>🪙 +${coinsAmount.toLocaleString("ko-KR")}</span>`);
            Object.keys(ITEM_DATA).forEach(type => {
                const amount = Math.max(0, Math.floor(Number((entry.items || {})[type]) || 0));
                if (amount > 0) parts.push(`<span>${ITEM_DATA[type].icon} ${escapeHTML(ITEM_DATA[type].name)} ×${amount}</span>`);
            });
            if (entry.special) { parts.unshift(`<span>🏆 최고 레벨 보상</span>`); cls += " special"; }
            inner = parts.join("");

            if (lv < level) { cls += " done"; state = "달성 ✓"; }
            else if (lv === level) { cls += " done current"; state = "현재 레벨"; }
            else if (lv === level + 1) { cls += " next"; state = "다음 보상"; }
        }
        if (entry.start && lv === level) cls += " current";

        return `<div class="${cls}" data-level="${lv}"><span class="reward-list-level">Lv.${lv}</span><span class="reward-list-items">${inner}</span><span class="reward-list-state">${state}</span></div>`;
    }).join("");

    body.innerHTML = `<div class="reward-track" id="rewardTrack">${rowsHTML}</div>`;

    const track = document.getElementById("rewardTrack");
    const layoutGauge = () => {
        const rows = Array.from(track.querySelectorAll(".reward-list-row"));
        if (rows.length < 2) return;

        const centerOf = row => row.offsetTop + row.offsetHeight / 2;
        const centers = new Map(rows.map(row => [Number(row.dataset.level), centerOf(row)]));
        const yTop = centers.get(entries[0].level);                 // 가장 높은 레벨(위쪽)
        const yBottom = centers.get(1);                             // Lv.1(아래쪽)

        track.querySelectorAll(".reward-gauge,.reward-tick,.reward-now").forEach(el => el.remove());

        const gauge = document.createElement("div");
        gauge.className = "reward-gauge";
        gauge.style.top = `${yTop}px`;
        gauge.style.height = `${yBottom - yTop}px`;

        // 현재 레벨 위치에서 다음 레벨 위치까지 EXP 비율만큼 채웁니다.
        const yCurrent = centers.get(level);
        const yNext = centers.has(level + 1) ? centers.get(level + 1) : yCurrent;
        const yFill = yCurrent - (yCurrent - yNext) * frac;

        const fill = document.createElement("div");
        fill.className = "reward-gauge-fill";
        fill.style.height = `${Math.max(0, yBottom - yFill)}px`;
        gauge.appendChild(fill);
        track.appendChild(gauge);

        // 레벨 선: 모든 레벨 위치에 눈금, 5레벨마다 굵은 눈금
        centers.forEach((y, lv) => {
            const tick = document.createElement("div");
            tick.className = "reward-tick" + (lv <= level ? " reached" : "") + (lv % 5 === 0 ? " big" : "");
            tick.style.top = `${y}px`;
            track.appendChild(tick);
        });

        // 현재 EXP 위치 표시
        const now = document.createElement("div");
        now.className = "reward-now";
        now.style.top = `${yFill}px`;
        track.appendChild(now);

        // 다음 레벨(진행 중인 구간)이 화면 중앙에 오도록 스크롤
        const focus = track.querySelector(`.reward-list-row[data-level="${level >= maxLevel ? level : level + 1}"]`);
        if (focus) {
            body.scrollTop = Math.max(0, focus.offsetTop - body.clientHeight / 2 + focus.offsetHeight / 2);
        }
    };

    layoutGauge();
    requestAnimationFrame(layoutGauge);   // 폰트 로드 등으로 높이가 바뀌는 경우 한 번 더 맞춤
}

const NICKNAME_CHANGE_COST = 100;
let profileTab = "stats";
let rewardListData = null, rewardListError = "";
let profileStatsData = null, profileStatsError = "";
let profileLoading = false;
let nicknameChanging = false;
let nicknameNotice = null;   // { text, type }

function formatPlayTime(totalSeconds) {
    const sec = Math.max(0, Math.floor(Number(totalSeconds) || 0));
    const h = Math.floor(sec / 3600);
    const m = Math.floor((sec % 3600) / 60);
    const s = sec % 60;
    if (h > 0) return `${h}시간 ${m}분`;
    if (m > 0) return `${m}분 ${s}초`;
    return `${s}초`;
}

function formatRemainKo(ms) {
    const total = Math.max(1, Math.ceil(ms / 60000));
    const h = Math.floor(total / 60);
    const m = total % 60;
    return h > 0 ? `${h}시간 ${m}분` : `${m}분`;
}

const RECORD_RESET_COST = 100;
let recordResetting = false;
let recordNotice = { solo: null, multiplayer: null };

function formatAvg(value) {
    if (value === null || value === undefined || !Number.isFinite(Number(value))) return "-";
    return Number(value).toLocaleString("ko-KR", { maximumFractionDigits: 1 });
}

function renderProfileStats() {
    const body = document.getElementById("rewardListBody");
    const subtitle = document.getElementById("rewardListSubtitle");
    if (!body) return;
    if (subtitle) subtitle.textContent = "내 활동 기록";

    if (profileLoading) {
        body.innerHTML = `<div class="reward-list-message">불러오는 중...</div>`;
        return;
    }
    const d = profileStatsData;
    if (!d) {
        body.innerHTML = `<div class="reward-list-message">${escapeHTML(profileStatsError || "내 정보를 불러오지 못했습니다.")}</div>`;
        return;
    }

    const rate = d.winRate == null ? "-" : `${d.winRate}%`;
    const nextMs = d.nextNicknameChangeAt ? new Date(d.nextNicknameChangeAt).getTime() - Date.now() : 0;
    const cooling = nextMs > 0;

    let note = nicknameNotice;
    if (!note) {
        note = cooling
            ? { text: `다음 변경까지 ${formatRemainKo(nextMs)} 남았어요.`, type: "" }
            : { text: `변경 후 24시간 동안은 다시 바꿀 수 없어요. · 보유 🪙 ${coins}`, type: "" };
    }

    const resetNote = scope => recordNotice[scope] || { text: `초기화하면 되돌릴 수 없어요. · 보유 🪙 ${coins}`, type: "" };
    const soloNote = resetNote("solo");
    const mpNote = resetNote("multiplayer");
    const num = v => Math.max(0, Number(v) || 0).toLocaleString("ko-KR");

    body.innerHTML = `
        <div class="profile-section-title">🎮 개인 도전 기록</div>
        <div class="profile-stat-grid">
            <div class="profile-stat"><span>게임 도전 횟수</span><b>${num(d.playCount)}회</b></div>
            <div class="profile-stat"><span>총 플레이 시간</span><b>${escapeHTML(formatPlayTime(d.playSeconds))}</b></div>
            <div class="profile-stat"><span>평균 점수</span><b>${formatAvg(d.soloAvgScore)}${d.soloAvgScore == null ? "" : "점"}</b></div>
            <div class="profile-stat"><span>평균 클리어 횟수</span><b>${formatAvg(d.soloAvgClears)}${d.soloAvgClears == null ? "" : "회"}</b></div>
            <div class="profile-stat wide"><span>평균 연속 클리어 기록</span><b>${formatAvg(d.soloAvgStreak)}${d.soloAvgStreak == null ? "" : "회"}</b></div>
        </div>
        <div class="profile-reset-box">
            <button id="profileResetSoloButton" type="button">🗑 개인 기록 초기화 (🪙 ${RECORD_RESET_COST})</button>
            <div class="profile-nick-note ${soloNote.type || ""}">${escapeHTML(soloNote.text)}</div>
        </div>

        <div class="profile-section-title">⚔ 2인 대전 기록</div>
        <div class="profile-stat-grid">
            <div class="profile-stat win"><span>2인 대전 승리</span><b>${num(d.mpWins)}승</b></div>
            <div class="profile-stat loss"><span>2인 대전 패배</span><b>${num(d.mpLosses)}패</b></div>
            <div class="profile-stat rate"><span>2인 대전 승률</span><b>${rate}</b></div>
            <div class="profile-stat"><span>대전 플레이 시간</span><b>${escapeHTML(formatPlayTime(d.mpSeconds))}</b></div>
            <div class="profile-stat"><span>평균 점수</span><b>${formatAvg(d.mpAvgScore)}${d.mpAvgScore == null ? "" : "점"}</b></div>
            <div class="profile-stat"><span>평균 클리어 횟수</span><b>${formatAvg(d.mpAvgClears)}${d.mpAvgClears == null ? "" : "회"}</b></div>
            <div class="profile-stat wide"><span>평균 연속 클리어 기록</span><b>${formatAvg(d.mpAvgStreak)}${d.mpAvgStreak == null ? "" : "회"}</b></div>
        </div>
        <div class="profile-reset-box">
            <button id="profileResetMpButton" type="button">🗑 2인 대전 기록 초기화 (🪙 ${RECORD_RESET_COST})</button>
            <div class="profile-nick-note ${mpNote.type || ""}">${escapeHTML(mpNote.text)}</div>
        </div>

        <div class="profile-section-title">✏️ 닉네임 변경</div>
        <div class="profile-nick-box">
            <div class="profile-nick-current">현재 닉네임 <b>${escapeHTML(d.nickname)}</b></div>
            <input id="profileNicknameInput" type="text" maxlength="16" placeholder="새 닉네임 (2~16자)" autocomplete="off" ${cooling ? "disabled" : ""}>
            <button id="profileNicknameButton" type="button" ${cooling ? "disabled" : ""}>🪙 ${NICKNAME_CHANGE_COST} 코인으로 변경</button>
            <div class="profile-nick-note ${note.type || ""}">${escapeHTML(note.text)}</div>
        </div>`;

    document.getElementById("profileResetSoloButton")?.addEventListener("click", () => requestRecordReset("solo"));
    document.getElementById("profileResetMpButton")?.addEventListener("click", () => requestRecordReset("multiplayer"));
    document.getElementById("profileNicknameButton")?.addEventListener("click", changeNickname);
    document.getElementById("profileNicknameInput")?.addEventListener("keydown", event => {
        if (event.key === "Enter") { event.preventDefault(); changeNickname(); }
    });
}

// 기록 초기화: 코인 100 소모 + 최종 확인창. 서버에서 초기화가 확정된 뒤에만 코인을 차감합니다.
async function requestRecordReset(scope) {
    if (recordResetting || logoutConfirmOpen || !profileStatsData) return;

    const isSolo = scope === "solo";
    const label = isSolo ? "개인 도전 기록" : "2인 대전 기록";
    const fail = text => {
        recordNotice[scope] = { text, type: "error" };
        playUIInvalidSound();
        renderProfileStats();
    };

    if (coins < RECORD_RESET_COST) {
        return fail(`코인이 부족합니다. (필요 ${RECORD_RESET_COST} / 보유 ${coins})`);
    }

    const ok = await openLogoutConfirm({
        title: `${label} 초기화`,
        message: (isSolo
            ? "게임 도전 횟수 · 총 플레이 시간 ·\n평균 점수/클리어/연속 클리어 기록이 모두 0으로 돌아갑니다.\n"
            : "2인 대전 승/패 · 승률 · 대전 플레이 시간 ·\n평균 점수/클리어/연속 클리어 기록이 모두 0으로 돌아갑니다.\n") +
            `\n🪙 ${RECORD_RESET_COST}코인이 소모되며 되돌릴 수 없습니다.\n정말 초기화할까요?`,
        confirmLabel: "초기화"
    });
    if (!ok || !rewardListOpen || recordResetting) return;

    if (coins < RECORD_RESET_COST) {
        return fail(`코인이 부족합니다. (필요 ${RECORD_RESET_COST} / 보유 ${coins})`);
    }

    recordResetting = true;
    document.querySelectorAll(".profile-reset-box button").forEach(btn => { btn.disabled = true; });

    try {
        const data = await apiJSON("/api/profile/reset", {
            method: "POST",
            body: JSON.stringify({ scope })
        });

        coins = Math.max(0, coins - RECORD_RESET_COST);
        saveCoins();
        if (data?.profile) profileStatsData = data.profile;

        recordNotice[scope] = { text: `${label}이 초기화되었어요! (🪙 -${RECORD_RESET_COST})`, type: "success" };
        updateUI();
    } catch (error) {
        recordNotice[scope] = { text: error?.message || "기록을 초기화하지 못했습니다.", type: "error" };
    } finally {
        recordResetting = false;
        if (rewardListOpen && profileTab === "stats") renderProfileStats();
    }
}

async function changeNickname() {
    if (nicknameChanging || !profileStatsData) return;

    const input = document.getElementById("profileNicknameInput");
    const nickname = (input?.value || "").trim();
    const fail = text => {
        nicknameNotice = { text, type: "error" };
        playUIInvalidSound();
        renderProfileStats();
    };

    if (nickname.length < 2 || nickname.length > 16) return fail("닉네임은 2~16자로 입력해주세요.");
    if (nickname === profileStatsData.nickname) return fail("현재 닉네임과 같습니다.");
    if (coins < NICKNAME_CHANGE_COST) return fail(`코인이 부족합니다. (필요 ${NICKNAME_CHANGE_COST} / 보유 ${coins})`);

    if (!window.confirm(`🪙 ${NICKNAME_CHANGE_COST}코인을 사용해 닉네임을 "${nickname}"(으)로 변경할까요?\n변경 후 24시간 동안은 다시 바꿀 수 없습니다.`)) return;

    nicknameChanging = true;
    const button = document.getElementById("profileNicknameButton");
    if (button) button.disabled = true;

    try {
        const data = await apiJSON("/api/profile/nickname", {
            method: "POST",
            body: JSON.stringify({ nickname })
        });

        // 서버에서 변경이 확정된 뒤에만 코인을 차감합니다.
        coins = Math.max(0, coins - NICKNAME_CHANGE_COST);
        saveCoins();

        profileStatsData.nickname = data.nickname;
        profileStatsData.nicknameChangedAt = data.nicknameChangedAt;
        profileStatsData.nextNicknameChangeAt = data.nextNicknameChangeAt;
        if (currentAccount) currentAccount.nickname = data.nickname;

        nicknameNotice = { text: `닉네임이 "${data.nickname}"(으)로 변경되었습니다!`, type: "success" };
        updateStartMenuOverlay();
        updateUI();
        if (profileTab === "stats" && rewardListOpen) renderProfileStats();
    } catch (error) {
        nicknameNotice = { text: error?.message || "닉네임을 변경하지 못했습니다.", type: "error" };
        if (rewardListOpen) renderProfileStats();
    } finally {
        nicknameChanging = false;
    }
}

function renderProfileTab() {
    document.getElementById("profileTabStats")?.classList.toggle("active", profileTab === "stats");
    document.getElementById("profileTabRewards")?.classList.toggle("active", profileTab === "rewards");

    if (profileTab === "stats") {
        renderProfileStats();
        return;
    }

    const body = document.getElementById("rewardListBody");
    const subtitle = document.getElementById("rewardListSubtitle");
    if (profileLoading) {
        if (subtitle) subtitle.textContent = "";
        if (body) body.innerHTML = `<div class="reward-list-message">불러오는 중...</div>`;
    } else if (rewardListData) {
        renderRewardList(rewardListData);
    } else {
        if (subtitle) subtitle.textContent = "";
        if (body) body.innerHTML = `<div class="reward-list-message">${escapeHTML(rewardListError || "레벨 보상표를 불러오지 못했습니다.")}</div>`;
    }
}

function setProfileTab(tab) {
    profileTab = tab === "rewards" ? "rewards" : "stats";
    if (rewardListOpen) renderProfileTab();
}

async function openRewardList() {
    if (!currentAccount || guestMode) {
        window.alert("게스트 모드에서는 프로필을 볼 수 없습니다. 회원으로 로그인해 주세요.");
        return;
    }
    if (rewardListOpen) return;

    const overlay = document.getElementById("rewardListOverlay");
    if (!overlay) return;

    rewardListOpen = true;
    profileLoading = true;
    profileTab = "stats";
    nicknameNotice = null;
    recordNotice = { solo: null, multiplayer: null };
    rewardListData = null; rewardListError = "";
    profileStatsData = null; profileStatsError = "";

    overlay.classList.add("visible");
    overlay.setAttribute("aria-hidden", "false");
    renderProfileTab();

    const [statsResult, rewardsResult] = await Promise.allSettled([
        apiJSON("/api/profile/stats"),
        apiJSON("/api/progress/rewards")
    ]);
    if (!rewardListOpen) return;   // 불러오는 사이에 닫은 경우

    if (statsResult.status === "fulfilled") profileStatsData = statsResult.value;
    else profileStatsError = statsResult.reason?.message || "";
    if (rewardsResult.status === "fulfilled") rewardListData = rewardsResult.value;
    else rewardListError = rewardsResult.reason?.message || "";

    profileLoading = false;
    renderProfileTab();
}

document.getElementById("profileTabStats")?.addEventListener("click", () => { playUIClickSound(); setProfileTab("stats"); });
document.getElementById("profileTabRewards")?.addEventListener("click", () => { playUIClickSound(); setProfileTab("rewards"); });

function closeRewardList() {
    const overlay = document.getElementById("rewardListOverlay");
    rewardListOpen = false;
    if (!overlay) return;
    overlay.classList.remove("visible");
    overlay.setAttribute("aria-hidden", "true");
}

(function bindRewardListUI() {
    const box = document.getElementById("startMenuAccount");
    if (box) {
        // 시작 화면의 더블 터치/스와이프 처리로 이벤트가 넘어가지 않게 막습니다.
        ["pointerdown", "pointerup", "touchstart", "touchend"].forEach(type => {
            box.addEventListener(type, event => event.stopPropagation(), { passive: true });
        });
        box.addEventListener("click", event => {
            event.preventDefault();
            event.stopPropagation();
            playUIClickSound();
            openRewardList();
        });
    }

    document.getElementById("rewardListCloseButton")?.addEventListener("click", () => {
        playUIClickSound();
        closeRewardList();
    });

    const overlay = document.getElementById("rewardListOverlay");
    overlay?.addEventListener("click", event => {
        if (event.target === overlay) closeRewardList();
    });
})();

// 로그인/자동 로그인 직후에도 아직 받지 않은 레벨 보상이 있으면 지급합니다.
const refreshPlayerProgressBase = refreshPlayerProgress;
refreshPlayerProgress = async function () {
    await refreshPlayerProgressBase();
    await claimLevelRewards();
};

/* =========================================================
   튜토리얼
   - 코인, 점수, 일일 퀘스트, 랭킹, 아이템에 어떤 기록도 남기지 않습니다.
   - gameState "tutorial" 전용 상태에서만 동작합니다.
========================================================= */
const TUTORIAL_MAP_ROWS = [
"####################",
"#S.X..X##..#######.#",
"#...##.##.##....##.#",
"###.##..#.##.#.###.#",
"###.##X..X###.####.#",
"###.G###......####.#",
"#.##.###.#######.#.#",
"#...##...##...####.#",
"####..#..#.#####.#.#",
"##################.#",
"######.#########.#.#",
"##..#.....######.#.#",
"##..##.....#######.#",
"#..................#",
"####################"
];

const TUTORIAL_STEPS = [
    { type: "info", title: "슬라이딩 튜토리얼", lines: [
        "초록 블록을 움직여 목표에 도착하는 게임이에요.",
        "기본 조작과 규칙을 직접 해보며 알려드릴게요.",
        "튜토리얼은 코인 · 점수 · 퀘스트 · 랭킹에",
        "아무 영향도 주지 않아요. 부담 없이 해보세요!"
    ] },
    { type: "move", title: "이동하기", need: 5,
      text: "WASD 또는 스와이프로 5번 이동해 보세요! (벽에 닿을 때까지 미끄러져요)" },
    { type: "danger", title: "위험 블록",
      text: "빨간 위험 블록에 부딪혀 보세요! 닿으면 목숨이 1개 줄어요. (튜토리얼이라 게임 오버는 없어요)" },
    { type: "goal", title: "목표 도달",
      text: "위험 블록을 피해 파란 목표 블록에 멈추면 클리어! 위험 블록에 닿으면 목숨이 줄고 처음 위치로 돌아가요." },
    { type: "skip", title: "맵 넘기기",
      text: "막힐 땐 G키 또는 화면 더블 터치로 맵을 넘겨 보세요! 넘길 때마다 맵 넘기기 횟수가 1개 줄어요." },
    { type: "info", title: "시간 · 목숨 · 점수", lines: [
        "맵마다 제한 시간이 있고, 0초가 되면 목숨을 잃어요.",
        "목숨은 3개! 모두 잃으면 게임 오버예요.",
        "클리어할 때마다 코인 1개를 얻어요.",
        "연속 클리어는 점수 보너스! 맵 넘기기 · 목숨 손실은 감점이에요.",
        "클리어가 쌓일수록 제한 시간이 점점 줄어들어요."
    ] },
    { type: "info", title: "아이템 · 코인 · 레벨", lines: [
        "코인으로 🛒 상점에서 아이템을 사고, 🎒 인벤토리에서 장착해요.",
        "시계 · 보호막 · 경로 안내 · 응급 처치 · 에너지 복구가 있어요.",
        "📜 일일 퀘스트를 완료하면 코인 보상을 받아요.",
        "게임이 끝나면 EXP를 얻고, 레벨업하면 보상을 받아요! (최고 Lv.100)",
        "⚔ 2인 대전에서 친구와 실력을 겨뤄 보세요!"
    ] },
    { type: "info", title: "튜토리얼 완료!", last: true, lines: [
        "이제 준비됐어요!",
        "홈에서 더블 터치 또는 키 입력으로 게임을 시작해 보세요.",
        "행운을 빌어요!"
    ] }
];

let tutorialActive = false;
let tutorialStep = 0;
let tutorialMoves = 0;
let tutorialLocked = false;
let tutorialNotice = "";
let tutorialNoticeUntil = 0;
let tutorialAdvanceTimer = null;
let tutorialExitConfirming = false;
let tutorialMapData = null;
let lastTutorialTapTime = 0;
let tutorialStepStartedAt = 0;
let tutorialAwaitingNext = false;   // 미션 완료 후 "터치하면 다음으로" 대기 중
let tutorialCompletedAt = 0;
let tutorialSavedLives = null;
let tutorialSavedSkips = null;
const TUTORIAL_INFO_DELAY_MS = 3000;
let tutorialPointerDown = { x: 0, y: 0 };
const TUTORIAL_EXIT_BUTTON = { x: 696, y: 6, w: 92, h: 28 };
const TUTORIAL_NEXT_BUTTON = { x: 300, y: 392, w: 200, h: 46 };

function parseTutorialMap() {
    if (tutorialMapData) return tutorialMapData;
    const wallSet = new Set();
    const dangerSet = new Set();
    let goalCell = null;

    TUTORIAL_MAP_ROWS.forEach((row, r) => {
        for (let c = 0; c < COLS; c++) {
            const ch = row[c];
            if (ch === "#") wallSet.add(keyOf(c, r));
            else if (ch === "G") goalCell = { c, r };
            else if (ch === "X") dangerSet.add(keyOf(c, r));
        }
    });

    tutorialMapData = { walls: wallSet, dangers: dangerSet, goal: goalCell };
    return tutorialMapData;
}

// 설명 창은 3초가 지나야 넘길 수 있습니다. (남은 시간을 ms로 반환)
function tutorialNextWaitMs() {
    return Math.max(0, TUTORIAL_INFO_DELAY_MS - (performance.now() - tutorialStepStartedAt));
}

function wrapTutorialText(text, maxWidth) {
    const lines = [];
    let line = "";
    for (const ch of String(text)) {
        const candidate = line + ch;
        if (ctx.measureText(candidate).width > maxWidth && line) {
            lines.push(line.trimEnd());
            line = ch === " " ? "" : ch;
        } else {
            line = candidate;
        }
    }
    if (line) lines.push(line);
    return lines;
}

function setTutorialNotice(text, ms = 2200) {
    tutorialNotice = text;
    tutorialNoticeUntil = performance.now() + ms;
}

function setupTutorialStep(index) {
    clearTimeout(tutorialAdvanceTimer);
    tutorialStep = index;
    tutorialMoves = 0;
    tutorialLocked = false;
    tutorialAwaitingNext = false;
    tutorialNotice = "";
    tutorialNoticeUntil = 0;

    tutorialStepStartedAt = performance.now();
    const step = TUTORIAL_STEPS[index];
    const data = parseTutorialMap();
    stageStart = { c: START.c, r: START.r };
    movement = null;

    if (step.type === "move") {
        dangers = new Set();
        goal = null;
        resetPlayer();
    } else if (step.type === "danger") {
        dangers = new Set(data.dangers);
        goal = null;
        resetPlayer();
    } else if (step.type === "goal" || step.type === "skip") {
        dangers = new Set(data.dangers);
        goal = { c: data.goal.c, r: data.goal.r };
        resetPlayer();
    }
}

function startTutorial() {
    if (!gameAccessGranted || gameState !== "start" || tutorialActive) return;

    const data = parseTutorialMap();
    tutorialActive = true;
    tutorialSavedLives = lives;
    tutorialSavedSkips = mapSkips;
    lives = MAX_LIVES;
    mapSkips = MAX_MAP_SKIPS;
    clearTimeout(roundTimer);
    settingsOpen = false;
    questOpen = false;
    shopOpen = false;
    inventoryOpen = false;
    skinOpen = false;

    const oldWalls = new Set(walls);
    walls = new Set(data.walls);
    beginMapTransition(oldWalls, walls);
    gameState = "tutorial";

    resetRecoil();
    flash.alpha = 0;
    trail = [];
    setMessage("");
    setupTutorialStep(0);
    updateStartMenuOverlay();
    updateUI();
}

function exitTutorial() {
    clearTimeout(tutorialAdvanceTimer);
    tutorialActive = false;
    tutorialLocked = false;
    tutorialAwaitingNext = false;
    if (tutorialSavedLives !== null) lives = tutorialSavedLives;
    if (tutorialSavedSkips !== null) mapSkips = tutorialSavedSkips;
    tutorialSavedLives = null;
    tutorialSavedSkips = null;
    movement = null;
    trail = [];
    mapTransition.active = false;
    dangers = new Set();
    goal = null;
    stageStart = { c: START.c, r: START.r };
    resetPlayer();
    setMessage("");
    flash.alpha = 0;
    resetRecoil();
    shake.power = 0;
    shake.time = 0;
    gameState = "start";
    updateStartMenuOverlay();
    updateUI();
}

function tutorialAdvance() {
    if (!tutorialActive) return;
    if (tutorialStep >= TUTORIAL_STEPS.length - 1) {
        exitTutorial();
        return;
    }
    setupTutorialStep(tutorialStep + 1);
}

// 미션 완료: 자동으로 넘어가지 않고, 터치(클릭/Space/Enter)하면 다음 단계로 넘어갑니다.
function tutorialComplete(message) {
    tutorialLocked = true;
    tutorialAwaitingNext = true;
    tutorialCompletedAt = performance.now();
    movement = null;
    tutorialNotice = message;
    tutorialNoticeUntil = Infinity;
    clearTimeout(tutorialAdvanceTimer);
}

// 튜토리얼 전용 목숨 감소 (목숨이 0이 되면 다시 채워서 게임 오버가 없게 함)
function tutorialLoseLife() {
    lives--;
    let refilled = false;
    if (lives <= 0) {
        lives = MAX_LIVES;
        refilled = true;
    }
    updateUI();
    return refilled;
}

function tutorialCheckTile() {
    const step = TUTORIAL_STEPS[tutorialStep];
    if (!step || tutorialLocked) return;

    if (step.type === "move") {
        tutorialMoves++;
        if (tutorialMoves >= step.need) {
            tutorialComplete("좋아요! 이동을 익혔어요.");
        } else {
            setTutorialNotice(`이동 ${tutorialMoves}/${step.need}`, 1500);
        }
        return;
    }

    if (dangers.has(keyOf(player.c, player.r))) {
        applyImpactRecoil(190, 14, 0.40);
        flash.color = "#ff3e4d";
        flash.alpha = 0.32;

        const refilled = tutorialLoseLife();

        if (step.type === "danger") {
            tutorialComplete(`위험 블록에 닿았어요! 목숨이 1개 줄었어요. (남은 목숨 ${lives}개)`);
        } else {
            setTutorialNotice(
                refilled
                    ? "목숨이 모두 사라졌지만 튜토리얼이라 다시 채워졌어요. 처음 위치로 돌아갑니다."
                    : `위험 블록! 목숨이 1개 줄었어요. (남은 목숨 ${lives}개) 처음 위치로 돌아갑니다.`,
                2800
            );
            resetPlayer();
        }
        return;
    }

    if (step.type === "goal" && goal && player.c === goal.c && player.r === goal.r) {
        playEffectSound("goal");
        applyImpactRecoil(150, 12, 0.32);
        flash.color = "#63ff91";
        flash.alpha = 0.25;
        tutorialComplete("클리어! 실제 게임에서는 코인 1개를 얻어요.");
    }
}

function tutorialSkipAction() {
    const step = TUTORIAL_STEPS[tutorialStep];
    if (!tutorialActive || !step || step.type === "info" || tutorialLocked) return;

    // 단계 시작 직후의 연타(더블 터치)는 무시합니다.
    if (performance.now() - tutorialStepStartedAt < 600) return;

    if (step.type !== "skip") {
        setTutorialNotice("맵 넘기기는 뒤에서 해 볼 거예요.", 1600);
        return;
    }

    if (mapSkips <= 0) {
        setTutorialNotice("맵 넘기기 횟수가 없어요.", 1600);
        return;
    }

    mapSkips--;
    updateUI();

    // 실제 맵 생성기를 사용하되, 최근 맵 기록에는 남기지 않습니다.
    const layoutCount = previousLayouts.length;
    movement = null;
    stageStart = { c: START.c, r: START.r };
    resetPlayer();
    createMapWithSeed(20260101);
    previousLayouts.length = layoutCount;
    gameState = "tutorial";

    applyImpactRecoil(90, 5, 0.18);
    flash.color = "#b995ff";
    flash.alpha = 0.12;
    tutorialComplete(`맵이 바뀌었어요! 맵 넘기기 횟수가 1개 줄었어요. (남은 횟수 ${mapSkips}회)`);
}

async function requestTutorialExit() {
    if (tutorialExitConfirming || !tutorialActive) return;
    tutorialExitConfirming = true;
    try {
        const ok = await openLogoutConfirm({
            title: "튜토리얼 종료",
            message: "튜토리얼을 종료하고 홈으로 돌아갈까요?",
            confirmLabel: "종료"
        });
        if (ok && tutorialActive) exitTutorial();
    } finally {
        tutorialExitConfirming = false;
    }
}

function handleTutorialTap(x, y) {
    if (!tutorialActive || gameState !== "tutorial") return false;

    if (isInsideRect(x, y, TUTORIAL_EXIT_BUTTON)) {
        playUIClickSound();
        requestTutorialExit();
        return true;
    }

    if (tutorialAwaitingNext) {
        // 완료 직후 같은 터치로 바로 넘어가는 것을 방지
        if (performance.now() - tutorialCompletedAt < 500) return true;
        playUIClickSound();
        tutorialAdvance();
        return true;
    }

    const step = TUTORIAL_STEPS[tutorialStep];
    if (step && step.type === "info" && isInsideRect(x, y, TUTORIAL_NEXT_BUTTON)) {
        if (tutorialNextWaitMs() > 0) {
            playUIInvalidSound();
            return true;
        }
        playUIClickSound();
        tutorialAdvance();
        return true;
    }

    return false;
}

function drawTutorialOverlay() {
    const step = TUTORIAL_STEPS[tutorialStep];
    if (!step) return;

    const now = performance.now();
    const isInfo = step.type === "info";

    ctx.save();
    ctx.textBaseline = "middle";

    if (isInfo) {
        ctx.fillStyle = "rgba(0,0,0,0.76)";
        ctx.fillRect(0, 0, WIDTH, HEIGHT);

        const card = { x: 90, y: 90, w: 620, h: 380 };
        ctx.fillStyle = "#171c25";
        ctx.strokeStyle = "#394352";
        ctx.lineWidth = 2;
        ctx.beginPath();
        ctx.roundRect(card.x, card.y, card.w, card.h, 20);
        ctx.fill();
        ctx.stroke();

        ctx.textAlign = "center";
        ctx.fillStyle = "#ffffff";
        ctx.font = "bold 28px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(step.title, WIDTH / 2, 145);

        ctx.fillStyle = "#c5ced8";
        ctx.font = "17px Pretendard, Noto Sans KR, sans-serif";
        step.lines.forEach((line, i) => {
            ctx.fillText(line, WIDTH / 2, 208 + i * 33);
        });

        const waitMs = tutorialNextWaitMs();
        const baseLabel = step.last ? "홈으로" : "다음 ▶";
        ctx.globalAlpha = waitMs > 0 ? 0.45 : 1;
        drawSettingsButton(
            TUTORIAL_NEXT_BUTTON.x, TUTORIAL_NEXT_BUTTON.y,
            TUTORIAL_NEXT_BUTTON.w, TUTORIAL_NEXT_BUTTON.h,
            waitMs > 0 ? `${baseLabel}  (${Math.ceil(waitMs / 1000)}초)` : baseLabel
        );
        ctx.globalAlpha = 1;
    }

    // 상단 바 (맵의 바깥 벽 줄 위에 표시)
    ctx.fillStyle = "rgba(9,12,17,0.94)";
    ctx.fillRect(0, 0, WIDTH, 40);
    ctx.textAlign = "left";
    ctx.fillStyle = "#7ddcff";
    ctx.font = "700 15px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(`📖 튜토리얼 ${tutorialStep + 1}/${TUTORIAL_STEPS.length} · ${step.title}`, 14, 20);
    drawSettingsButton(
        TUTORIAL_EXIT_BUTTON.x, TUTORIAL_EXIT_BUTTON.y,
        TUTORIAL_EXIT_BUTTON.w, TUTORIAL_EXIT_BUTTON.h, "종료"
    );

    // 오른쪽 가운데의 반투명 퀘스트 창
    if (!isInfo) {
        const panel = { x: WIDTH - 262, y: 130, w: 250, h: 345 };
        const innerX = panel.x + 16;
        const innerW = panel.w - 32;

        ctx.fillStyle = "rgba(15,20,28,0.80)";
        ctx.strokeStyle = "rgba(255,215,106,0.55)";
        ctx.lineWidth = 1.5;
        ctx.beginPath();
        ctx.roundRect(panel.x, panel.y, panel.w, panel.h, 14);
        ctx.fill();
        ctx.stroke();

        ctx.textAlign = "left";
        ctx.fillStyle = "#ffd76a";
        ctx.font = "700 12px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("📜 튜토리얼 미션", innerX, panel.y + 22);

        ctx.fillStyle = "rgba(255,255,255,0.14)";
        ctx.fillRect(innerX, panel.y + 36, innerW, 1);

        ctx.fillStyle = "#ffffff";
        ctx.font = "bold 17px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(step.title, innerX, panel.y + 58);

        ctx.fillStyle = "#dfe5ea";
        ctx.font = "600 14px Pretendard, Noto Sans KR, sans-serif";
        wrapTutorialText(step.text, innerW).slice(0, 5).forEach((line, i) => {
            ctx.fillText(line, innerX, panel.y + 86 + i * 22);
        });

        // 진행 상황 / 결과 안내
        let statusText = "";
        let statusColor = "#9dffb4";
        if (now < tutorialNoticeUntil && tutorialNotice) {
            statusText = tutorialNotice;
        } else if (step.type === "move") {
            statusText = `이동 ${Math.min(tutorialMoves, step.need)}/${step.need}`;
            statusColor = "#9eabb9";
        }

        if (statusText) {
            const box = { x: innerX, y: panel.y + 188, w: innerW, h: 58 };
            ctx.fillStyle = "rgba(255,255,255,0.06)";
            ctx.beginPath();
            ctx.roundRect(box.x, box.y, box.w, box.h, 9);
            ctx.fill();

            ctx.fillStyle = statusColor;
            ctx.font = "600 13px Pretendard, Noto Sans KR, sans-serif";
            const statusLines = wrapTutorialText(statusText, box.w - 16).slice(0, 3);
            const startY = box.y + box.h / 2 - (statusLines.length - 1) * 9;
            statusLines.forEach((line, i) => {
                ctx.fillText(line, box.x + 8, startY + i * 18);
            });
        }

        // 미션 완료 후: 터치하면 다음으로 안내
        if (tutorialAwaitingNext) {
            const hintBox = { x: innerX, y: panel.y + 262, w: innerW, h: 56 };
            const blink = 0.65 + 0.35 * Math.sin(now * 0.006);
            ctx.fillStyle = `rgba(255,215,106,${0.10 + 0.08 * blink})`;
            ctx.strokeStyle = `rgba(255,215,106,${0.55 * blink + 0.2})`;
            ctx.lineWidth = 1.5;
            ctx.beginPath();
            ctx.roundRect(hintBox.x, hintBox.y, hintBox.w, hintBox.h, 9);
            ctx.fill();
            ctx.stroke();

            ctx.textAlign = "center";
            ctx.fillStyle = "#ffd76a";
            ctx.font = "700 15px Pretendard, Noto Sans KR, sans-serif";
            ctx.fillText("👆 터치하면 다음으로 ▶", hintBox.x + hintBox.w / 2, hintBox.y + 20);
            ctx.fillStyle = "#9eabb9";
            ctx.font = "11px Pretendard, Noto Sans KR, sans-serif";
            ctx.fillText("(PC : 클릭 / Space / Enter)", hintBox.x + hintBox.w / 2, hintBox.y + 40);
        }
    }

    ctx.restore();
}

document.getElementById("startTutorialButton")?.addEventListener("click", async event => {
    event.preventDefault();
    event.stopPropagation();
    playUIClickSound();
    const ok = await openLogoutConfirm({
        title: "튜토리얼",
        message: "튜토리얼을 시작하시겠습니까?\n(코인 · 점수 · 랭킹에 영향을 주지 않습니다)",
        confirmLabel: "시작",
        danger: false
    });
    if (ok && gameState === "start") startTutorial();
});

canvas.addEventListener("pointerdown", event => {
    tutorialPointerDown = { x: event.clientX, y: event.clientY };
}, { passive: true });

canvas.addEventListener("pointerup", event => {
    if (gameState !== "tutorial") return;
    if (Math.hypot(event.clientX - tutorialPointerDown.x, event.clientY - tutorialPointerDown.y) > 12) return;
    const rect = canvas.getBoundingClientRect();
    const x = (event.clientX - rect.left) * (WIDTH / rect.width);
    const y = (event.clientY - rect.top) * (HEIGHT / rect.height);
    if (handleTutorialTap(x, y)) lastTutorialTapTime = performance.now();
});

addGameTouchListener("touchend", event => {
    if (gameState !== "tutorial" || event.changedTouches.length !== 1) return;

    const touch = event.changedTouches[0];
    const dx = touch.clientX - touchStartX;
    const dy = touch.clientY - touchStartY;
    const distance = Math.hypot(dx, dy);
    const duration = performance.now() - touchStartTime;

    if (distance < SWIPE_MIN_DISTANCE) {
        if (duration > TAP_MAX_DURATION) return;
        if (performance.now() - lastTutorialTapTime < 450) return;
        const rect = canvas.getBoundingClientRect();
        const x = (touch.clientX - rect.left) * (WIDTH / rect.width);
        const y = (touch.clientY - rect.top) * (HEIGHT / rect.height);
        if (handleTutorialTap(x, y)) lastTutorialTapTime = performance.now();
        return;
    }

    if (Math.abs(dx) > Math.abs(dy)) startMove(dx > 0 ? 1 : -1, 0);
    else startMove(0, dy > 0 ? 1 : -1);
}, { passive: true });

window.addEventListener("keydown", event => {
    if (!gameAccessGranted || gameState !== "tutorial" || event.repeat) return;
    const key = event.key.toLowerCase();
    const step = TUTORIAL_STEPS[tutorialStep];

    if (key === "escape") {
        requestTutorialExit();
        return;
    }
    if (tutorialAwaitingNext && (key === "enter" || event.code === "Space")) {
        event.preventDefault();
        if (performance.now() - tutorialCompletedAt < 500) return;
        tutorialAdvance();
        return;
    }
    if (step && step.type === "info" && (key === "enter" || event.code === "Space")) {
        event.preventDefault();
        if (tutorialNextWaitMs() > 0) return;
        tutorialAdvance();
    }
});

/* =========================================================
   더블 동작 (스페이스 더블 / PC 화면 밖 더블클릭 공용)
   - 시작 화면: 게임 시작 / 플레이 중: 경로 안내 재사용 → 맵 넘기기
   - 2인 대전: 포기 확인창 / 튜토리얼: 맵 넘기기 단계 동작
========================================================= */
let lastSpacePressTime = 0;

function performDoubleAction() {
    if (!gameAccessGranted || loadingActive || gamePopupOpen || guestNameOpen ||
        rewardListOpen || logoutConfirmOpen || energyRecoveryChoiceOpen) return;
    if (document.getElementById("rankingPanel")?.hidden === false) return;

    if (gameState === "start") {
        if (isMultiplayerPending()) return;
        if (settingsOpen || questOpen || shopOpen || inventoryOpen || skinOpen || multiplayerOpen) return;
        withGuestName(playGameStartSoundAndThenStart);
        return;
    }

    if (gameState === "tutorial") {
        if (!tutorialAwaitingNext) skipMap();
        return;
    }

    if (multiplayerMatchActive) {
        if (gameState !== "multiplayerResult" && gameState !== "expResult") openGamePopup("multi");
        return;
    }

    if (["gameover", "multiplayerResult", "expResult",
         "multiplayerWaitingRound", "multiplayerWaitingResult"].includes(gameState)) return;

    if (!useSecondPathGuide()) skipMap();
}

// 메뉴/결과 화면에서 시작한 마우스 입력은 직후 더블클릭 동작을 막기 위해 기록합니다.
let lastBlockedPressTime = 0;
document.addEventListener("pointerdown", event => {
    if (event.pointerType !== "mouse") return;
    const menuOpen = settingsOpen || questOpen || shopOpen || inventoryOpen ||
                     skinOpen || multiplayerOpen;
    const resultScreen = ["gameover", "multiplayerResult", "expResult"].includes(gameState);
    if (menuOpen || resultScreen) lastBlockedPressTime = performance.now();
}, true); // capture 단계에서 상태가 바뀌기 전에 기록

// PC: 게임 영역(캔버스 포함) 또는 화면 밖 빈 배경 더블클릭 = 더블 터치
document.addEventListener("dblclick", event => {
    const t = event.target;
    const onGameArea = t === document.body || t === document.documentElement ||
        t === gameWrapper || t === canvas || t === canvasStage;
    if (!onGameArea) return;

    event.preventDefault();
    // 메뉴를 닫거나 결과 화면을 넘긴 직후 발생한 더블클릭은 무시합니다.
    if (performance.now() - lastBlockedPressTime < 700) return;
    performDoubleAction();
});

// PC: 결과 화면에서는 화면 안/밖 클릭으로도 다음 단계로 이동
document.addEventListener("click", event => {
    if (!gameAccessGranted) return;
    const t = event.target;
    const onGameArea = t === document.body || t === document.documentElement ||
        t === gameWrapper || t === canvas || t === canvasStage;
    if (!onGameArea) return;

    if (gameState === "gameover" || gameState === "multiplayerResult") startExperienceResult();
    else if (gameState === "expResult") finishExperienceResult();
});


/* =========================================================
   PC: 시작 화면에서 게임 캔버스 바깥의 빈 배경을 클릭하면 열린 메뉴 닫기
   - 모바일 터치 동작은 기존 캔버스 입력 처리를 그대로 사용합니다.
   - 로그인/팝업/랭킹 등 별도 UI 클릭에는 개입하지 않습니다.
========================================================= */
document.addEventListener("click", event => {
    // 마우스/트랙패드 환경에서만 적용하여 모바일 터치 동작과 충돌하지 않게 합니다.
    if (!window.matchMedia("(hover: hover) and (pointer: fine)").matches) return;
    if (!gameAccessGranted || gameState !== "start") return;
    if (loadingActive || gamePopupOpen || guestNameOpen || logoutConfirmOpen || rewardListOpen) return;
    if (document.getElementById("rankingPanel")?.hidden === false) return;

    const target = event.target;
    const clickedBlankOutsideCanvas =
        target === document.body ||
        target === document.documentElement ||
        target === gameWrapper;
    if (!clickedBlankOutsideCanvas) return;

    const hasOpenMenu = settingsOpen || questOpen || shopOpen || inventoryOpen || skinOpen || multiplayerOpen;
    if (!hasOpenMenu) return;

    // 메뉴 상태를 한 번에 닫되, 게임 진행/기록/인벤토리 내용은 변경하지 않습니다.
    settingsOpen = false;
    questOpen = false;
    shopOpen = false;
    inventoryOpen = false;
    closeInventoryDetail();
    skinOpen = false;
    if (multiplayerOpen) closeMultiplayerMenu();

    syncQuestRewardOverlay(true);
    requestSettingsRender();
    positionVolumeTouchArea();
});

let volumeSliderDragging = false;

let lastSettingsPointerTime = 0;


canvas.addEventListener(
    "pointerup",
    event => {

        if (document.getElementById("rankingPanel")?.hidden === false) {
            return;
        }

        if (!gameAccessGranted) {
            return;
        }

        if (
            gameState !== "start"
        ) {
            return;
        }

        const rect =
            canvas.getBoundingClientRect();

        const x =
            (
                event.clientX -
                rect.left
            ) *
            (
                WIDTH /
                rect.width
            );

        const y =
            (
                event.clientY -
                rect.top
            ) *
            (
                HEIGHT /
                rect.height
            );

        // 퀘스트 보상 수령은 일반 시작 화면의 더블탭 처리보다 먼저 확정합니다.
        if (questOpen && handleQuestRewardTap(x, y)) {
            lastSettingsPointerTime = performance.now();
            return;
        }

        if (
            handleSettingsTap(
                x,
                y
            )
        ) {
            playUIClickSound();
            lastSettingsPointerTime =
                performance.now();
        }
    }
);


/* =========================================================
   업데이트
========================================================= */

let gameplayUIAccumulator = 0;
function update(delta) {
    if (gameState === "tutorial") updateMovement(delta);
    refreshDailyQuestIfNeeded();

    // 시작 전 카운트다운: 끝나면 플레이 시작 (그 전에는 제한 시간이 흐르지 않음)
    if (countdownActive && performance.now() >= countdownEndAt) {
        finishIntroCountdown();
    }

    // 게임이 끝났거나 상태가 바뀌어 더 이상 의미 없는 팝업은 닫습니다.
    if (gamePopupOpen) {
        const stale = !GAME_POPUP_STATES.includes(gameState) ||
            (gamePopupMode === "multi" && !multiplayerMatchActive) ||
            (gamePopupMode === "solo" && multiplayerMatchActive);
        if (stale) closeGamePopup();
    }

    if (multiplayerMatchActive) {
        multiplayerSendAccumulator += delta;
        if (opponent.visible) {
            const follow = Math.min(1, delta * 18);
            opponent.x += (opponent.targetX - opponent.x) * follow;
            opponent.y += (opponent.targetY - opponent.y) * follow;
        }
    }

    for (
        let i = trail.length - 1;
        i >= 0;
        i--
    ) {

        trail[i].life -=
            delta * 3.5;

        if (
            trail[i].life <= 0
        ) {
            trail.splice(i, 1);
        }
    }

    updateRecoil(delta);

    if (
        shake.time > 0
    ) {

        shake.time -= delta;

        if (
            shake.time <= 0
        ) {

            shake.time = 0;
            shake.power = 0;
        }
    }

    if (
        flash.alpha > 0
    ) {

        flash.alpha -=
            delta * 0.9;

        if (
            flash.alpha < 0
        ) {
            flash.alpha = 0;
        }
    }

    updateMapTransition(delta);

    if (
        gameState === "playing"
    ) {

        remainingTime -= delta;

        if (
            remainingTime <= 0
        ) {

            remainingTime = 0;

            timeoutGame();

            return;
        }

        updateMovement(delta);
        sendMultiplayerPosition();

        // 매 프레임 DOM 전체를 갱신하면 멀티플레이에서 입력/렌더링이 끊기므로
        // 화면의 숫자/UI는 초당 약 10회만 갱신합니다.
        gameplayUIAccumulator += delta;
        if (gameplayUIAccumulator >= 0.10) {
            gameplayUIAccumulator = 0;
            updateUI();
        }
    } else if (
        gameState === "multiplayerWaitingResult" &&
        multiplayerSelfDead &&
        multiplayerMatchActive
    ) {
        // 관전 중에는 표시용으로만 시간을 줄입니다. (시간 초과 처리는 하지 않음)
        remainingTime = Math.max(0, remainingTime - delta);
        gameplayUIAccumulator += delta;
        if (gameplayUIAccumulator >= 0.10) {
            gameplayUIAccumulator = 0;
            updateUI();
        }
    }
}


/* =========================================================
   배경
========================================================= */

function drawBackground() {

    ctx.fillStyle =
        getBackgroundColor();

    ctx.fillRect(
        0,
        0,
        WIDTH,
        HEIGHT
    );
}


/* =========================================================
   연속 클리어 효과
========================================================= */

function getStreakStrength() {

    if (
        clearStreak < 1
    ) {
        return 0;
    }

    if (
        clearStreak === 1
    ) {
        return 0.07;
    }

    return Math.min(
        1,
        0.24 +
        (clearStreak - 2) *
        0.15
    );
}


/* 효과/위험 블록 공용 도우미 */
function fxHash(n) { const v = Math.sin(n * 127.1 + 311.7) * 43758.5453; return v - Math.floor(v); }
function fxPerim(p) {
    const P = 2 * (WIDTH + HEIGHT);
    let d = (((p % 1) + 1) % 1) * P;
    if (d < WIDTH) return { x: d, y: 0, nx: 0, ny: 1 };
    d -= WIDTH;
    if (d < HEIGHT) return { x: WIDTH, y: d, nx: -1, ny: 0 };
    d -= HEIGHT;
    if (d < WIDTH) return { x: WIDTH - d, y: HEIGHT, nx: 0, ny: -1 };
    d -= WIDTH;
    return { x: 0, y: HEIGHT - d, nx: 1, ny: 0 };
}

const STREAK_RENDERERS = {
    aurora(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        for (let i = 0; i < 3; i++) {
            const g = ctx.createLinearGradient(0, 0, WIDTH, HEIGHT);
            for (let n = 0; n <= 4; n++) g.addColorStop(n / 4, `hsla(${(150 + i * 50 + n * 35 + Math.sin(t * 0.8 + i) * 40) % 360},90%,60%,${0.35 + 0.3 * Math.sin(t * 1.5 + n + i)})`);
            const lw = 10 + 22 * k - i * 5;
            ctx.strokeStyle = g; ctx.lineWidth = lw; ctx.globalAlpha = 0.10 + 0.22 * k;
            ctx.shadowBlur = 20; ctx.shadowColor = "rgba(120,255,200,0.6)";
            ctx.strokeRect(lw / 2, lw / 2, WIDTH - lw, HEIGHT - lw);
        }
        ctx.restore();
    },
    ember(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        for (let i = 0; i < 44; i++) {
            const ph = (t * (0.25 + fxHash(i) * 0.35) + fxHash(i + 50)) % 1;
            const p = fxPerim(fxHash(i + 9));
            const d = ph * (24 + 40 * k), sway = Math.sin(t * 3 + i) * 5;
            const px = p.x + p.nx * d + p.ny * sway, py = p.y + p.ny * d - p.nx * sway;
            ctx.fillStyle = `hsla(${12 + ph * 34},100%,${55 + ph * 20}%,${(1 - ph) * (0.25 + 0.5 * k)})`;
            ctx.shadowBlur = 8; ctx.shadowColor = "rgba(255,120,40,0.8)";
            ctx.beginPath(); ctx.arc(px, py, (1 + fxHash(i + 3) * 2.2) * (0.6 + k * 0.6) * (1 - ph * 0.5), 0, Math.PI * 2); ctx.fill();
        }
        const lw = 8 + 10 * k;
        ctx.shadowBlur = 16; ctx.shadowColor = "rgba(255,90,30,0.7)";
        ctx.strokeStyle = `rgba(255,90,30,${0.05 + 0.1 * k})`; ctx.lineWidth = lw;
        ctx.strokeRect(lw / 2, lw / 2, WIDTH - lw, HEIGHT - lw);
        ctx.restore();
    },
    lightning(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        const lw = 6 + 8 * k;
        ctx.strokeStyle = `rgba(90,200,255,${0.07 + 0.13 * k})`; ctx.lineWidth = lw;
        ctx.shadowBlur = 14; ctx.shadowColor = "#46d8ff";
        ctx.strokeRect(lw / 2, lw / 2, WIDTH - lw, HEIGHT - lw);
        const tick = Math.floor(t * 7);
        for (let i = 0; i < 4; i++) {
            const seed = tick * 7 + i * 13;
            if (fxHash(seed) < 0.45) continue;
            const p = fxPerim(fxHash(seed + 1));
            let x = p.x, y = p.y;
            ctx.beginPath(); ctx.moveTo(x, y);
            for (let n = 1; n <= 5; n++) {
                const step = (14 + 30 * k) / 5 * 1;
                x += p.nx * step * 1.6 + p.ny * (fxHash(seed + n * 3) - 0.5) * 26;
                y += p.ny * step * 1.6 - p.nx * (fxHash(seed + n * 3) - 0.5) * 26;
                ctx.lineTo(x, y);
            }
            ctx.strokeStyle = `rgba(235,250,255,${0.5 + 0.4 * k})`; ctx.lineWidth = 1.5 + k;
            ctx.shadowBlur = 12; ctx.shadowColor = "#7fe3ff"; ctx.stroke();
        }
        ctx.restore();
    },
    petals(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save();
        for (let i = 0; i < 26; i++) {
            const p = fxPerim(fxHash(i) + t * (0.012 + fxHash(i + 4) * 0.015));
            const d = (10 + fxHash(i + 8) * 30 * (0.5 + k)) + Math.sin(t * 1.6 + i) * 6;
            const px = p.x + p.nx * d, py = p.y + p.ny * d;
            ctx.translate(px, py); ctx.rotate(t * 1.3 + i);
            ctx.fillStyle = `hsla(${335 + fxHash(i + 2) * 25},90%,${75 + fxHash(i) * 12}%,${0.22 + 0.45 * k})`;
            ctx.beginPath(); ctx.ellipse(0, 0, 3 + 3.5 * k, 1.8 + 1.6 * k, 0, 0, Math.PI * 2); ctx.fill();
            // 캔버스 해상도가 커져도 논리 좌표계(800x600)를 유지합니다.
            ctx.setTransform(renderScale, 0, 0, renderScale, 0, 0);
            ctx.restore(); ctx.save();
        }
        ctx.restore();
    },
    pulse(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        for (let i = 0; i < 3; i++) {
            const ph = (t * 0.6 + i / 3) % 1, inset = ph * (26 + 34 * k);
            ctx.strokeStyle = `hsla(${195 + i * 25},100%,68%,${(1 - ph) * (0.12 + 0.3 * k)})`;
            ctx.lineWidth = 2 + 3 * k * (1 - ph);
            ctx.shadowBlur = 12; ctx.shadowColor = ctx.strokeStyle;
            ctx.beginPath(); ctx.roundRect(inset + 2, inset + 2, WIDTH - inset * 2 - 4, HEIGHT - inset * 2 - 4, 6 + ph * 14); ctx.stroke();
        }
        ctx.restore();
    },
    comet(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        const heads = 2 + Math.round(k * 2);
        for (let c = 0; c < heads; c++) {
            const head = t * 0.13 + c / heads;
            for (let i = 0; i < 22; i++) {
                const p = fxPerim(head - i * 0.0045), f = 1 - i / 22;
                ctx.fillStyle = `hsla(${45 - i * 1.5},100%,${80 - i}%,${f * (0.3 + 0.6 * k)})`;
                ctx.shadowBlur = 10; ctx.shadowColor = "rgba(255,230,150,0.9)";
                ctx.beginPath(); ctx.arc(p.x + p.nx * 7, p.y + p.ny * 7, (1.4 + 4.2 * k) * f, 0, Math.PI * 2); ctx.fill();
            }
        }
        ctx.restore();
    },
    snow(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        const lw = 8 + 10 * k;
        ctx.strokeStyle = `rgba(170,225,255,${0.06 + 0.12 * k})`; ctx.lineWidth = lw;
        ctx.shadowBlur = 16; ctx.shadowColor = "rgba(150,220,255,0.8)";
        ctx.strokeRect(lw / 2, lw / 2, WIDTH - lw, HEIGHT - lw);
        for (let i = 0; i < 40; i++) {
            const ph = (t * (0.18 + fxHash(i) * 0.2) + fxHash(i + 70)) % 1;
            const p = fxPerim(fxHash(i + 9));
            const d = ph * (20 + 40 * k), sway = Math.sin(t * 2 + i) * 6;
            const px = p.x + p.nx * d + p.ny * sway, py = p.y + p.ny * d - p.nx * sway;
            ctx.fillStyle = `rgba(235,248,255,${(1 - ph) * (0.3 + 0.55 * k)})`;
            ctx.shadowBlur = 6; ctx.shadowColor = "rgba(200,240,255,0.9)";
            ctx.beginPath(); ctx.arc(px, py, (1 + fxHash(i + 3) * 2) * (0.7 + k * 0.5), 0, Math.PI * 2); ctx.fill();
        }
        ctx.restore();
    },
    spore(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        const lw = 8 + 10 * k;
        ctx.strokeStyle = `rgba(120,255,100,${0.05 + 0.1 * k})`; ctx.lineWidth = lw;
        ctx.shadowBlur = 16; ctx.shadowColor = "rgba(110,255,100,0.7)";
        ctx.strokeRect(lw / 2, lw / 2, WIDTH - lw, HEIGHT - lw);
        for (let i = 0; i < 30; i++) {
            const ph = (t * (0.15 + fxHash(i) * 0.2) + fxHash(i + 30)) % 1;
            const p = fxPerim(fxHash(i + 5));
            const d = 10 + ph * (30 + 40 * k), sway = Math.sin(t * 1.8 + i) * 6;
            const px = p.x + p.nx * d + p.ny * sway, py = p.y + p.ny * d - p.nx * sway;
            const r = (2 + fxHash(i + 2) * 4) * (0.6 + k * 0.5);
            ctx.fillStyle = `rgba(110,230,100,${(1 - ph) * (0.08 + 0.12 * k)})`;
            ctx.strokeStyle = `rgba(170,255,140,${(1 - ph) * (0.25 + 0.5 * k)})`;
            ctx.lineWidth = 1.3; ctx.shadowBlur = 8; ctx.shadowColor = "rgba(120,255,110,0.8)";
            ctx.beginPath(); ctx.arc(px, py, r, 0, Math.PI * 2); ctx.fill(); ctx.stroke();
        }
        ctx.restore();
    },
    goldRain(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        const lw = 6 + 8 * k;
        ctx.strokeStyle = `rgba(255,200,70,${0.06 + 0.12 * k})`; ctx.lineWidth = lw;
        ctx.shadowBlur = 14; ctx.shadowColor = "rgba(255,200,60,0.7)";
        ctx.strokeRect(lw / 2, lw / 2, WIDTH - lw, HEIGHT - lw);
        for (let i = 0; i < 30; i++) {
            const ph = (t * (0.25 + fxHash(i) * 0.25) + fxHash(i + 11)) % 1;
            const px = (i % 2 ? 0 : WIDTH - 46) + fxHash(i + 3) * 46, py = ph * HEIGHT;
            const sx = Math.max(0.25, Math.abs(Math.cos(t * 5 + i)));
            ctx.fillStyle = `rgba(255,205,70,${0.25 + 0.5 * k})`;
            ctx.shadowBlur = 8; ctx.shadowColor = "rgba(255,210,80,0.9)";
            ctx.beginPath(); ctx.ellipse(px, py, (2 + 3 * k) * sx, 2 + 3 * k, 0, 0, Math.PI * 2); ctx.fill();
        }
        ctx.restore();
    },
    neon(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        for (let i = 0; i < 2; i++) {
            const g = ctx.createLinearGradient(0, 0, WIDTH, HEIGHT);
            const a = (0.18 + 0.32 * k) * (0.75 + 0.25 * Math.sin(t * 4 + i * 2));
            g.addColorStop(0, `hsla(180,100%,60%,${a})`);
            g.addColorStop(0.5, `hsla(305,100%,62%,${a})`);
            g.addColorStop(1, `hsla(180,100%,60%,${a})`);
            const lw = 4 + 8 * k - i * 2;
            ctx.strokeStyle = g; ctx.lineWidth = lw;
            ctx.shadowBlur = 18; ctx.shadowColor = i ? "#ff46dc" : "#37f5ff";
            ctx.strokeRect(lw / 2 + i * 5, lw / 2 + i * 5, WIDTH - lw - i * 10, HEIGHT - lw - i * 10);
        }
        const heads = 1 + Math.round(k);
        for (let h = 0; h < heads; h++) {
            const head = t * 0.18 + h / heads;
            for (let i = 0; i < 16; i++) {
                const p = fxPerim(head - i * 0.004), f = 1 - i / 16;
                ctx.fillStyle = `hsla(${h ? 305 : 180},100%,${85 - i * 2}%,${f * (0.4 + 0.5 * k)})`;
                ctx.shadowBlur = 10; ctx.shadowColor = h ? "#ff46dc" : "#37f5ff";
                ctx.beginPath(); ctx.arc(p.x + p.nx * 6, p.y + p.ny * 6, (1.5 + 3.5 * k) * f, 0, Math.PI * 2); ctx.fill();
            }
        }
        ctx.restore();
    },
    rainbowNeon(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        const P = 2 * (WIDTH + HEIGHT), m = 6;
        const edges = [
            { x1: m, y1: m, x2: WIDTH - m, y2: m, o: 0 },
            { x1: WIDTH - m, y1: m, x2: WIDTH - m, y2: HEIGHT - m, o: WIDTH },
            { x1: WIDTH - m, y1: HEIGHT - m, x2: m, y2: HEIGHT - m, o: WIDTH + HEIGHT },
            { x1: m, y1: HEIGHT - m, x2: m, y2: m, o: 2 * WIDTH + HEIGHT }
        ];
        const hueAt = d => ((d / P) * 360 + t * 90) % 360;
        ctx.save(); ctx.globalCompositeOperation = "screen"; ctx.lineCap = "round";
        for (let layer = 0; layer < 2; layer++) {
            const lw = layer === 0 ? 5 + 9 * k : 1.8 + 2.2 * k;
            const alpha = layer === 0 ? 0.22 + 0.38 * k : 0.55 + 0.4 * k;
            for (const e of edges) {
                const len = Math.hypot(e.x2 - e.x1, e.y2 - e.y1);
                const g = ctx.createLinearGradient(e.x1, e.y1, e.x2, e.y2);
                for (let n = 0; n <= 8; n++) {
                    g.addColorStop(n / 8, `hsla(${hueAt(e.o + len * n / 8)},100%,${layer ? 78 : 60}%,${alpha})`);
                }
                ctx.strokeStyle = g; ctx.lineWidth = lw;
                ctx.shadowBlur = layer === 0 ? 22 : 10;
                ctx.shadowColor = `hsla(${hueAt(e.o + len / 2)},100%,62%,0.95)`;
                ctx.beginPath(); ctx.moveTo(e.x1, e.y1); ctx.lineTo(e.x2, e.y2); ctx.stroke();
            }
        }
        const heads = 1 + Math.round(k * 2);
        for (let h = 0; h < heads; h++) {
            const head = t * 0.16 + h / heads;
            for (let i = 0; i < 18; i++) {
                const p = fxPerim(head - i * 0.004), f = 1 - i / 18;
                const hue = hueAt(((head - i * 0.004) % 1 + 1) % 1 * P);
                ctx.fillStyle = `hsla(${hue},100%,${88 - i * 2}%,${f * (0.45 + 0.5 * k)})`;
                ctx.shadowBlur = 12; ctx.shadowColor = `hsla(${hue},100%,65%,1)`;
                ctx.beginPath(); ctx.arc(p.x + p.nx * 9, p.y + p.ny * 9, (1.6 + 3.6 * k) * f, 0, Math.PI * 2); ctx.fill();
            }
        }
        ctx.restore();
    },
    prism(s) {
        const k = Math.min(1, s), t = performance.now() * 0.001;
        ctx.save(); ctx.globalCompositeOperation = "screen";
        const N = 96;
        for (let i = 0; i < N; i++) {
            const p = fxPerim(i / N);
            const wave = (Math.sin(t * 2.5 - i * 0.28) + 1) / 2;
            ctx.fillStyle = `hsla(${(i * 3.75 + t * 70) % 360},100%,62%,${(0.10 + 0.35 * k) * (0.35 + 0.65 * wave)})`;
            ctx.shadowBlur = 10; ctx.shadowColor = ctx.fillStyle;
            ctx.beginPath(); ctx.arc(p.x + p.nx * 8, p.y + p.ny * 8, 2 + 4 * k * wave, 0, Math.PI * 2); ctx.fill();
        }
        ctx.restore();
    }
};

function drawStreakEffect() {
    const strength = getStreakStrength();
    const effect = (STREAK_EFFECTS[visualSettings.streakEffect] || STREAK_EFFECTS[0]).value;
    if (strength <= 0 || effect === "none") return;
    const fn = STREAK_RENDERERS[effect];
    if (fn) fn(strength);
}

/* =========================================================
   위험 블록 스킨
========================================================= */
function drawDangerBlock(c, r, skin) {
    const x = c * CELL, y = r * CELL, t = performance.now() * 0.001;
    const cx = x + CELL / 2, cy = y + CELL / 2;
    ctx.save();
    switch (skin) {
        case "spike": {
            ctx.fillStyle = "rgba(255,60,80,0.12)"; ctx.fillRect(x + 3, y + 3, CELL - 6, CELL - 6);
            const g = ctx.createRadialGradient(cx, cy, 2, cx, cy, 18); g.addColorStop(0, "#ff8a96"); g.addColorStop(1, "#c4202f");
            ctx.fillStyle = g; ctx.beginPath();
            for (let i = 0; i < 16; i++) {
                const a = i * Math.PI / 8 + t * 0.6, rad = i % 2 === 0 ? 17.5 : 8.5;
                i ? ctx.lineTo(cx + Math.cos(a) * rad, cy + Math.sin(a) * rad) : ctx.moveTo(cx + Math.cos(a) * rad, cy + Math.sin(a) * rad);
            }
            ctx.closePath(); ctx.fill(); ctx.strokeStyle = "#5a0d16"; ctx.lineWidth = 1.5; ctx.stroke();
            ctx.fillStyle = "#2a0a10"; ctx.beginPath(); ctx.arc(cx, cy, 4, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "laser": {
            ctx.fillStyle = "#140a10"; ctx.fillRect(x + 3, y + 3, CELL - 6, CELL - 6);
            for (let i = 0; i < 3; i++) {
                const pulse = (Math.sin(t * 6 + i * 1.7) + 1) / 2, yy = y + 10 + i * 10;
                ctx.strokeStyle = `rgba(255,50,70,${0.45 + pulse * 0.55})`; ctx.lineWidth = 2;
                ctx.shadowBlur = 8; ctx.shadowColor = "#ff2e46";
                ctx.beginPath(); ctx.moveTo(x + 6, yy); ctx.lineTo(x + CELL - 6, yy); ctx.stroke();
            }
            ctx.shadowBlur = 0; ctx.fillStyle = "#6b7684";
            for (let i = 0; i < 3; i++) { ctx.fillRect(x + 3, y + 8 + i * 10, 4, 4); ctx.fillRect(x + CELL - 7, y + 8 + i * 10, 4, 4); }
            ctx.strokeStyle = "rgba(255,50,70,0.6)"; ctx.lineWidth = 1.5; ctx.strokeRect(x + 3.5, y + 3.5, CELL - 7, CELL - 7);
            break;
        }
        case "lava": {
            const g = ctx.createLinearGradient(x, y, x, y + CELL); g.addColorStop(0, "#ff9a2a"); g.addColorStop(1, "#c4200f");
            ctx.beginPath(); ctx.roundRect(x + 3, y + 3, CELL - 6, CELL - 6, 7); ctx.fillStyle = g; ctx.fill();
            ctx.save(); ctx.clip();
            for (let i = 0; i < 3; i++) {
                ctx.fillStyle = "rgba(255,225,100,0.7)"; ctx.beginPath();
                ctx.arc(cx + Math.sin(t * 1.7 + i * 2.1) * 9, cy + Math.cos(t * 1.3 + i * 1.6) * 9, 4 + i, 0, Math.PI * 2); ctx.fill();
            }
            ctx.restore();
            ctx.strokeStyle = "#3a0d08"; ctx.lineWidth = 3; ctx.beginPath(); ctx.roundRect(x + 4.5, y + 4.5, CELL - 9, CELL - 9, 6); ctx.stroke();
            break;
        }
        case "bomb": {
            ctx.fillStyle = "rgba(255,60,60,0.16)"; ctx.fillRect(x + 3, y + 3, CELL - 6, CELL - 6);
            ctx.strokeStyle = "rgba(255,80,90,0.85)"; ctx.lineWidth = 2; ctx.strokeRect(x + 3.5, y + 3.5, CELL - 7, CELL - 7);
            const bg = ctx.createRadialGradient(cx - 4, cy, 1, cx, cy + 3, 15); bg.addColorStop(0, "#7a8494"); bg.addColorStop(1, "#171b22");
            ctx.fillStyle = bg; ctx.beginPath(); ctx.arc(cx, cy + 3, 13.5, 0, Math.PI * 2); ctx.fill();
            ctx.strokeStyle = "#9aa5b4"; ctx.lineWidth = 1.2; ctx.stroke();
            ctx.fillStyle = "rgba(255,255,255,0.35)"; ctx.beginPath(); ctx.ellipse(cx - 5, cy - 2, 3.5, 2.2, -0.6, 0, Math.PI * 2); ctx.fill();
            ctx.fillStyle = "#8b95a3"; ctx.fillRect(cx - 4, cy - 12, 8, 4);
            ctx.strokeStyle = "#d1b57d"; ctx.lineWidth = 2; ctx.beginPath(); ctx.moveTo(cx + 2, cy - 12); ctx.quadraticCurveTo(cx + 11, cy - 12, cx + 10, cy - 17); ctx.stroke();
            ctx.fillStyle = "#ffd24a"; ctx.shadowBlur = 12; ctx.shadowColor = "#ff7a1f";
            ctx.beginPath(); ctx.arc(cx + 10, cy - 17, 3 + Math.sin(t * 20) * 1.2, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "electric": {
            ctx.fillStyle = "#0b1630"; ctx.fillRect(x + 3, y + 3, CELL - 6, CELL - 6);
            const seed = Math.floor(t * 10) * 11 + c * 7 + r * 13;
            ctx.beginPath(); ctx.moveTo(x + 9, y + 6);
            for (let n = 1; n <= 5; n++) ctx.lineTo(x + 9 + (CELL - 18) * n / 5 + (fxHash(seed + n) - 0.5) * 10 * (n < 5 ? 1 : 0), y + 6 + (CELL - 12) * n / 5);
            ctx.strokeStyle = "#fff176"; ctx.lineWidth = 2.4; ctx.lineJoin = "round"; ctx.shadowBlur = 9; ctx.shadowColor = "#46d8ff"; ctx.stroke();
            ctx.shadowBlur = 0; ctx.strokeStyle = "rgba(70,216,255,0.85)"; ctx.lineWidth = 2; ctx.strokeRect(x + 4, y + 4, CELL - 8, CELL - 8);
            break;
        }
        case "toxic": {
            ctx.fillStyle = "#0f2a14"; ctx.beginPath(); ctx.roundRect(x + 3, y + 3, CELL - 6, CELL - 6, 6); ctx.fill();
            ctx.strokeStyle = "#6bff6b"; ctx.lineWidth = 2; ctx.beginPath(); ctx.roundRect(x + 4, y + 4, CELL - 8, CELL - 8, 6); ctx.stroke();
            for (let i = 0; i < 4; i++) {
                const ph = (t * 0.55 + i * 0.27) % 1;
                ctx.strokeStyle = `rgba(150,255,120,${1 - ph * 0.6})`; ctx.fillStyle = `rgba(90,220,90,${0.35 * (1 - ph)})`; ctx.lineWidth = 1.4;
                const bx = x + 10 + i * 7 + Math.sin(t * 2 + i) * 2, by = y + CELL - 8 - ph * (CELL - 16);
                ctx.beginPath(); ctx.arc(bx, by, 2.2 + fxHash(i + c) * 2, 0, Math.PI * 2); ctx.fill(); ctx.stroke();
            }
            break;
        }
        case "void": {
            const g = ctx.createRadialGradient(cx, cy, 1, cx, cy, 18); g.addColorStop(0, "#000"); g.addColorStop(0.6, "#1a0b33"); g.addColorStop(1, "#6b2bd9");
            ctx.fillStyle = g; ctx.beginPath(); ctx.roundRect(x + 3, y + 3, CELL - 6, CELL - 6, 9); ctx.fill();
            ctx.lineWidth = 2; ctx.shadowBlur = 7; ctx.shadowColor = "#b98cff"; ctx.strokeStyle = "#b98cff";
            ctx.setLineDash([5, 4]); ctx.lineDashOffset = -t * 20; ctx.beginPath(); ctx.arc(cx, cy, 13, 0, Math.PI * 2); ctx.stroke();
            ctx.lineDashOffset = t * 24; ctx.strokeStyle = "#e0ccff"; ctx.beginPath(); ctx.arc(cx, cy, 7, 0, Math.PI * 2); ctx.stroke();
            break;
        }
        case "ice": {
            for (let n = 0; n < 3; n++) {
                const bx = x + 8 + n * 12, h = n === 1 ? 28 : 22;
                ctx.fillStyle = n === 1 ? "#d9f6ff" : "#9fdcf7";
                ctx.beginPath(); ctx.moveTo(bx - 6, y + CELL - 4); ctx.lineTo(bx, y + CELL - 4 - h); ctx.lineTo(bx + 6, y + CELL - 4); ctx.closePath(); ctx.fill();
                ctx.strokeStyle = "#3b8fc4"; ctx.lineWidth = 1.3; ctx.stroke();
            }
            ctx.fillStyle = "rgba(255,255,255,0.7)"; ctx.beginPath(); ctx.arc(cx, y + 12, 1.5 + (Math.sin(t * 4) + 1) * 0.5, 0, Math.PI * 2); ctx.fill();
            ctx.strokeStyle = "rgba(120,210,255,0.5)"; ctx.lineWidth = 1.5; ctx.strokeRect(x + 3.5, y + 3.5, CELL - 7, CELL - 7);
            break;
        }
        case "thorn": {
            ctx.fillStyle = "rgba(40,10,25,0.55)"; ctx.fillRect(x + 3, y + 3, CELL - 6, CELL - 6);
            ctx.strokeStyle = "#3f8f4a"; ctx.lineWidth = 2.6; ctx.lineCap = "round";
            ctx.beginPath(); ctx.moveTo(x + 4, y + CELL - 6); ctx.bezierCurveTo(x + 12, y + 8, x + 26, y + 30, x + CELL - 4, y + 6); ctx.stroke();
            ctx.beginPath(); ctx.moveTo(x + 4, y + 8); ctx.bezierCurveTo(x + 14, y + 26, x + 24, y + 10, x + CELL - 4, y + CELL - 6); ctx.stroke();
            ctx.fillStyle = "#c9e8c0";
            [[10, 14], [20, 20], [30, 12], [14, 28], [28, 28]].forEach(([px, py]) => {
                ctx.beginPath(); ctx.moveTo(x + px - 2.5, y + py + 2); ctx.lineTo(x + px, y + py - 4); ctx.lineTo(x + px + 2.5, y + py + 2); ctx.closePath(); ctx.fill();
            });
            const pu = (Math.sin(t * 3) + 1) / 2;
            ctx.fillStyle = "#e8325c"; ctx.shadowBlur = 5 + pu * 5; ctx.shadowColor = "#ff4d7a";
            ctx.beginPath(); ctx.arc(cx, cy, 5, 0, Math.PI * 2); ctx.fill();
            ctx.shadowBlur = 0; ctx.strokeStyle = "#7a0f2c"; ctx.lineWidth = 1.2; ctx.beginPath(); ctx.arc(cx, cy, 2.6, 0, Math.PI * 1.6); ctx.stroke();
            ctx.strokeStyle = "rgba(232,50,92,0.6)"; ctx.lineWidth = 1.5; ctx.strokeRect(x + 3.5, y + 3.5, CELL - 7, CELL - 7);
            break;
        }
        case "trap": {
            ctx.fillStyle = "#2b2010"; ctx.fillRect(x + 3, y + 3, CELL - 6, CELL - 6);
            const up = (Math.sin(t * 3 + c + r) + 1) / 2;
            for (let ry = 0; ry < 2; ry++) for (let rx = 0; rx < 2; rx++) {
                const px = x + 11 + rx * 18, py = y + 12 + ry * 17, h = 5 + up * 5;
                const g = ctx.createLinearGradient(px, py - h, px, py + 5); g.addColorStop(0, "#fff3a8"); g.addColorStop(1, "#b8860b");
                ctx.fillStyle = g; ctx.beginPath(); ctx.moveTo(px - 5, py + 5); ctx.lineTo(px, py - h); ctx.lineTo(px + 5, py + 5); ctx.closePath(); ctx.fill();
            }
            ctx.strokeStyle = "#f5c232"; ctx.lineWidth = 2; ctx.strokeRect(x + 3.5, y + 3.5, CELL - 7, CELL - 7);
            ctx.strokeStyle = "rgba(220,50,60,0.75)"; ctx.lineWidth = 1.2; ctx.strokeRect(x + 6.5, y + 6.5, CELL - 13, CELL - 13);
            break;
        }
        case "neon": {
            const pulse = 0.65 + Math.sin(t * 5 + c + r) * 0.35;
            ctx.fillStyle = "#12060f"; ctx.fillRect(x + 3, y + 3, CELL - 6, CELL - 6);
            ctx.strokeStyle = `rgba(255,40,120,${pulse})`; ctx.lineWidth = 2.5;
            ctx.shadowBlur = 12; ctx.shadowColor = "#ff2878";
            ctx.strokeRect(x + 4, y + 4, CELL - 8, CELL - 8);
            ctx.strokeStyle = `rgba(255,130,200,${0.5 + pulse * 0.5})`; ctx.lineWidth = 2; ctx.lineCap = "round";
            ctx.beginPath();
            ctx.moveTo(x + 12, y + 12); ctx.lineTo(x + CELL - 12, y + CELL - 12);
            ctx.moveTo(x + CELL - 12, y + 12); ctx.lineTo(x + 12, y + CELL - 12);
            ctx.stroke();
            ctx.shadowBlur = 0; ctx.fillStyle = "rgba(255,255,255,0.85)";
            ctx.beginPath(); ctx.arc(cx, cy, 2, 0, Math.PI * 2); ctx.fill();
            break;
        }
        case "solid":
        default: {
            const g = ctx.createLinearGradient(x, y, x, y + CELL); g.addColorStop(0, "#f0505f"); g.addColorStop(1, "#b0212f");
            ctx.fillStyle = g; ctx.beginPath(); ctx.roundRect(x + 4, y + 4, CELL - 8, CELL - 8, 6); ctx.fill();
            ctx.fillStyle = "rgba(255,255,255,0.22)"; ctx.beginPath(); ctx.roundRect(x + 8, y + 8, CELL - 16, 5, 2.5); ctx.fill();
            ctx.strokeStyle = "#6a1420"; ctx.lineWidth = 2; ctx.beginPath(); ctx.roundRect(x + 4, y + 4, CELL - 8, CELL - 8, 6); ctx.stroke();
        }
    }
    ctx.restore();
}


/* =========================================================
   게임 화면
========================================================= */

function getMultiplayerScorePair(scores = multiplayerScores) {
    const me = multiplayerRole === "guest" ? "guest" : "host";
    const other = me === "host" ? "guest" : "host";
    return {
        mine: Number(scores && scores[me]) || 0,
        theirs: Number(scores && scores[other]) || 0
    };
}

function drawMultiplayerScoreHUD() {
    if (!multiplayerMatchActive) return;
    const pair = getMultiplayerScorePair();
    const text = `나 ${pair.mine} : ${pair.theirs} 상대 · 5000점 승리`;
    ctx.save();
    ctx.font = "700 13px Pretendard, Noto Sans KR, sans-serif";
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    const w = ctx.measureText(text).width + 24;
    const x = WIDTH / 2 - w / 2;
    ctx.fillStyle = "rgba(9,12,17,0.72)";
    ctx.strokeStyle = "rgba(255,255,255,0.16)";
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.roundRect(x, 6, w, 24, 12);
    ctx.fill();
    ctx.stroke();
    ctx.fillStyle = pair.mine >= pair.theirs ? "#9dffb4" : "#ffb3b3";
    ctx.fillText(text, WIDTH / 2, 18);
    ctx.restore();
}

function drawGame() {

    drawBackground();

    const shakeOffset =
        getShakeOffset();

    const ox =
        recoil.x +
        shakeOffset.x;

    const oy =
        recoil.y +
        shakeOffset.y;

    ctx.save();

    ctx.translate(
        ox,
        oy
    );


    /* 격자 */

    ctx.strokeStyle =
        "rgba(255,255,255,0.055)";

    ctx.lineWidth = 1;

    for (
        let c = 0;
        c <= COLS;
        c++
    ) {

        ctx.beginPath();

        ctx.moveTo(
            c * CELL,
            0
        );

        ctx.lineTo(
            c * CELL,
            HEIGHT
        );

        ctx.stroke();
    }


    for (
        let r = 0;
        r <= ROWS;
        r++
    ) {

        ctx.beginPath();

        ctx.moveTo(
            0,
            r * CELL
        );

        ctx.lineTo(
            WIDTH,
            r * CELL
        );

        ctx.stroke();
    }


    /* =====================================================
       위험 블록
    ===================================================== */

    const dangerSkin =
        DANGER_SKINS[
            visualSettings.dangerSkin
        ].value;

    for (
        const danger
        of dangers
    ) {

        const {
            c,
            r
        } =
            parseKey(
                danger
            );

        drawDangerBlock(
            c,
            r,
            dangerSkin
        );
    }


    /* =====================================================
       목표 (도착 지점 스킨 설정 적용)
    ===================================================== */

    if (goal) {
        drawGoalSkin(
            getGoalSkinValue(),
            goal.c * CELL + 5,
            goal.r * CELL + 5,
            CELL - 10
        );
    }


    /* =====================================================
       벽
    ===================================================== */

    const drawAnimatedWallSet =
        (
            wallSet,
            isNewWall
        ) => {

            const scale =
                getWallScaleForTransition(
                    isNewWall
                );

            for (
                const wall
                of wallSet
            ) {

                const {
                    c,
                    r
                } =
                    parseKey(
                        wall
                    );

                if (
                    isBoundary(c, r)
                ) {
                    continue;
                }

                if (
                    scale <= 0.001
                ) {
                    continue;
                }

                const size =
                    CELL * scale;

                const offset =
                    (
                        CELL -
                        size
                    ) / 2;

                ctx.fillStyle =
                    getWallColor();

                ctx.fillRect(
                    c * CELL + offset,
                    r * CELL + offset,
                    size,
                    size
                );

                ctx.strokeStyle =
                    "rgba(255,255,255,0.05)";

                ctx.strokeRect(
                    c * CELL +
                    offset +
                    0.5,

                    r * CELL +
                    offset +
                    0.5,

                    Math.max(
                        0,
                        size - 1
                    ),

                    Math.max(
                        0,
                        size - 1
                    )
                );
            }
        };


    for (
        const wall
        of walls
    ) {

        const {
            c,
            r
        } =
            parseKey(
                wall
            );

        if (
            !isBoundary(c, r)
        ) {
            continue;
        }

        ctx.fillStyle =
            getWallColor();

        ctx.fillRect(
            c * CELL,
            r * CELL,
            CELL,
            CELL
        );

        ctx.strokeStyle =
            "rgba(255,255,255,0.05)";

        ctx.strokeRect(
            c * CELL + 0.5,
            r * CELL + 0.5,
            CELL - 1,
            CELL - 1
        );
    }


    if (
        mapTransition.active
    ) {

        drawAnimatedWallSet(
            mapTransition.oldWalls,
            false
        );

        drawAnimatedWallSet(
            mapTransition.newWalls,
            true
        );

    } else {

        drawAnimatedWallSet(
            walls,
            true
        );
    }


    /* =====================================================
       경로 안내 프로토콜
    ===================================================== */

    if (
        activeItem === "pathGuide" &&
        performance.now() < pathGuideVisibleUntil &&
        pathGuidePath.length > 1
    ) {
        const now = performance.now();
        const fadeStart =
            pathGuideFadeStart > 0
                ? pathGuideFadeStart
                : pathGuideAutoFadeAt;
        const fadeProgress =
            now >= fadeStart
                ? Math.min(1, (now - fadeStart) / (PATH_GUIDE_FADE_DURATION * 1000))
                : 0;
        const fadeAlpha = Math.max(0, 1 - fadeProgress);

        const pulse =
            (0.32 +
            0.48 *
            (0.5 + 0.5 * Math.sin(now * 0.012))) *
            fadeAlpha;

        ctx.save();
        ctx.lineWidth = 5;
        ctx.lineCap = "round";
        ctx.lineJoin = "round";
        ctx.strokeStyle = `rgba(120,220,255,${pulse})`;
        ctx.shadowBlur = 12;
        ctx.shadowColor = "#55cfff";

        ctx.beginPath();

        pathGuidePath.forEach((point, index) => {
            const x = point.c * CELL + CELL / 2;
            const y = point.r * CELL + CELL / 2;

            if (index === 0) ctx.moveTo(x, y);
            else ctx.lineTo(x, y);
        });

        ctx.stroke();

        ctx.shadowBlur = 0;
        ctx.fillStyle = `rgba(170,240,255,${pulse})`;

        for (let i = 0; i < pathGuidePath.length; i++) {
            if (i % 2 !== 0 && i !== pathGuidePath.length - 1) continue;
            const point = pathGuidePath[i];
            ctx.beginPath();
            ctx.arc(
                point.c * CELL + CELL / 2,
                point.r * CELL + CELL / 2,
                4,
                0,
                Math.PI * 2
            );
            ctx.fill();
        }

        ctx.restore();
    }


    /* =====================================================
       이동 흔적 (플레이어 잔상 설정 적용)
    ===================================================== */

    {
        const trailEffect = getPlayerTrailValue();
        const trailTime = performance.now() * 0.001;

        for (let i = 0; i < trail.length; i++) {
            const point = trail[i];
            const k = (i + 1) / trail.length * (point.life ?? 1);
            drawTrailPoint(trailEffect, point.x, point.y, k, i, trailTime);
        }
    }


    /* =====================================================
       상대 플레이어 - 주황색
    ===================================================== */

    if (multiplayerMatchActive && opponent.visible) {
        const opx = opponent.x + 7;
        const opy = opponent.y + 7;
        ctx.fillStyle = "#ff9f43";
        ctx.fillRect(opx, opy, CELL - 14, CELL - 14);
        ctx.strokeStyle = "#fff1d6";
        ctx.lineWidth = 2;
        ctx.strokeRect(opx, opy, CELL - 14, CELL - 14);
        ctx.fillStyle = "rgba(255,255,255,0.32)";
        ctx.fillRect(opx + 4, opy + 4, CELL - 22, 4);
        ctx.fillStyle = "#ffd29a";
        ctx.font = "bold 10px Pretendard, Noto Sans KR, sans-serif";
        ctx.textAlign = "center";
        ctx.textBaseline = "bottom";
        ctx.fillText("상대", opponent.x + CELL / 2, opponent.y - 3);
    }


    /* =====================================================
       플레이어 (스킨 설정 적용)
    ===================================================== */

    if (multiplayerPlayerVisible || !multiplayerMatchActive) {
        drawPlayerSkin(
            getPlayerSkinValue(),
            player.x + 5,
            player.y + 5,
            CELL - 10
        );
    }


    ctx.restore();


    /* =====================================================
       하단 메시지
    ===================================================== */

    if (
        messageText
    ) {

        ctx.fillStyle =
            "rgba(0,0,0,0.58)";

        ctx.fillRect(
            0,
            HEIGHT - 42,
            WIDTH,
            42
        );

        ctx.fillStyle =
            "#f3f5f7";

        ctx.font =
            "600 17px Pretendard, Noto Sans KR, sans-serif";

        ctx.textAlign =
            "center";

        ctx.textBaseline =
            "middle";

        ctx.fillText(
            messageText,
            WIDTH / 2,
            HEIGHT - 21
        );
    }


    /* =====================================================
       플래시
    ===================================================== */

    if (
        flash.alpha > 0
    ) {

        ctx.fillStyle =
            flash.color;

        ctx.globalAlpha =
            flash.alpha;

        ctx.fillRect(
            0,
            0,
            WIDTH,
            HEIGHT
        );

        ctx.globalAlpha = 1;
    }


    drawStreakEffect();
    drawMultiplayerScoreHUD();
}


/* =========================================================
   상점 / 설정
========================================================= */

function getShopButton() {
    return {
        x: 116,
        y: window.innerWidth <= 520 ? 112 : 74,
        w: 42,
        h: 42
    };
}

function drawShopButton() {
    const button = getShopButton();

    ctx.save();
    ctx.fillStyle = "rgba(9,12,17,0.68)";
    ctx.strokeStyle = "rgba(255,255,255,0.14)";
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.roundRect(button.x, button.y, button.w, button.h, 12);
    ctx.fill();
    ctx.stroke();

    ctx.fillStyle = "#f0f3f6";
    ctx.font = "bold 22px Arial, sans-serif";
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    drawClearEmoji("🛒", button.x + button.w / 2, button.y + button.h / 2 + 1, 25);
    ctx.restore();
}

function getStartSettingsButton() {

    return {
        x: 12,
        y: window.innerWidth <= 520 ? 112 : 74,
        w: 42,
        h: 42
    };
}


function isInsideRect(
    x,
    y,
    rect
) {

    return (
        x >= rect.x &&
        x <= rect.x + rect.w &&
        y >= rect.y &&
        y <= rect.y + rect.h
    );
}


function drawSettingsGear() {

    const button =
        getStartSettingsButton();

    ctx.save();

    ctx.fillStyle =
        "rgba(9,12,17,0.68)";

    ctx.strokeStyle =
        "rgba(255,255,255,0.14)";

    ctx.lineWidth = 1;

    ctx.beginPath();

    ctx.roundRect(
        button.x,
        button.y,
        button.w,
        button.h,
        12
    );

    ctx.fill();
    ctx.stroke();

    ctx.fillStyle =
        "#cbd4dc";

    ctx.font =
        "bold 25px Arial, sans-serif";

    ctx.textAlign =
        "center";

    ctx.textBaseline =
        "middle";

    ctx.fillText(
        "⚙",
        button.x +
        button.w / 2,
        button.y +
        button.h / 2 + 1
    );

    ctx.restore();
}


function drawSettingsButton(
    x,
    y,
    w,
    h,
    textValue
) {
    // 닉네임 박스와 동일한 공통 버튼 스타일
    ctx.save();
    ctx.fillStyle = "rgba(9,12,17,0.68)";
    ctx.strokeStyle = "rgba(255,255,255,0.14)";
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.roundRect(x, y, w, h, Math.min(9, h / 2));
    ctx.fill();
    ctx.stroke();

    ctx.fillStyle = "#cbd4dc";
    ctx.font = "700 15px Pretendard, Noto Sans KR, sans-serif";
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    ctx.fillText(textValue, x + w / 2, y + h / 2);
    ctx.restore();
}


/* =========================================================
   위험 블록 미리보기
========================================================= */

function drawDangerPreviewInBox(
    skin,
    box
) {
    const previewSize = 32;

    // 미리보기 박스의 정확한 가운데
    const previewX =
        box.x + (box.w - previewSize) / 2;

    const previewY =
        box.y + (box.h - previewSize) / 2;

    ctx.save();

    ctx.translate(
        previewX,
        previewY
    );

    ctx.scale(
        previewSize / CELL,
        previewSize / CELL
    );

    drawDangerBlock(
        0,
        0,
        skin
    );

    ctx.restore();
}

/* =========================================================
   상점 패널
========================================================= */

function drawShopPanel() {
    ctx.save();

    ctx.fillStyle = "rgba(0,0,0,0.76)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);

    const panel = getShopPanelRect();

    ctx.fillStyle = "#171c25";
    ctx.strokeStyle = "#394352";
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.roundRect(panel.x, panel.y, panel.w, panel.h, 20);
    ctx.fill();
    ctx.stroke();

    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    ctx.fillStyle = "#fff";
    ctx.font = "bold 28px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("🛒 아이템 상점", WIDTH / 2, 62);

    ctx.fillStyle = "#ffd76a";
    ctx.font = "700 18px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(`🪙 코인 ${coins}`, WIDTH / 2, 95);

    const types = ["timeClock", "energyShield", "pathGuide", "firstAid", "energyRecovery"];
    const pageCount = Math.max(1, Math.ceil(types.length / SHOP_PAGE_SIZE));
    shopPage = clamp(shopPage, 0, pageCount - 1);
    const pageTypes = types.slice(shopPage * SHOP_PAGE_SIZE, (shopPage + 1) * SHOP_PAGE_SIZE);

    // 페이지 화살표는 상점 양옆의 세로 중앙에 배치
    const arrowY = 276;
    // 화살표는 패널 안쪽에 완전히 들어오도록 배치
    drawSettingsButton(panel.x + 8, arrowY, 48, 48, "◀");
    drawSettingsButton(panel.x + panel.w - 56, arrowY, 48, 48, "▶");

    ctx.fillStyle = "#aeb8c5";
    ctx.font = "600 13px Pretendard, Noto Sans KR, sans-serif";
    const rowStart = 190;
    pageTypes.forEach((type, index) => {
        const y = rowStart + index * 108;
        const data = ITEM_DATA[type];
        const inventory = itemInventory[type];
        const price = ITEM_PRICES[type];
        const maxQty = getMaxAffordableQuantity(type);
        const qty = maxQty > 0 ? getPurchaseQuantity(type) : 0;
        const remaining = maxQty > 0 ? coins - qty * price : coins;

        ctx.fillStyle = "rgba(255,255,255,0.035)";
        ctx.strokeStyle = "rgba(255,255,255,0.12)";
        ctx.lineWidth = 1;
        ctx.beginPath();
        ctx.roundRect(panel.x + 65, y - 40, panel.w - 130, 92, 13);
        ctx.fill();
        ctx.stroke();

        ctx.textAlign = "left";
        ctx.fillStyle = "#f1f4f7";
        ctx.font = "700 16px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(`${data.icon} ${data.name}`, panel.x + 88, y - 18);

        ctx.fillStyle = "#9eabb9";
        ctx.font = "12px Pretendard, Noto Sans KR, sans-serif";
        if (type === "energyRecovery") {
            ctx.fillText("맵 넘기기 모두 소모 시 한 번만 작동 ·", panel.x + 88, y - 2);
            ctx.fillText("(1개 3회복 / 2개 5회복)", panel.x + 88, y + 14);
        } else {
            ctx.fillText(data.description, panel.x + 88, y + 5);
        }

        ctx.fillStyle = "#cbd4dc";
        ctx.font = "12px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(`보유 ${inventory}개 · 개당 ${price} 코인`, panel.x + 88, y + 27);

        // 구매 수량 조절
        drawSettingsButton(panel.x + 430, y - 25, 30, 34, "−");
        drawSettingsButton(panel.x + 464, y - 25, 50, 34, `${qty}`);
        drawSettingsButton(panel.x + 518, y - 25, 30, 34, "+");
        drawSettingsButton(panel.x + 550, y - 25, 90, 34, "구매");

        ctx.textAlign = "center";
        ctx.fillStyle = maxQty > 0 ? "#91e7b2" : "#7f8b99";
        ctx.font = "11px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(
            maxQty > 0
                ? `총 ${qty * price} 코인 · 구매 후 ${remaining} 코인 남음`
                : "구매 가능한 코인 부족",
            panel.x + 489,
            y + 25
        );
    });

    ctx.textAlign = "center";
    ctx.fillStyle = "#aeb8c5";
    ctx.font = "16px Arial, sans-serif";
    let dots = "";
    for (let i = 0; i < pageCount; i++) {
        dots += i === shopPage ? "●" : "○";
        if (i < pageCount - 1) dots += "  ";
    }
    ctx.fillText(dots, WIDTH / 2, 505);
    drawSettingsButton(WIDTH / 2 - 80, 550, 160, 26, "닫기");
    ctx.restore();
}

function getInventoryButton() {
    return { x: 64, y: window.innerWidth <= 520 ? 112 : 74, w: 42, h: 42 };
}

function drawInventoryButton() {
    const button = getInventoryButton();
    ctx.save();
    ctx.fillStyle = "rgba(9,12,17,0.68)";
    ctx.strokeStyle = "rgba(255,255,255,0.14)";
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.roundRect(button.x, button.y, button.w, button.h, 12);
    ctx.fill();
    ctx.stroke();
    ctx.fillStyle = "#f0f3f6";
    ctx.font = "bold 22px Arial, sans-serif";
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    drawClearEmoji("🎒", button.x + button.w / 2, button.y + button.h / 2 + 1, 25);
    ctx.restore();
}

function drawInventoryPanel() {
    ctx.save();
    ctx.fillStyle = "rgba(0,0,0,0.76)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);

    const panel = { x: 55, y: 55, w: 690, h: 490 };
    ctx.fillStyle = "#171c25";
    ctx.strokeStyle = "#394352";
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.roundRect(panel.x, panel.y, panel.w, panel.h, 20);
    ctx.fill();
    ctx.stroke();

    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    ctx.fillStyle = "#fff";
    ctx.font = "bold 28px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("🎒 인벤토리", WIDTH / 2, 98);

    const types = Object.keys(ITEM_DATA);
    const cols = 5;
    const size = 82;
    const gap = 20;
    const totalW = cols * size + (cols - 1) * gap;
    const startX = WIDTH / 2 - totalW / 2;
    const y = 185;

    types.forEach((type, index) => {
        const x = startX + index * (size + gap);
        const owned = itemInventory[type] > 0;
        const equipped = selectedItem === type;

        ctx.save();
        ctx.globalAlpha = owned ? 1 : 0.28;
        ctx.fillStyle = equipped ? "rgba(20,25,32,0.95)" : "rgba(255,255,255,0.07)";
        ctx.strokeStyle = equipped ? "rgba(120,220,255,0.75)" : "rgba(255,255,255,0.18)";
        ctx.lineWidth = equipped ? 2 : 1;
        ctx.beginPath();
        ctx.roundRect(x, y, size, size, 16);
        ctx.fill();
        ctx.stroke();

        ctx.font = "34px Arial, sans-serif";
        ctx.textAlign = "center";
        ctx.textBaseline = "middle";

        // ⏱️와 🛡️는 글리프의 실제 좌우 여백 때문에
        // 수학적인 중앙보다 오른쪽으로 보일 수 있으므로
        // 실제 글리프 경계를 기준으로 시각적 중앙에 맞춘다.
        let iconX = x + size / 2;
        if (type === "timeClock" || type === "energyShield") {
            const metrics = ctx.measureText(ITEM_DATA[type].icon);
            if (metrics.actualBoundingBoxLeft != null && metrics.actualBoundingBoxRight != null) {
                iconX += (metrics.actualBoundingBoxLeft - metrics.actualBoundingBoxRight) / 2;
            }
        }

        ctx.fillText(ITEM_DATA[type].icon, iconX, y + size / 2);

        if (equipped) {
            ctx.fillStyle = "#111820";
            ctx.beginPath();
            ctx.arc(x + size - 13, y + 13, 11, 0, Math.PI * 2);
            ctx.fill();
            ctx.fillStyle = "#7ddcff";
            ctx.font = "bold 15px Arial, sans-serif";
            ctx.fillText("✓", x + size - 13, y + 13);
        }
        ctx.restore();

        ctx.fillStyle = "#cbd4dc";
        ctx.font = "12px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(`${owned ? itemInventory[type] : 0}`, x + size / 2, y + size + 18);
    });

    ctx.fillStyle = "#aeb8c5";
    ctx.font = "13px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("아이콘을 눌러 아이템 설명과 장착 상태를 확인하세요.", WIDTH / 2, 345);

    if (selectedItem) {
        const label = ITEM_DATA[selectedItem].name +
            (selectedItem === "timeClock" ? ` × ${selectedTimeClocks}` : "");
        ctx.fillStyle = "#91e7b2";
        ctx.fillText(`현재 장착: ${label}`, WIDTH / 2, 375);
    } else {
        ctx.fillStyle = "#7f8b99";
        ctx.fillText("현재 장착된 아이템이 없습니다.", WIDTH / 2, 375);
    }

    drawSettingsButton(WIDTH / 2 - 80, 485, 160, 30, "닫기");
    ctx.restore();

    if (inventoryDetailType) drawInventoryDetailModal();
}

function drawInventoryDetailModal() {
    const type = inventoryDetailType;
    const data = ITEM_DATA[type];
    const owned = itemInventory[type];
    const equipped = selectedItem === type;
    const box = { x: 145, y: 145, w: 510, h: 320 };

    ctx.save();
    ctx.fillStyle = "rgba(0,0,0,0.52)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);

    ctx.fillStyle = "#171c25";
    ctx.strokeStyle = "#4b596b";
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.roundRect(box.x, box.y, box.w, box.h, 18);
    ctx.fill();
    ctx.stroke();

    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    // 이모지와 아이템 이름을 분리해서 각각 모달의 정중앙에 배치
    // 폰트마다 이모지의 실제 시각적 폭이 달라 한 줄로 묶으면
    // 아이콘이 중앙에서 살짝 치우쳐 보일 수 있으므로 별도로 그립니다.
    ctx.fillStyle = "#fff";
    ctx.font = "34px Arial, sans-serif";
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";

    // ⏱️와 🛡️는 글리프의 실제 좌우 여백 때문에
    // 수학적인 중앙보다 오른쪽으로 보일 수 있으므로
    // 실제 글리프 경계를 기준으로 시각적 중앙에 맞춘다.
    let detailIconX = box.x + box.w / 2;
    if (type === "timeClock" || type === "energyShield") {
        const metrics = ctx.measureText(data.icon);
        if (metrics.actualBoundingBoxLeft != null && metrics.actualBoundingBoxRight != null) {
            detailIconX += (metrics.actualBoundingBoxLeft - metrics.actualBoundingBoxRight) / 2;
        }
    }

    ctx.fillText(data.icon, detailIconX, 178);

    ctx.font = "bold 25px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(data.name, box.x + box.w / 2, 208);

    ctx.fillStyle = "#c5ced8";
    ctx.font = "15px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(data.description, box.x + box.w / 2, 245);
    ctx.fillText(`보유 ${owned}개`, box.x + box.w / 2, 278);

    if (type === "timeClock") {
        drawSettingsButton(310, 292, 42, 38, "−");
        drawSettingsButton(361, 292, 78, 38, `${selectedTimeClocks}개`);
        drawSettingsButton(446, 292, 42, 38, "+");
        ctx.fillStyle = "#9eabb9";
        ctx.font = "12px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("한 게임에서 최대 5개 사용", box.x + box.w / 2, 342);
    }

    if (type === "energyRecovery") {
        if (owned > 0) {
            selectedEnergyRecovery = Math.max(1, Math.min(2, selectedEnergyRecovery, owned));
        }
        drawSettingsButton(310, 292, 42, 38, "−");
        drawSettingsButton(361, 292, 78, 38, `${selectedEnergyRecovery}개`);
        drawSettingsButton(446, 292, 42, 38, "+");
        ctx.fillStyle = "#9eabb9";
        ctx.font = "12px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(
            `다음 사용: ${selectedEnergyRecovery}개 → 맵 넘기기 +${selectedEnergyRecovery === 1 ? 3 : 5}`,
            box.x + box.w / 2,
            342
        );
    }

    drawSettingsButton(410, 395, 100, 38, owned > 0 ? (equipped ? "해제" : "장착") : "보유하지 않음");
    drawSettingsButton(290, 395, 100, 38, "닫기");
    ctx.restore();
}

/* =========================================================
   상점 / 설정
========================================================= */

function getShopPanelRect() {
    return { x: 45, y: 15, w: 710, h: 570 };
}

/* =========================================================
   설정 패널
========================================================= */

function drawSettingsPanel() {
    ctx.save();
    ctx.fillStyle = "rgba(0,0,0,0.72)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);
    const panel = { x: 120, y: 65, w: 560, h: 455 };
    ctx.fillStyle = "#171c25";
    ctx.strokeStyle = "#394352";
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.roundRect(panel.x, panel.y, panel.w, panel.h, 20);
    ctx.fill(); ctx.stroke();
    ctx.textAlign = "center"; ctx.textBaseline = "middle";
    ctx.fillStyle = "#ffffff";
    ctx.font = "bold 28px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("⚙ 설정", WIDTH / 2, 108);
    ctx.fillStyle = "#aeb8c5";
    ctx.font = "600 15px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(`효과음 크기  ${Math.round(effectVolume * 100)}%`, WIDTH / 2, 175);
    const volumeBar = { x: WIDTH / 2 - 130, y: 195, w: 260, h: 8 };
    ctx.fillStyle = "rgba(255,255,255,0.10)";
    ctx.beginPath(); ctx.roundRect(volumeBar.x, volumeBar.y, volumeBar.w, volumeBar.h, 5); ctx.fill();
    ctx.fillStyle = "#7ddcff";
    ctx.beginPath(); ctx.roundRect(volumeBar.x, volumeBar.y, volumeBar.w * effectVolume, volumeBar.h, 5); ctx.fill();
    ctx.fillStyle = "#dfe5ea";
    ctx.beginPath(); ctx.arc(volumeBar.x + volumeBar.w * effectVolume, volumeBar.y + volumeBar.h / 2, 8, 0, Math.PI * 2); ctx.fill();

    ctx.fillText(`배경음악 크기  ${Math.round(musicVolume * 100)}%`, WIDTH / 2, 255);
    const musicBar = { x: WIDTH / 2 - 130, y: 275, w: 260, h: 8 };
    ctx.fillStyle = "rgba(255,255,255,0.10)";
    ctx.beginPath(); ctx.roundRect(musicBar.x, musicBar.y, musicBar.w, musicBar.h, 5); ctx.fill();
    ctx.fillStyle = "#7ddcff";
    ctx.beginPath(); ctx.roundRect(musicBar.x, musicBar.y, musicBar.w * musicVolume, musicBar.h, 5); ctx.fill();
    ctx.fillStyle = "#dfe5ea";
    ctx.beginPath(); ctx.arc(musicBar.x + musicBar.w * musicVolume, musicBar.y + musicBar.h / 2, 8, 0, Math.PI * 2); ctx.fill();

    drawSettingsButton(WIDTH / 2 - 130, 340, 260, 48, "🚪 로그아웃");
    drawSettingsButton(WIDTH / 2 - 80, 450, 160, 32, "닫기");
    ctx.restore();
}

function drawSkinPanel() {

    ctx.save();

    ctx.fillStyle = "rgba(0,0,0,0.72)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);

    const panel = SKIN_PANEL;

    ctx.fillStyle = "#171c25";
    ctx.strokeStyle = "#394352";
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.roundRect(panel.x, panel.y, panel.w, panel.h, 20);
    ctx.fill();
    ctx.stroke();

    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    ctx.fillStyle = "#ffffff";
    ctx.font = "bold 28px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("👔 스킨", WIDTH / 2, 58);

    SKIN_ROWS.forEach(row => {
        const centerY = row.centerY;
        const list = row.list;
        const selected = list[visualSettings[row.key]] || list[0];

        const selectedBox = {
            x: WIDTH / 2 - 155,
            y: centerY - 21,
            w: 310,
            h: 42
        };

        ctx.fillStyle = "#aeb8c5";
        ctx.font = "600 15px Pretendard, Noto Sans KR, sans-serif";
        ctx.textAlign = "center";
        ctx.textBaseline = "middle";
        ctx.fillText(row.label, WIDTH / 2, centerY - 32);

        drawSettingsButton(panel.x + 24, centerY - 21, 62, 42, "◀");
        drawSettingsButton(panel.x + panel.w - 86, centerY - 21, 62, 42, "▶");

        /* 벽 / 배경 색상 */
        if (row.key === "wall" || row.key === "background") {
            const displayColor = row.key === "wall" ? getWallColor() : getBackgroundColor();

            ctx.fillStyle = displayColor;
            ctx.beginPath();
            ctx.roundRect(selectedBox.x, selectedBox.y, selectedBox.w, selectedBox.h, 10);
            ctx.fill();

            const hex = displayColor.replace("#", "");
            const r = parseInt(hex.slice(0, 2), 16);
            const g = parseInt(hex.slice(2, 4), 16);
            const b = parseInt(hex.slice(4, 6), 16);
            const luminance = (r * 299 + g * 587 + b * 114) / 1000;

            ctx.fillStyle = luminance > 145 ? "#101318" : "#ffffff";
            ctx.font = "600 16px Pretendard, Noto Sans KR, sans-serif";
            ctx.textAlign = "center";
            ctx.textBaseline = "middle";
            ctx.fillText(selected.name, WIDTH / 2, centerY);

            if (selected.custom) {
                ctx.font = "11px Pretendard, Noto Sans KR, sans-serif";
                ctx.fillStyle = luminance > 145 ? "rgba(16,19,24,0.72)" : "rgba(255,255,255,0.72)";
                ctx.fillText("눌러서 색상 코드 입력", WIDTH / 2, centerY + 15);
            }

            ctx.strokeStyle = "rgba(255,255,255,0.34)";
            ctx.lineWidth = 1.5;
            ctx.beginPath();
            ctx.roundRect(selectedBox.x, selectedBox.y, selectedBox.w, selectedBox.h, 10);
            ctx.stroke();
            return;
        }

        /* 연속 클리어 효과 */
        if (row.key === "streakEffect") {
            drawEffectPreviewInBox(selected.value, selected.name, selectedBox);
            return;
        }

        /* 잔상: 움직이는 미리보기 */
        if (row.key === "playerTrail") {
            drawTrailPreviewInBox(selected.value, selected.name, selectedBox);
            return;
        }

        /* 위험 블록 / 플레이어 스킨: 왼쪽에 미리보기, 가운데에 이름 */
        ctx.fillStyle = "rgba(255,255,255,0.055)";
        ctx.strokeStyle = "rgba(255,255,255,0.16)";
        ctx.lineWidth = 1;
        ctx.beginPath();
        ctx.roundRect(selectedBox.x, selectedBox.y, selectedBox.w, selectedBox.h, 10);
        ctx.fill();
        ctx.stroke();

        if (row.key === "dangerSkin") {
            drawDangerPreviewInBox(selected.value, {
                x: selectedBox.x + 14,
                y: selectedBox.y + 5,
                w: 32,
                h: 32
            });
        } else if (row.key === "playerSkin") {
            drawPlayerSkin(selected.value, selectedBox.x + 15, selectedBox.y + 6, 30);
        } else if (row.key === "goalSkin") {
            drawGoalSkin(selected.value, selectedBox.x + 15, selectedBox.y + 6, 30);
        }

        ctx.fillStyle = "#f0f3f6";
        ctx.font = "600 15px Pretendard, Noto Sans KR, sans-serif";
        ctx.textAlign = "center";
        ctx.textBaseline = "middle";
        ctx.fillText(selected.name, WIDTH / 2 + 10, centerY);
    });

    {
        const themeIndex = getCurrentSkinThemeIndex();
        drawSettingsButton(
            SKIN_THEME_BUTTON.x, SKIN_THEME_BUTTON.y, SKIN_THEME_BUTTON.w, SKIN_THEME_BUTTON.h,
            `🎨 테마: ${themeIndex >= 0 ? SKIN_THEMES[themeIndex].name : "직접 설정"} ▶`
        );
    }
    drawSettingsButton(WIDTH / 2 - 80, 550, 160, 26, "닫기");

    ctx.restore();
}


/* =========================================================
   연속 효과 미리보기
========================================================= */

function drawEffectPreviewInBox(effect, name, box) {
    if (effect !== "none" && STREAK_RENDERERS[effect]) {
        ctx.save();
        ctx.translate(box.x, box.y);
        ctx.scale(box.w / WIDTH, box.h / HEIGHT);
        ctx.beginPath();
        ctx.rect(0, 0, WIDTH, HEIGHT);
        ctx.rect(12, 12, WIDTH - 24, HEIGHT - 24);
        ctx.clip("evenodd");
        STREAK_RENDERERS[effect](3.5);
        ctx.restore();
    }
    ctx.save();
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    ctx.fillStyle = "rgba(255,255,255,0.94)";
    ctx.font = "600 15px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(effect === "none" ? "효과 없음" : name, WIDTH / 2, box.y + box.h / 2);
    ctx.restore();
}


/* =========================================================
   설정 터치
========================================================= */


function handleQuestRewardTap(x, y) {
    // 완료된 퀘스트의 보상은 실제 HTML <button>만 처리합니다.
    // Canvas 좌표 판정은 제거하여 iPad 터치와 중복 실행을 방지합니다.
    return false;
}

function handleSkinSettingTap(x, y) {
    const panel = SKIN_PANEL;

    if (isInsideRect(x, y, SKIN_THEME_BUTTON)) {
        cycleSkinTheme();
        return true;
    }

    for (const row of SKIN_ROWS) {
        const centerY = row.centerY;

        if ((row.key === "wall" || row.key === "background") &&
            row.list[visualSettings[row.key]]?.custom &&
            isInsideRect(x, y, { x: WIDTH / 2 - 155, y: centerY - 21, w: 310, h: 42 })) {
            setCustomColor(row.key);
            return true;
        }
        if (isInsideRect(x, y, { x: panel.x + 24, y: centerY - 21, w: 62, h: 42 })) {
            cycleSetting(row.key, row.list, -1);
            return true;
        }
        if (isInsideRect(x, y, { x: panel.x + panel.w - 86, y: centerY - 21, w: 62, h: 42 })) {
            cycleSetting(row.key, row.list, 1);
            return true;
        }
    }
    return true;
}

function handleSettingsTap(x, y) {
    refreshDailyQuestIfNeeded();
    const questButton = getQuestButton();
    const skinButton = getSkinButton();
    const shopButton = getShopButton();
    const inventoryButton = getInventoryButton();
    const gear = getStartSettingsButton();

    // 2인용 메뉴가 열려 있으면 다른 시작 화면 기능보다 먼저 처리
    if (multiplayerOpen) {
        const multiplayerPanel = { x: 135, y: 80, w: 530, h: 440 };
        if (x < multiplayerPanel.x || x > multiplayerPanel.x + multiplayerPanel.w || y < multiplayerPanel.y || y > multiplayerPanel.y + multiplayerPanel.h) {
            closeMultiplayerMenu();
            return true;
        }
        if (multiplayerMatchmaking) {
            if (isInsideRect(x, y, { x: 205, y: 345, w: 390, h: 48 })) {
                cancelMultiplayerMatchmaking();
                return true;
            }
            return true;
        } else if (!multiplayerRole) {
            if (isInsideRect(x, y, { x: 205, y: 205, w: 390, h: 52 })) {
                startMultiplayerMatchmaking();
                return true;
            }
            if (isInsideRect(x, y, { x: 205, y: 275, w: 390, h: 52 })) {
                createMultiplayerRoom();
                return true;
            }
            if (isInsideRect(x, y, { x: 205, y: 345, w: 390, h: 52 })) {
                joinMultiplayerRoom();
                return true;
            }
            if (isInsideRect(x, y, { x: 305, y: 415, w: 190, h: 42 })) {
                closeMultiplayerMenu();
                return true;
            }
        } else if (multiplayerRole === "host") {
            if (isInsideRect(x, y, { x: 305, y: 292, w: 190, h: 38 })) {
                copyMultiplayerRoomCode();
                return true;
            }
            if (isInsideRect(x, y, { x: 205, y: 365, w: 180, h: 48 })) {
                if (multiplayerPeerJoined) startMultiplayerMatch();
                return true;
            }
            if (isInsideRect(x, y, { x: 415, y: 365, w: 180, h: 48 })) {
                multiplayerRoomCode = generateRoomCode();
                multiplayerSeed = generateMatchSeed();
                multiplayerPeerJoined = false;
                connectMultiplayerSocket(() => {
                    multiplayerMatchType = "friend";
                    multiplayerSend({ type: "create", room: multiplayerRoomCode });
                });
                return true;
            }
            if (isInsideRect(x, y, { x: 205, y: 430, w: 390, h: 42 })) {
                closeMultiplayerMenu();
                return true;
            }
        } else {
            if (isInsideRect(x, y, { x: 205, y: 345, w: 180, h: 48 })) {
                joinMultiplayerRoom();
                return true;
            }
            if (isInsideRect(x, y, { x: 415, y: 345, w: 180, h: 48 })) {
                closeMultiplayerMenu();
                return true;
            }
        }
        return true;
    }

    if (!shopOpen && !inventoryOpen && !settingsOpen && !multiplayerOpen && !questOpen && !skinOpen && isInsideRect(x, y, skinButton)) {
        skinOpen = true;
        requestSettingsRender();
        return true;
    }

    if (!shopOpen && !inventoryOpen && !settingsOpen && !multiplayerOpen && !questOpen && isInsideRect(x, y, questButton)) {
        questOpen = true;
        syncQuestRewardOverlay(true);
        return true;
    }

    if (questOpen) {
        refreshDailyQuestIfNeeded();

        if (handleQuestRewardTap(x, y)) {
            return true;
        }

        if (isInsideRect(x, y, { x: WIDTH / 2 - 105, y: 410, w: 210, h: 38 })) {
            rerollDailyQuests();
            return true;
        }
        if (isInsideRect(x, y, { x: WIDTH / 2 - 80, y: 465, w: 160, h: 32 })) {
            questOpen = false;
            syncQuestRewardOverlay(true);
            return true;
        }
        if (x < 35 || x > 765 || y < 25 || y > 575) {
            questOpen = false;
            syncQuestRewardOverlay(true);
        }
        return true;
    }

    if (!shopOpen && !inventoryOpen && !settingsOpen && !multiplayerOpen && isInsideRect(x, y, shopButton)) {
        shopOpen = true;
        shopPage = 0;
        return true;
    }

    if (!shopOpen && !inventoryOpen && !settingsOpen && isInsideRect(x, y, inventoryButton)) {
        inventoryOpen = true;
        inventoryDetailType = null;
        return true;
    }

    if (inventoryOpen) {
        const panel = { x: 55, y: 55, w: 690, h: 490 };

        if (inventoryDetailType) {
            const box = { x: 145, y: 145, w: 510, h: 320 };

            // 상세창 바깥의 빈 공간을 누르면 상세창만 닫고
            // 인벤토리 화면은 그대로 유지합니다.
            if (x < box.x || x > box.x + box.w || y < box.y || y > box.y + box.h) {
                closeInventoryDetail();
                return true;
            }

            // 상세창의 닫기 버튼
            if (isInsideRect(x, y, { x: 290, y: 395, w: 100, h: 38 })) {
                closeInventoryDetail();
                return true;
            }

            // 장착 / 해제
            if (isInsideRect(x, y, { x: 410, y: 395, w: 100, h: 38 })) {
                if (selectedItem === inventoryDetailType) unequipItem();
                else if (itemInventory[inventoryDetailType] > 0) equipItem(inventoryDetailType);
                closeInventoryDetail();
                return true;
            }

            if (inventoryDetailType === "timeClock") {
                if (isInsideRect(x, y, { x: 310, y: 292, w: 42, h: 38 })) {
                    adjustSelectedTimeClocks(-1);
                    return true;
                }
                if (isInsideRect(x, y, { x: 446, y: 292, w: 42, h: 38 })) {
                    adjustSelectedTimeClocks(1);
                    return true;
                }
            }

            if (inventoryDetailType === "energyRecovery") {
                if (isInsideRect(x, y, { x: 310, y: 292, w: 42, h: 38 })) {
                    adjustSelectedEnergyRecovery(-1);
                    return true;
                }
                if (isInsideRect(x, y, { x: 446, y: 292, w: 42, h: 38 })) {
                    adjustSelectedEnergyRecovery(1);
                    return true;
                }
            }
            return true;
        }

        if (x < panel.x || x > panel.x + panel.w || y < panel.y || y > panel.y + panel.h) {
            closeInventoryDetail();
            inventoryOpen = false;
            return true;
        }

        if (isInsideRect(x, y, { x: WIDTH / 2 - 80, y: 485, w: 160, h: 30 })) {
            inventoryOpen = false;
            return true;
        }

        const types = Object.keys(ITEM_DATA);
        const cols = 5;
        const size = 82;
        const gap = 20;
        const totalW = cols * size + (cols - 1) * gap;
        const startX = WIDTH / 2 - totalW / 2;
        const iconY = 185;
        types.forEach((type, index) => {
            const ix = startX + index * (size + gap);
            if (isInsideRect(x, y, { x: ix, y: iconY, w: size, h: size })) {
                openInventoryDetail(type);
            }
        });
        return true;
    }

    if (skinOpen) {
        const panel = { x: 70, y: 20, w: 660, h: 560 };
        if (isInsideRect(x, y, { x: WIDTH / 2 - 80, y: 550, w: 160, h: 26 })) {
            skinOpen = false; requestSettingsRender(); return true;
        }
        if (x < panel.x || x > panel.x + panel.w || y < panel.y || y > panel.y + panel.h) {
            skinOpen = false; requestSettingsRender(); return true;
        }
        return handleSkinSettingTap(x, y);
    }

    if (shopOpen) {
        const panel = getShopPanelRect();
        const types = ["timeClock", "energyShield", "pathGuide", "firstAid", "energyRecovery"];
        const pageCount = Math.max(1, Math.ceil(types.length / SHOP_PAGE_SIZE));
        const pageTypes = types.slice(shopPage * SHOP_PAGE_SIZE, (shopPage + 1) * SHOP_PAGE_SIZE);

        if (isInsideRect(x, y, { x: WIDTH / 2 - 80, y: 550, w: 160, h: 26 })) {
            shopOpen = false;
            return true;
        }
        if (isInsideRect(x, y, { x: panel.x + 8, y: 276, w: 48, h: 48 })) {
            shopPage = (shopPage - 1 + pageCount) % pageCount;
            return true;
        }
        if (isInsideRect(x, y, { x: panel.x + panel.w - 56, y: 276, w: 48, h: 48 })) {
            shopPage = (shopPage + 1) % pageCount;
            return true;
        }
        if (x < panel.x || x > panel.x + panel.w || y < panel.y || y > panel.y + panel.h) {
            shopOpen = false;
            return true;
        }

        const rowStart = 205;
        pageTypes.forEach((type, index) => {
            const cy = rowStart + index * 108;
            if (isInsideRect(x, y, { x: panel.x + 430, y: cy - 25, w: 30, h: 34 })) adjustPurchaseQuantity(type, -1);
            if (isInsideRect(x, y, { x: panel.x + 464, y: cy - 25, w: 50, h: 34 })) return;
            if (isInsideRect(x, y, { x: panel.x + 518, y: cy - 25, w: 30, h: 34 })) adjustPurchaseQuantity(type, 1);
            if (isInsideRect(x, y, { x: panel.x + 550, y: cy - 25, w: 90, h: 34 })) requestBuyItem(type);
        });
        return true;
    }

    if (!settingsOpen && isInsideRect(x, y, { x: 570, y: 58, w: 200, h: 38 })) {
        withGuestName(openMultiplayerMenu);
        return true;
    }

    if (!settingsOpen && isInsideRect(x, y, gear)) {
        settingsOpen = true;
        requestSettingsRender();
        positionVolumeTouchArea();
        return true;
    }

    if (!settingsOpen) return false;

    const settingsPanel = { x: 120, y: 65, w: 560, h: 455 };
    if (isInsideRect(x, y, { x: WIDTH / 2 - 80, y: 450, w: 160, h: 32 })) {
        settingsOpen = false;
        positionVolumeTouchArea();
        return true;
    }
    if (isInsideRect(x, y, { x: WIDTH / 2 - 130, y: 340, w: 260, h: 48 })) {
        logoutToEntry();
        return true;
    }
    if (x < settingsPanel.x || x > settingsPanel.x + settingsPanel.w || y < settingsPanel.y || y > settingsPanel.y + settingsPanel.h) {
        settingsOpen = false;
        positionVolumeTouchArea();
        return true;
    }
    return true;
}

/* =========================================================
   시작 화면
========================================================= */

function drawStartScreen() {

    drawBackground();

    ctx.save();

    ctx.textAlign =
        "center";

    ctx.textBaseline =
        "middle";


    ctx.fillStyle =
        "#f3f5f7";

    ctx.font =
        "bold 48px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        "슬라이딩",
        WIDTH / 2,
        100
    );


    ctx.fillStyle =
        "#8f9aa8";

    ctx.font =
        "600 20px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        "끝 없는 미로 탈출",
        WIDTH / 2,
        145
    );


    ctx.fillStyle =
        "#dfe5ea";

    ctx.font =
        "600 18px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        "키보드 조작 : W A S D 를 눌러 이동",
        WIDTH / 2,
        205
    );

    ctx.fillText(
        "모바일 조작 : 화면을 쓸어 이동",
        WIDTH / 2,
        240
    );

    ctx.fillText(
        "맵 넘기기 : 더블 터치",
        WIDTH / 2,
        275
    );

    ctx.fillStyle =
        "#8995a3";

    ctx.font =
        "15px Pretendard, Noto Sans KR, sans-serif";

    // 홈 화면에서는 개인 최고 기록 2줄만 숨깁니다.
    // 기록 변수와 저장 기능은 게임 오버/점수 시스템에서 그대로 유지합니다.

    ctx.fillStyle =
        "#dfe5ea";

    ctx.font =
        "600 17px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        "최근 기록",
        WIDTH / 2,
        455
    );


    ctx.font =
        "14px Pretendard, Noto Sans KR, sans-serif";


    if (
        recentRecords.length === 0
    ) {

        ctx.fillStyle =
            "#697584";

        ctx.fillText(
            "아직 기록이 없습니다.",
            WIDTH / 2,
            480
        );

    } else {

        recentRecords.forEach(
            (
                record,
                index
            ) => {

                const y =
                    480 +
                    index * 15;

                ctx.fillStyle =
                    "#aeb8c4";

                ctx.fillText(
                    `${
                        record.startTime ||
                        record.time ||
                        "--:--"
                    } ~ ${
                        record.endTime ||
                        "--:--"
                    }　${
                        record.clears
                    }회 클리어　최대 연속 ${
                        record.maxStreak
                    }회`,

                    WIDTH / 2,
                    y
                );
            }
        );
    }


    ctx.fillStyle =
        "#ffffff";

    ctx.font =
        "bold 20px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        "키 사용 또는 더블 터치로 시작",
        WIDTH / 2,
        420
    );


    drawQuestButton();
    drawSkinButton();
    drawShopButton();
    drawInventoryButton();
    drawSettingsGear();


    if (questOpen) {
        drawQuestPanel();
    } else if (shopOpen) {
        drawShopPanel();
    } else if (inventoryOpen) {
        drawInventoryPanel();
    } else if (skinOpen) {
        drawSkinPanel();
    } else if (settingsOpen) {
        drawSettingsPanel();
    } else if (multiplayerOpen) {
        drawMultiplayerMenu();
    }


    ctx.restore();
}


/* =========================================================
   게임 오버
========================================================= */

function drawGameOverScreen() {

    ctx.fillStyle =
        "#090b10";

    ctx.fillRect(
        0,
        0,
        WIDTH,
        HEIGHT
    );


    const shakeOffset =
        getShakeOffset();

    const ox =
        recoil.x +
        shakeOffset.x;

    const oy =
        recoil.y +
        shakeOffset.y;


    ctx.save();

    ctx.translate(
        ox,
        oy
    );

    ctx.textAlign =
        "center";

    ctx.textBaseline =
        "middle";


    ctx.fillStyle =
        "#ff4d5d";

    ctx.font =
        "bold 56px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        "GAME OVER",
        WIDTH / 2,
        150
    );


    ctx.fillStyle =
        "#f1f4f7";

    ctx.font =
        "600 22px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        `클리어 기록 : ${clearCount}회`,
        WIDTH / 2,
        245
    );

    ctx.fillText(
        `최대 연속 클리어 기록 : ${maxClearStreak}회`,
        WIDTH / 2,
        285
    );

    ctx.fillStyle =
        "#ffd76a";

    ctx.font =
        "bold 28px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        `최종 점수 : ${calculateV28Score().toLocaleString("ko-KR")}점`,
        WIDTH / 2,
        335
    );


    ctx.fillStyle =
        "#7ddcff";

    ctx.fillText(
        `전체 최고 연속 클리어 : ${allTimeBestStreak}회`,
        WIDTH / 2,
        375
    );


    ctx.fillStyle =
        "#8d98a6";

    ctx.font =
        "16px Pretendard, Noto Sans KR, sans-serif";

    ctx.fillText(
        "R 또는 SPACE : 시작 화면",
        WIDTH / 2,
        430
    );

    ctx.fillText(
        "G 또는 Space, 또는 화면 더블 터치로 시작 화면으로 돌아갑니다.",
        WIDTH / 2,
        470
    );


    ctx.restore();


    if (
        flash.alpha > 0
    ) {

        ctx.fillStyle =
            flash.color;

        ctx.globalAlpha =
            flash.alpha;

        ctx.fillRect(
            0,
            0,
            WIDTH,
            HEIGHT
        );

        ctx.globalAlpha = 1;
    }
}


function drawSpectatorBanner() {
    ctx.save();
    const text = "👁 관전 중";
    ctx.font = "700 13px Pretendard, Noto Sans KR, sans-serif";
    ctx.textAlign = "left";
    ctx.textBaseline = "middle";
    const w = ctx.measureText(text).width + 24;
    ctx.fillStyle = "rgba(9,12,17,0.72)";
    ctx.strokeStyle = "rgba(255,215,106,0.55)";
    ctx.lineWidth = 1;
    ctx.beginPath();
    ctx.roundRect(10, 6, w, 24, 12);
    ctx.fill();
    ctx.stroke();
    ctx.fillStyle = "#ffd76a";
    ctx.fillText(text, 22, 18);
    ctx.restore();
}

function drawMultiplayerResultScreen() {
    drawBackground();
    ctx.save();
    ctx.fillStyle = "rgba(5,8,13,0.90)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);
    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    const title = gameState === "multiplayerWaitingResult" ? "경기 결과 대기 중" :
        multiplayerResult === multiplayerRole ? "승리!" : multiplayerResult === "draw" ? "무승부" : "패배";
    ctx.fillStyle = "#f3f5f7";
    ctx.font = "bold 46px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(title, WIDTH / 2, 205);
    ctx.fillStyle = "#aeb8c4";
    ctx.font = "600 18px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(gameState === "multiplayerWaitingResult" ? "상대 플레이어가 아직 플레이 중입니다. 경기가 끝날 때까지 기다려 주세요." : "2인용 경쟁 경기가 종료되었습니다.", WIDTH / 2, 270);
    ctx.fillStyle = "#7ddcff";
    ctx.font = "600 16px Pretendard, Noto Sans KR, sans-serif";
    if ((gameState === "multiplayerResult" && multiplayerFinalScores) || gameState === "multiplayerWaitingResult") {
        const pair = getMultiplayerScorePair(multiplayerFinalScores || multiplayerScores);
        ctx.fillStyle = "#ffd76a";
        ctx.font = "bold 26px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(`내 점수 ${pair.mine.toLocaleString("ko-KR")}  :  ${pair.theirs.toLocaleString("ko-KR")} 상대 점수`, WIDTH / 2, 325);
        ctx.fillStyle = "#8d98a6";
        ctx.font = "14px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText("둘 다 목숨을 잃으면 점수가 더 높은 플레이어가, 5000점에 먼저 도달하면 그 플레이어가 승리합니다.", WIDTH / 2, 362);
    }
    if (multiplayerRoomCode) {
        ctx.fillStyle = "#7ddcff";
        ctx.font = "600 16px Pretendard, Noto Sans KR, sans-serif";
        ctx.fillText(`방 코드 ${multiplayerRoomCode}`, WIDTH / 2, 405);
    }
    ctx.fillStyle = "#ffffff";
    ctx.font = "bold 18px Pretendard, Noto Sans KR, sans-serif";
    if (gameState === "multiplayerResult") ctx.fillText("Space 또는 화면 터치로 시작 화면으로", WIDTH / 2, 470);
    ctx.restore();
}


function drawEnergyRecoveryChoice() {
    if (!energyRecoveryChoiceOpen) return;

    ctx.save();
    ctx.fillStyle = "rgba(0,0,0,0.62)";
    ctx.fillRect(0, 0, WIDTH, HEIGHT);

    const box = { x: 155, y: 205, w: 490, h: 190 };
    ctx.fillStyle = "#171c25";
    ctx.strokeStyle = "#4b596b";
    ctx.lineWidth = 2;
    ctx.beginPath();
    ctx.roundRect(box.x, box.y, box.w, box.h, 18);
    ctx.fill();
    ctx.stroke();

    ctx.textAlign = "center";
    ctx.textBaseline = "middle";
    ctx.fillStyle = "#f3f5f7";
    ctx.font = "bold 23px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("🌀 에너지 복구 장치", WIDTH / 2, 240);

    ctx.fillStyle = "#aeb8c4";
    ctx.font = "14px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText("맵 넘기기를 모두 소모했습니다. 몇 개 사용할까요?", WIDTH / 2, 275);

    const canUse2 = itemInventory.energyRecovery >= 2;
    drawSettingsButton(205, 310, 160, 42, "1개 사용 · +3");
    if (canUse2) {
        drawSettingsButton(435, 310, 160, 42, "2개 사용 · +5");
    } else {
        drawSettingsButton(435, 310, 160, 42, "2개 사용 불가");
    }

    ctx.fillStyle = "#7f8b99";
    ctx.font = "12px Pretendard, Noto Sans KR, sans-serif";
    ctx.fillText(`현재 보유량: ${itemInventory.energyRecovery}개 · 이 게임에서는 1회만 사용 가능`, WIDTH / 2, 370);
    ctx.restore();
}

/* =========================================================
   렌더링
========================================================= */

function draw(now = performance.now()) {

    if (
        gameState === "start"
    ) {

        updateStartMenuOverlay();
        syncQuestRewardOverlay();

        // 설정 화면은 정적인 UI이므로 내용이 바뀔 때만 다시 그립니다.
        // 미리보기의 모양/강도는 그대로 유지하면서, 매 프레임 반복되는
        // Canvas 연산을 없애 화살표 입력 시 발생하는 순간적인 지연을 줄입니다.
        if (questOpen) {
            drawStartScreen();
        } else if (settingsOpen || skinOpen) {
            const previewFrameInterval = 1000 / 24;

            if (
                !settingsRenderRequested &&
                now - lastSettingsRenderTime < previewFrameInterval
            ) {
                return;
            }

            settingsRenderRequested = false;
            lastSettingsRenderTime = now;
            drawBackground();
            if (skinOpen) drawSkinPanel();
            else drawSettingsPanel();
        } else {
            drawStartScreen();
        }

        return;
    }


    if (gameState !== "start") {
        syncQuestRewardOverlay(true);
    }

    if (
        gameState === "gameover"
    ) {

        drawGameOverScreen();

        return;
    }

    if (gameState === "multiplayerWaitingResult" && multiplayerMatchActive && multiplayerSelfDead) {
        drawGame();
        drawSpectatorBanner();
        return;
    }
    if (gameState === "multiplayerResult" || gameState === "multiplayerWaitingResult") {
        drawMultiplayerResultScreen();
        return;
    }
    if (gameState === "expResult") {
        drawExperienceResultScreen(now);
        return;
    }

    drawGame();
    if (gameState === "tutorial") {
        drawTutorialOverlay();
    } else {
        drawEnergyRecoveryChoice();
        if (gameState === "countdown") drawIntroCountdown(now);
    }
}


/* =========================================================
   메인 루프
========================================================= */

/* 캔버스 해상도 자동 조절 (PC에서 크게 표시할 때 선명도 개선) */
function updateCanvasResolution(now) {
    if (now - lastResolutionCheck < 400) return;
    lastResolutionCheck = now;

    const isDesktop = window.matchMedia("(hover: hover) and (pointer: fine)").matches;
    const rect = canvas.getBoundingClientRect();
    if (rect.width <= 0) return;

    let nextScale = 1;
    if (isDesktop) {
        const dpr = window.devicePixelRatio || 1;
        nextScale = Math.min(2, Math.max(1, (rect.width / WIDTH) * dpr));
        nextScale = Math.round(nextScale * 4) / 4;
    }

    if (nextScale !== renderScale) {
        renderScale = nextScale;
        canvas.width = Math.round(WIDTH * renderScale);
        canvas.height = Math.round(HEIGHT * renderScale);
        // width/height 변경은 캔버스를 초기화하므로 컨텍스트 변환은 매 프레임 다시 설정합니다.
        settingsRenderRequested = true;
    }
}

function gameLoop(
    now
) {

    let delta =
        (
            now -
            lastTime
        ) / 1000;

    lastTime =
        now;

    delta =
        Math.min(
            delta,
            0.05
        );

    update(delta);

    // 게임 상태에 맞춰 배경음악을 시작/정지합니다.
    syncBackgroundMusic();

    updateCanvasResolution(now);
    ctx.setTransform(renderScale, 0, 0, renderScale, 0, 0);

    draw(now);

    requestAnimationFrame(
        gameLoop
    );
}


/* =========================================================
   V28 초기 계정 진입 화면
========================================================= */

function refreshRankingAccountLabel() {
    const el = document.getElementById("rankingAccountLabel");
    if (!el) return;
    el.textContent = currentAccount
        ? `로그인 계정: ${currentAccount.nickname || currentAccount.id || "회원"}`
        : `게스트: ${guestAccount?.nickname || "준비 중..."}`;
}

const originalOpenRankingPanel = openRankingPanel;
openRankingPanel = function(mode = "today") {
    if (!currentAccount && !guestMode) return;
    refreshRankingAccountLabel();
    originalOpenRankingPanel(mode);
};

/* =========================================================
   초기 실행
========================================================= */

function setLoginScreenLock(locked) {
    const html = document.documentElement;
    const body = document.body;
    if (!html || !body) return;

    html.classList.toggle("login-lock", !!locked);
    body.classList.toggle("login-lock", !!locked);

    if (locked) {
        // iPad Safari can retain the previous scroll offset when an overlay appears.
        // Reset it while the login screen owns the viewport.
        window.scrollTo(0, 0);
    }
}

const loginViewportGuard = event => {
    const gate = document.getElementById("entryGate");
    if (!gate || gate.style.display === "none" || gate.classList.contains("session-checking")) return;
    event.preventDefault();
};

document.addEventListener("touchmove", loginViewportGuard, { passive: false });
document.addEventListener("gesturestart", loginViewportGuard, { passive: false });
document.addEventListener("gesturechange", loginViewportGuard, { passive: false });
document.addEventListener("gestureend", loginViewportGuard, { passive: false });

async function restoreSavedSession() {
    loadSavedLoginId();

    // 저장된 세션 확인 중에는 로그인 화면을 숨겨 두어
    // iPad에서 로그인 화면이 잠깐 보이거나 그 순간의 터치가
    // 게임 시작 입력으로 이어지는 문제를 막습니다.
    const gate = document.getElementById("entryGate");
    if (gate) {
        gate.classList.add("session-checking");
        gate.style.display = "flex";
    }

    try {
        const data = await apiJSON("/api/me");
        const account = data?.user || data?.account || data;
        if (account && (account.id || account.nickname)) {
            enterGameAsAccount(account);
            return;
        }
    } catch (error) {}

    showEntryGate();
    updateUI();
}


const entryGateObserver = new MutationObserver(() => {
    const gate = document.getElementById("entryGate");
    if (!gate) return;
    const visible = getComputedStyle(gate).display !== "none" && !gate.classList.contains("session-checking");
    setLoginScreenLock(visible);
});

entryGateObserver.observe(document.documentElement, {
    subtree: true,
    attributes: true,
    attributeFilter: ["style", "class"]
});


/* =========================================================
   화면 맞춤 (모바일 가로 모드 등 화면 높이가 낮을 때)
   - 게임 전체를 800x644 기준으로 두고 화면에 맞게 통째로 축소합니다.
   - 터치 좌표는 getBoundingClientRect 기반이라 그대로 정확합니다.
========================================================= */
function fitGameToViewport() {
    const w = window.innerWidth;
    const h = window.innerHeight;
    const NEED_W = 800;
    const NEED_H = 644;
    const root = document.documentElement;

    // 마우스/정밀 포인터를 사용하는 PC에서만 확대를 허용합니다.
    const isDesktop = window.matchMedia("(hover: hover) and (pointer: fine)").matches;
    const MAX_UPSCALE = 2.5;
    const raw = Math.min(w / NEED_W, h / NEED_H);
    const needsShrink = (w < NEED_W || h < NEED_H) && w > h;
    const needsGrow = isDesktop && raw > 1.02;
    const useFit = needsShrink || needsGrow;
    const scale = needsGrow
        ? Math.min(raw * 0.97, MAX_UPSCALE)
        : Math.min(raw, 1);

    root.classList.toggle("fit-scale", useFit);
    root.style.setProperty("--fit-scale", String(scale));

    if (typeof positionVolumeTouchArea === "function") positionVolumeTouchArea();
}

window.addEventListener("resize", fitGameToViewport);
window.addEventListener("orientationchange", () => setTimeout(fitGameToViewport, 200));
if (window.visualViewport) window.visualViewport.addEventListener("resize", fitGameToViewport);
fitGameToViewport();

restoreSavedSession();

requestAnimationFrame(
    gameLoop
);

</script>

</body>
    </html>
    

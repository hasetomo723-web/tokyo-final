<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>HASETOMO. ONE MAN LIVE TOUR 2026 ~ REVOLUTION ~</title>
  <meta name="description" content="HASETOMO. ONE MAN LIVE TOUR 2026 ~ REVOLUTION ~ チケットプレイガイド・公演日程まとめページ" />

  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,600;0,800;0,900;1,800&family=Noto+Sans+JP:wght@400;500;700;900&family=Oswald:wght@500;700&display=swap" rel="stylesheet" />

  <style>
    /* =========================================
       ベースリセット & カラー変数
       ========================================= */
    :root {
      --bg-base: #08080a;
      --bg-card: #121216;
      --bg-card-ended: #0d0d10;
      --border-subtle: #27272a;
      --text-primary: #f4f4f5;
      --text-secondary: #a1a1aa;
      --text-muted: #71717a;
      --accent-orange: #ff7b00;
      --accent-amber: #ff9e00;
      --eplus-pink: #eb0065;
      --ltike-blue: #0068b7;
      --pia-cyan: #0099d9;
    }

    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      background-color: var(--bg-base);
      background-image:
        radial-gradient(circle at 50% 0%, rgba(255, 123, 0, 0.14) 0%, rgba(8, 8, 10, 0) 60%),
        linear-gradient(to right, rgba(255, 255, 255, 0.025) 1px, transparent 1px),
        linear-gradient(to bottom, rgba(255, 255, 255, 0.025) 1px, transparent 1px);
      background-size: 100% 100%, 32px 32px, 32px 32px;
      color: var(--text-primary);
      font-family: "Noto Sans JP", -apple-system, BlinkMacSystemFont, sans-serif;
      line-height: 1.5;
      min-height: 100vh;
      overflow-x: hidden;
      -webkit-font-smoothing: antialiased;
      -webkit-tap-highlight-color: transparent;
    }

    /* =========================================
       背景の稲妻デコレーション
       ========================================= */
    .bg-lightning-wrap {
      position: fixed;
      inset: 0;
      pointer-events: none;
      overflow: hidden;
      z-index: 0;
    }

    .lightning-svg {
      position: absolute;
      animation: flashGlow 3.5s ease-in-out infinite;
    }

    .lightning-top {
      top: -3rem;
      right: -4rem;
      width: 24rem;
      height: 24rem;
      color: rgba(255, 255, 255, 0.09);
    }

    .lightning-bottom {
      bottom: 2.5rem;
      left: -5rem;
      width: 20rem;
      height: 20rem;
      color: rgba(255, 123, 0, 0.09);
      animation-delay: 1.6s;
    }

    @keyframes flashGlow {
      0%, 100% { opacity: 0.35; }
      50% { opacity: 0.8; }
    }

    /* =========================================
       メインレイアウトコンテナ
       ========================================= */
    .container {
      position: relative;
      z-index: 1;
      width: 100%;
      max-width: 600px;
      margin: 0 auto;
      padding: 16px 16px 64px;
    }

    @media (min-width: 640px) {
      .container {
        padding-top: 32px;
      }
    }

    /* =========================================
       ヒーローセクション（TOP画像 + タイトル）
       ========================================= */
    .hero-card {
      background-color: var(--bg-card);
      border: 1px solid rgba(39, 39, 42, 0.95);
      border-radius: 18px;
      overflow: hidden;
      box-shadow: 0 24px 50px rgba(0, 0, 0, 0.85);
    }

    .hero-media {
      position: relative;
      width: 100%;
      background-color: #18181b;
      overflow: hidden;
    }

    .hero-media img {
      width: 100%;
      height: auto;
      display: block;
      transition: transform 0.6s ease;
    }

    .hero-card:hover .hero-media img {
      transform: scale(1.015);
    }

    .hero-gradient-fade {
      position: absolute;
      left: 0;
      right: 0;
      bottom: 0;
      height: 56px;
      background: linear-gradient(to top, var(--bg-card) 0%, rgba(18, 18, 22, 0.5) 55%, transparent 100%);
      pointer-events: none;
    }

    .hero-header {
      padding: 14px 20px 24px;
      background-color: var(--bg-card);
    }

    @media (min-width: 640px) {
      .hero-header {
        padding: 16px 28px 28px;
      }
    }

    .tour-title {
      font-family: "Montserrat", sans-serif;
      font-weight: 900;
      font-size: 1.55rem;
      line-height: 1.2;
      letter-spacing: -0.02em;
      color: #ffffff;
    }

    .tour-title-sub {
      display: block;
      font-size: 1.125rem;
      font-weight: 800;
      color: #e4e4e7;
      margin-top: 2px;
    }

    .tour-title-accent {
      display: inline-block;
      font-size: 1.35rem;
      font-style: italic;
      font-weight: 900;
      letter-spacing: 0.03em;
      margin-top: 4px;
      background: linear-gradient(90deg, var(--accent-orange) 0%, var(--accent-amber) 50%, #ff6a00 100%);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }

    @media (min-width: 640px) {
      .tour-title {
        font-size: 1.875rem;
      }
      .tour-title-sub {
        font-size: 1.35rem;
      }
      .tour-title-accent {
        font-size: 1.6rem;
      }
    }

    /* =========================================
       共通セクション見出し
       ========================================= */
    .section-block {
      margin-top: 32px;
    }

    .section-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 4px;
      margin-bottom: 14px;
    }

    .section-title-group {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .section-bar {
      width: 4px;
      height: 20px;
      border-radius: 999px;
      background-color: var(--accent-orange);
    }

    .section-title {
      font-family: "Montserrat", sans-serif;
      font-weight: 800;
      font-size: 1.05rem;
      letter-spacing: 0.06em;
      color: #ffffff;
      text-transform: uppercase;
    }

    .section-title-jp {
      font-family: "Noto Sans JP", sans-serif;
      font-size: 0.75rem;
      font-weight: 700;
      color: var(--text-secondary);
      margin-left: 6px;
    }

    .section-note {
      font-size: 0.7rem;
      color: var(--text-muted);
      font-weight: 500;
    }

    /* =========================================
       チケットプレイガイドリンクカード
       ========================================= */
    .ticket-list {
      display: flex;
      flex-direction: column;
      gap: 14px;
    }

    .ticket-card {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
      padding: 16px 18px;
      border-radius: 16px;
      background: linear-gradient(135deg, #16161c 0%, #121216 100%);
      border: 1px solid var(--border-subtle);
      text-decoration: none;
      color: inherit;
      overflow: hidden;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.45);
      transition: transform 0.2s cubic-bezier(0.22, 1, 0.36, 1), border-color 0.2s ease, box-shadow 0.2s ease;
    }

    @media (min-width: 640px) {
      .ticket-card {
        padding: 18px 22px;
      }
    }

    .ticket-card:hover {
      transform: translateY(-2px);
    }

    .ticket-card:active {
      transform: scale(0.985);
    }

    .ticket-card-left {
      display: flex;
      align-items: center;
      gap: 14px;
    }

    .ticket-badge {
      width: 50px;
      height: 50px;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
      font-family: "Montserrat", sans-serif;
      font-weight: 900;
      transition: background-color 0.2s ease, color 0.2s ease, border-color 0.2s ease;
    }

    @media (min-width: 640px) {
      .ticket-badge {
        width: 56px;
        height: 56px;
      }
    }

    .ticket-name-row {
      display: flex;
      align-items: center;
      gap: 8px;
      flex-wrap: wrap;
    }

    .ticket-name {
      font-weight: 900;
      font-size: 1.05rem;
      color: #ffffff;
      transition: color 0.2s ease;
    }

    @media (min-width: 640px) {
      .ticket-name {
        font-size: 1.125rem;
      }
    }

    .ticket-tag {
      font-family: "Montserrat", sans-serif;
      font-size: 0.625rem;
      font-weight: 700;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      padding: 2px 7px;
      border-radius: 5px;
      background-color: rgba(39, 39, 42, 0.95);
      color: #d4d4d8;
      border: 1px solid rgba(63, 63, 70, 0.8);
    }

    .ticket-desc {
      font-size: 0.75rem;
      color: var(--text-secondary);
      margin-top: 3px;
    }

    .ticket-arrow {
      width: 36px;
      height: 36px;
      border-radius: 999px;
      background-color: rgba(39, 39, 42, 0.85);
      color: #d4d4d8;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
      transition: background-color 0.2s ease, color 0.2s ease, transform 0.2s ease;
    }

    .ticket-card:hover .ticket-arrow svg {
      transform: translate(2px, -2px);
    }

    /* イープラス固有カラー */
    .card-eplus:hover {
      border-color: rgba(235, 0, 101, 0.75);
      box-shadow: 0 10px 30px rgba(235, 0, 101, 0.2);
    }
    .card-eplus .ticket-badge {
      background-color: rgba(235, 0, 101, 0.15);
      border: 1px solid rgba(235, 0, 101, 0.45);
      color: #ff2e88;
      font-size: 1.35rem;
    }
    .card-eplus:hover .ticket-badge,
    .card-eplus:hover .ticket-arrow {
      background-color: var(--eplus-pink);
      border-color: var(--eplus-pink);
      color: #ffffff;
    }
    .card-eplus:hover .ticket-name {
      color: #ff5ca3;
    }

    /* ローチケ固有カラー */
    .card-ltike:hover {
      border-color: rgba(0, 104, 183, 0.85);
      box-shadow: 0 10px 30px rgba(0, 104, 183, 0.24);
    }
    .card-ltike .ticket-badge {
      background-color: rgba(0, 104, 183, 0.2);
      border: 1px solid rgba(0, 104, 183, 0.5);
      color: #38a1f3;
      font-size: 1rem;
    }
    .card-ltike:hover .ticket-badge,
    .card-ltike:hover .ticket-arrow {
      background-color: var(--ltike-blue);
      border-color: var(--ltike-blue);
      color: #ffffff;
    }
    .card-ltike:hover .ticket-name {
      color: #5ab4ff;
    }

    /* チケットぴあ固有カラー */
    .card-pia:hover {
      border-color: rgba(0, 153, 217, 0.85);
      box-shadow: 0 10px 30px rgba(0, 153, 217, 0.22);
    }
    .card-pia .ticket-badge {
      background-color: rgba(0, 153, 217, 0.16);
      border: 1px solid rgba(0, 153, 217, 0.45);
      color: #2ec2ff;
      font-size: 1.05rem;
    }
    .card-pia:hover .ticket-badge,
    .card-pia:hover .ticket-arrow {
      background-color: var(--pia-cyan);
      border-color: var(--pia-cyan);
      color: #ffffff;
    }
    .card-pia:hover .ticket-name {
      color: #5cd1ff;
    }

    /* =========================================
       ツアースケジュール一覧
       ========================================= */
    .schedule-count {
      font-family: "Montserrat", sans-serif;
      font-size: 0.7rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      color: var(--accent-orange);
    }

    .schedule-box {
      background-color: var(--bg-card);
      border: 1px solid rgba(39, 39, 42, 0.9);
      border-radius: 16px;
      overflow: hidden;
      box-shadow: 0 16px 36px rgba(0, 0, 0, 0.55);
    }

    .schedule-item {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      padding: 14px 16px;
      border-bottom: 1px solid rgba(39, 39, 42, 0.75);
    }

    .schedule-item:last-child {
      border-bottom: none;
    }

    @media (min-width: 640px) {
      .schedule-item {
        padding: 15px 22px;
      }
    }

    /* 公演終了アイテム */
    .schedule-item.is-ended {
      background-color: rgba(9, 9, 11, 0.65);
      opacity: 0.58;
    }

    .schedule-left {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 8px 12px;
    }

    .schedule-date-wrap {
      display: flex;
      align-items: baseline;
      gap: 6px;
    }

    .schedule-date {
      font-family: "Oswald", sans-serif;
      font-weight: 700;
      font-size: 1.05rem;
      letter-spacing: 0.03em;
      color: #a1a1aa;
      text-decoration: line-through;
      text-decoration-color: #52525b;
    }

    .schedule-day {
      font-family: "Montserrat", sans-serif;
      font-size: 0.7rem;
      font-weight: 700;
      color: #71717a;
    }

    .status-ended-badge {
      display: inline-flex;
      align-items: center;
      padding: 2px 8px;
      border-radius: 5px;
      font-size: 0.65rem;
      font-weight: 700;
      background-color: #27272a;
      color: #a1a1aa;
      border: 1px solid #3f3f46;
    }

    .schedule-right {
      text-align: right;
    }

    .schedule-city {
      font-family: "Montserrat", sans-serif;
      font-weight: 800;
      font-size: 0.9rem;
      letter-spacing: 0.05em;
      color: #a1a1aa;
    }

    .schedule-venue {
      display: block;
      font-size: 0.72rem;
      color: #71717a;
      margin-top: 1px;
    }

    @media (min-width: 640px) {
      .schedule-venue {
        display: inline;
        margin-left: 8px;
      }
    }

    /* ファイナル / 今後の公演ハイライト */
    .schedule-item.is-final {
      padding-top: 18px;
      padding-bottom: 18px;
      background: linear-gradient(90deg, rgba(255, 123, 0, 0.16) 0%, rgba(255, 123, 0, 0.04) 60%, transparent 100%);
    }

    .band-set-badge {
      display: inline-block;
      font-family: "Montserrat", sans-serif;
      font-size: 0.625rem;
      font-weight: 900;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      padding: 2px 8px;
      border-radius: 4px;
      background-color: var(--accent-orange);
      color: #09090b;
      margin-bottom: 4px;
    }

    .schedule-item.is-final .schedule-date {
      font-size: 1.2rem;
      color: #ffffff;
      text-decoration: none;
    }

    .schedule-item.is-final .schedule-day {
      font-size: 0.78rem;
      color: var(--accent-orange);
    }

    .schedule-item.is-final .schedule-city {
      font-size: 1.05rem;
      font-weight: 900;
      color: var(--accent-orange);
    }

    .schedule-item.is-final .schedule-venue {
      display: block;
      margin-left: 0;
      font-size: 0.78rem;
      font-weight: 500;
      color: #e4e4e7;
      margin-top: 2px;
    }

    /* =========================================
       シェアボタン & フッター
       ========================================= */
    .share-wrap {
      margin-top: 32px;
      display: flex;
      justify-content: center;
    }

    .share-btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 11px 22px;
      border-radius: 999px;
      background-color: #141418;
      border: 1px solid #2e2e34;
      color: #d4d4d8;
      font-family: inherit;
      font-size: 0.78rem;
      font-weight: 600;
      cursor: pointer;
      box-shadow: 0 6px 18px rgba(0, 0, 0, 0.4);
      transition: background-color 0.2s ease, color 0.2s ease, transform 0.15s ease;
    }

    .share-btn:hover {
      background-color: #1f1f25;
      color: #ffffff;
    }

    .share-btn:active {
      transform: scale(0.96);
    }

    .share-btn svg {
      color: var(--accent-orange);
    }

    .site-footer {
      margin-top: 40px;
      padding-top: 24px;
      border-top: 1px solid rgba(39, 39, 42, 0.75);
      text-align: center;
    }

    .footer-title {
      font-family: "Montserrat", sans-serif;
      font-size: 0.72rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      color: #71717a;
      text-transform: uppercase;
    }

    .footer-copy {
      font-size: 0.68rem;
      color: #52525b;
      margin-top: 6px;
    }

    /* =========================================
       トースト通知（URLコピー完了時）
       ========================================= */
    .copy-toast {
      position: fixed;
      bottom: 24px;
      left: 50%;
      transform: translate(-50%, 14px);
      z-index: 50;
      pointer-events: none;
      opacity: 0;
      transition: opacity 0.25s ease, transform 0.25s ease;
    }

    .copy-toast.is-visible {
      opacity: 1;
      transform: translate(-50%, 0);
    }

    .copy-toast-inner {
      display: flex;
      align-items: center;
      gap: 8px;
      padding: 10px 18px;
      border-radius: 999px;
      background-color: rgba(20, 20, 24, 0.96);
      border: 1px solid rgba(255, 123, 0, 0.65);
      color: #ffffff;
      font-size: 0.76rem;
      font-weight: 600;
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.75);
      white-space: nowrap;
    }

    .copy-toast-inner svg {
      color: var(--accent-orange);
      flex-shrink: 0;
    }
  </style>
</head>
<body>

  <!-- 背景稲妻アクセント -->
  <div class="bg-lightning-wrap" aria-hidden="true">
    <svg class="lightning-svg lightning-top" viewBox="0 0 200 200" fill="none">
      <path d="M120 10L65 95H110L85 190L155 85H105L120 10Z" stroke="currentColor" stroke-width="0.8" />
    </svg>
    <svg class="lightning-svg lightning-bottom" viewBox="0 0 200 200" fill="none">
      <path d="M90 15L40 105H85L65 185L135 85H90L90 15Z" stroke="currentColor" stroke-width="0.8" />
    </svg>
  </div>

  <main class="container">

    <!-- ヒーローセクション：TOP画像 & タイトル -->
    <header class="hero-card">
      <div class="hero-media">
        <img
          src="./はせとも2026ツアー横.webp"
          alt="HASETOMO. ONE MAN LIVE TOUR 2026 ~ REVOLUTION ~"
        />
        <div class="hero-gradient-fade"></div>
      </div>

      <div class="hero-header">
        <h1 class="tour-title">
          HASETOMO.
          <span class="tour-title-sub">ONE MAN LIVE TOUR 2026</span>
          <span class="tour-title-accent">~ REVOLUTION ~</span>
        </h1>
      </div>
    </header>

    <!-- チケットプレイガイド リンクセクション -->
    <section class="section-block" aria-labelledby="ticket-heading">
      <div class="section-header">
        <div class="section-title-group">
          <span class="section-bar"></span>
          <h2 id="ticket-heading" class="section-title">
            TICKET <span class="section-title-jp">チケット購入</span>
          </h2>
        </div>
        <span class="section-note">外部サイトへ移動します</span>
      </div>

      <div class="ticket-list">
        <!-- 1. イープラス -->
        <a
          href="https://eplus.jp/sf/detail/4369350001"
          target="_blank"
          rel="noopener noreferrer"
          class="ticket-card card-eplus"
        >
          <div class="ticket-card-left">
            <div class="ticket-badge">e+</div>
            <div>
              <div class="ticket-name-row">
                <span class="ticket-name">イープラス</span>
                <span class="ticket-tag">eplus</span>
              </div>
              <p class="ticket-desc">チケット申し込み・詳細はこちら</p>
            </div>
          </div>
          <div class="ticket-arrow" aria-hidden="true">
            <svg width="16" height="16" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M7 17L17 7M17 7H8M17 7V16" />
            </svg>
          </div>
        </a>

        <!-- 2. ローチケ -->
        <a
          href="https://l-tike.com/concert/mevent/?mid=797133"
          target="_blank"
          rel="noopener noreferrer"
          class="ticket-card card-ltike"
        >
          <div class="ticket-card-left">
            <div class="ticket-badge">L-tike</div>
            <div>
              <div class="ticket-name-row">
                <span class="ticket-name">ローチケ</span>
                <span class="ticket-tag">LAWSON TICKET</span>
              </div>
              <p class="ticket-desc">ローソンチケット 公演ページへ</p>
            </div>
          </div>
          <div class="ticket-arrow" aria-hidden="true">
            <svg width="16" height="16" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M7 17L17 7M17 7H8M17 7V16" />
            </svg>
          </div>
        </a>

        <!-- 3. チケットぴあ -->
        <a
          href="https://t.pia.jp/pia/event/event.do?eventBundleCd=b2671909"
          target="_blank"
          rel="noopener noreferrer"
          class="ticket-card card-pia"
        >
          <div class="ticket-card-left">
            <div class="ticket-badge">PIA</div>
            <div>
              <div class="ticket-name-row">
                <span class="ticket-name">チケットぴあ</span>
                <span class="ticket-tag">TICKET PIA</span>
              </div>
              <p class="ticket-desc">チケットぴあ 公演ページへ</p>
            </div>
          </div>
          <div class="ticket-arrow" aria-hidden="true">
            <svg width="16" height="16" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.2" d="M7 17L17 7M17 7H8M17 7V16" />
            </svg>
          </div>
        </a>
      </div>
    </section>

    <!-- ツアースケジュール一覧セクション -->
    <section class="section-block" aria-labelledby="schedule-heading">
      <div class="section-header">
        <div class="section-title-group">
          <span class="section-bar"></span>
          <h2 id="schedule-heading" class="section-title">
            SCHEDULE <span class="section-title-jp">公演日程</span>
          </h2>
        </div>
        <span class="schedule-count">ALL 9 SHOWS</span>
      </div>

      <div class="schedule-box">
        <!-- 1. CHIBA (公演終了) -->
        <div class="schedule-item is-ended">
          <div class="schedule-left">
            <div class="schedule-date-wrap">
              <span class="schedule-date">2026.9.12</span>
              <span class="schedule-day">(Sat)</span>
            </div>
            <span class="status-ended-badge">公演終了</span>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">CHIBA</span>
            <span class="schedule-venue">KASHIWA PALOOZA</span>
          </div>
        </div>

        <!-- 2. SENDAI (公演終了) -->
        <div class="schedule-item is-ended">
          <div class="schedule-left">
            <div class="schedule-date-wrap">
              <span class="schedule-date">2026.9.19</span>
              <span class="schedule-day">(Sat)</span>
            </div>
            <span class="status-ended-badge">公演終了</span>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">SENDAI</span>
            <span class="schedule-venue">enn2nd</span>
          </div>
        </div>

        <!-- 3. NAGOYA (公演終了) -->
        <div class="schedule-item is-ended">
          <div class="schedule-left">
            <div class="schedule-date-wrap">
              <span class="schedule-date">2026.9.26</span>
              <span class="schedule-day">(Sat)</span>
            </div>
            <span class="status-ended-badge">公演終了</span>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">NAGOYA</span>
            <span class="schedule-venue">X-HALL -ZEN-</span>
          </div>
        </div>

        <!-- 4. OSAKA (公演終了) -->
        <div class="schedule-item is-ended">
          <div class="schedule-left">
            <div class="schedule-date-wrap">
              <span class="schedule-date">2026.10.10</span>
              <span class="schedule-day">(Sat)</span>
            </div>
            <span class="status-ended-badge">公演終了</span>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">OSAKA</span>
            <span class="schedule-venue">ROCKTOWN</span>
          </div>
        </div>

        <!-- 5. HIROSHIMA (公演終了) -->
        <div class="schedule-item is-ended">
          <div class="schedule-left">
            <div class="schedule-date-wrap">
              <span class="schedule-date">2026.10.12</span>
              <span class="schedule-day">(Mon)</span>
            </div>
            <span class="status-ended-badge">公演終了</span>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">HIROSHIMA</span>
            <span class="schedule-venue">Yise</span>
          </div>
        </div>

        <!-- 6. SHIZUOKA (公演終了) -->
        <div class="schedule-item is-ended">
          <div class="schedule-left">
            <div class="schedule-date-wrap">
              <span class="schedule-date">2026.10.24</span>
              <span class="schedule-day">(Sat)</span>
            </div>
            <span class="status-ended-badge">公演終了</span>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">SHIZUOKA</span>
            <span class="schedule-venue">LIVE ROXY SHIZUOKA</span>
          </div>
        </div>

        <!-- 7. FUKUOKA (公演終了) -->
        <div class="schedule-item is-ended">
          <div class="schedule-left">
            <div class="schedule-date-wrap">
              <span class="schedule-date">2026.11.7</span>
              <span class="schedule-day">(Sat)</span>
            </div>
            <span class="status-ended-badge">公演終了</span>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">FUKUOKA</span>
            <span class="schedule-venue">LIVE HOUSE evoL</span>
          </div>
        </div>

        <!-- 8. HOKKAIDO (公演終了) -->
        <div class="schedule-item is-ended">
          <div class="schedule-left">
            <div class="schedule-date-wrap">
              <span class="schedule-date">2026.11.14</span>
              <span class="schedule-day">(Sat)</span>
            </div>
            <span class="status-ended-badge">公演終了</span>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">HOKKAIDO</span>
            <span class="schedule-venue">Pigsty</span>
          </div>
        </div>

        <!-- 9. TOKYO (Band Set) -->
        <div class="schedule-item is-final">
          <div>
            <span class="band-set-badge">Band Set</span>
            <div class="schedule-date-wrap">
              <span class="schedule-date">2027.1.29</span>
              <span class="schedule-day">(Fri)</span>
            </div>
          </div>
          <div class="schedule-right">
            <span class="schedule-city">TOKYO</span>
            <span class="schedule-venue">HULIC HALL TOKYO</span>
          </div>
        </div>
      </div>
    </section>

    <!-- URLコピー シェアボタン -->
    <div class="share-wrap">
      <button type="button" class="share-btn" onclick="copyPageUrl()">
        <svg width="16" height="16" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z" />
        </svg>
        <span>このページのURLをコピーしてシェア</span>
      </button>
    </div>

    <!-- フッター -->
    <footer class="site-footer">
      <p class="footer-title">HASETOMO. ONE MAN LIVE TOUR 2026 ~ REVOLUTION ~</p>
      <p class="footer-copy">&copy; 2026 HASETOMO. All Rights Reserved.</p>
    </footer>
  </main>

  <!-- コピー完了通知トースト -->
  <div id="copy-toast" class="copy-toast" role="status" aria-live="polite">
    <div class="copy-toast-inner">
      <svg width="16" height="16" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7" />
      </svg>
      <span>URLをクリップボードにコピーしました</span>
    </div>
  </div>

  <script>
    let toastTimer = null;

    function copyPageUrl() {
      const urlToCopy = window.location.href;
      const tempInput = document.createElement('textarea');
      tempInput.value = urlToCopy;
      tempInput.setAttribute('readonly', '');
      tempInput.style.position = 'absolute';
      tempInput.style.left = '-9999px';
      document.body.appendChild(tempInput);
      tempInput.select();

      try {
        document.execCommand('copy');
        showToast();
      } catch (err) {
        console.error('URLコピーに失敗しました:', err);
      } finally {
        document.body.removeChild(tempInput);
      }
    }

    function showToast() {
      const toast = document.getElementById('copy-toast');
      if (!toast) return;

      toast.classList.add('is-visible');
      if (toastTimer) clearTimeout(toastTimer);
      toastTimer = setTimeout(() => {
        toast.classList.remove('is-visible');
      }, 2500);
    }
  </script>
</body>
</html>

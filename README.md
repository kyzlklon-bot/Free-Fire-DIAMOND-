<!DOCTYPE html>
<html lang="kk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>FF Diamond</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@2.44.0/tabler-icons.min.css">

<!-- ============================================= -->
<!-- ADSTERRA POPUNDER — сайт ашылғанда бір рет шығады -->
<!-- ============================================= -->
<script type="text/javascript" src="https://www.effectivecpmnetwork.com/hsefgs7ghq?key=3599484f35ede989aec9a3a494d6a72c"></script>
<!-- ============================================= -->

<style>
*{box-sizing:border-box;margin:0;padding:0;font-family:'Segoe UI',sans-serif;}
body{background:#000;display:flex;justify-content:center;align-items:flex-start;min-height:100vh;}
:root{
  --ff-bg:#0a0e1a;--ff-card:#12192b;--ff-card2:#1a2340;
  --ff-orange:#ff6b00;--ff-orange2:#ff9900;--ff-blue:#00cfff;
  --ff-green:#00ff88;--ff-gold:#ffd700;--ff-text:#e8eaf0;
  --ff-muted:#7a8599;--ff-pink:#ff3d8c;--ff-purple:#9b59ff;
}
#app{width:390px;min-height:100vh;background:var(--ff-bg);color:var(--ff-text);overflow:hidden;position:relative;}

/* LOGIN */
#loginPage{position:fixed;inset:0;z-index:100;display:flex;flex-direction:column;align-items:center;justify-content:center;background:linear-gradient(160deg,#0a0e1a 0%,#0d1a33 60%,#1a0d2a 100%);padding:32px 24px;}
#loginPage.hidden{display:none;}
.login-logo{font-size:64px;margin-bottom:10px;text-align:center;}
.login-title{font-size:30px;font-weight:800;color:var(--ff-blue);letter-spacing:2px;margin-bottom:4px;text-align:center;}
.login-sub{font-size:13px;color:var(--ff-muted);margin-bottom:40px;text-align:center;}
.google-btn{width:100%;max-width:320px;background:#fff;border:none;border-radius:14px;padding:16px 22px;display:flex;align-items:center;gap:16px;cursor:pointer;transition:transform 0.15s,box-shadow 0.15s;box-shadow:0 4px 24px rgba(0,0,0,0.4);}
.google-btn:active{transform:scale(0.97);}
.google-icon{width:24px;height:24px;flex-shrink:0;}
.google-btn-text{font-size:16px;font-weight:700;color:#1a1a1a;}
.google-btn-sub{font-size:11px;color:#666;margin-top:2px;}
.login-note{font-size:10px;color:var(--ff-muted);margin-top:22px;text-align:center;line-height:1.7;}
.login-diamonds{display:flex;gap:8px;margin-bottom:30px;justify-content:center;}
.login-diamonds span{font-size:28px;animation:float 2s ease-in-out infinite;}
.login-diamonds span:nth-child(2){animation-delay:0.3s;}
.login-diamonds span:nth-child(3){animation-delay:0.6s;}
@keyframes float{0%,100%{transform:translateY(0);}50%{transform:translateY(-8px);}}

/* MAIN */
.page{display:none;flex-direction:column;min-height:100vh;}
.page.active{display:flex;}
.topbar{background:linear-gradient(135deg,#1a2a4a,#0d1a33);padding:16px 18px;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid rgba(0,207,255,0.15);}
.topbar-title{font-size:17px;font-weight:700;color:var(--ff-blue);}
.diamond-badge{background:linear-gradient(135deg,#1e3a6e,#0d2548);border:1px solid var(--ff-blue);border-radius:20px;padding:6px 14px;display:flex;align-items:center;gap:6px;font-size:14px;font-weight:700;color:var(--ff-gold);}
.nav{display:flex;background:#0d1424;border-top:1px solid rgba(0,207,255,0.1);position:sticky;bottom:0;}
.nav-btn{flex:1;padding:11px 4px;text-align:center;font-size:10px;color:var(--ff-muted);cursor:pointer;border:none;background:none;transition:all 0.2s;}
.nav-btn.active{color:var(--ff-orange);border-top:2px solid var(--ff-orange);}
.nav-btn i{display:block;font-size:22px;margin-bottom:2px;}
.content{flex:1;overflow-y:auto;padding:16px;}

/* ADS */
.ad-hero{background:linear-gradient(135deg,#1a3a6e,#0d2040);border:1px solid rgba(0,207,255,0.2);border-radius:16px;padding:22px;text-align:center;margin-bottom:16px;}
.ad-hero h2{font-size:19px;font-weight:700;color:var(--ff-blue);margin-bottom:6px;}
.ad-hero p{font-size:12px;color:var(--ff-muted);}
.ad-reward{font-size:30px;font-weight:800;color:var(--ff-gold);margin:10px 0;}
.ad-box{background:var(--ff-card);border:1px solid rgba(255,107,0,0.3);border-radius:12px;padding:16px;margin-bottom:12px;display:flex;align-items:center;gap:12px;}
.ad-box-icon{width:54px;height:54px;background:linear-gradient(135deg,#ff6b00,#ff9900);border-radius:12px;display:flex;align-items:center;justify-content:center;font-size:26px;flex-shrink:0;}
.ad-box-info h3{font-size:14px;font-weight:600;margin-bottom:3px;}
.ad-box-info p{font-size:11px;color:var(--ff-muted);}
.ad-reward-tag{margin-left:auto;background:rgba(255,215,0,0.15);border:1px solid var(--ff-gold);border-radius:8px;padding:5px 12px;font-size:14px;font-weight:700;color:var(--ff-gold);white-space:nowrap;}
.watch-btn{width:100%;background:linear-gradient(135deg,var(--ff-orange),var(--ff-orange2));border:none;border-radius:12px;padding:16px;font-size:15px;font-weight:700;color:#fff;cursor:pointer;display:flex;align-items:center;justify-content:center;gap:8px;transition:transform 0.1s;}
.watch-btn:active{transform:scale(0.97);}
.watch-btn:disabled{opacity:0.5;cursor:not-allowed;}

/* SPIN */
.spin-header{text-align:center;padding:16px 0 8px;}
.spin-header h2{font-size:20px;font-weight:700;color:var(--ff-blue);}
.spin-remaining{font-size:13px;color:var(--ff-orange);margin-top:4px;}
.wheel-wrap{display:flex;align-items:center;justify-content:center;padding:10px 0 16px;position:relative;}
#spinCanvas{border-radius:50%;border:4px solid rgba(0,207,255,0.4);box-shadow:0 0 30px rgba(0,207,255,0.2);}
.wheel-pointer{position:absolute;top:4px;left:50%;transform:translateX(-50%);z-index:10;font-size:30px;line-height:1;filter:drop-shadow(0 2px 6px rgba(0,0,0,0.6));}
.spin-btn-wrap{padding:0 16px 8px;}
.spin-btn{width:100%;background:linear-gradient(135deg,var(--ff-orange),var(--ff-orange2));border:none;border-radius:14px;padding:16px;font-size:17px;font-weight:800;color:#fff;cursor:pointer;letter-spacing:1px;transition:transform 0.1s;}
.spin-btn:active{transform:scale(0.97);}
.spin-btn:disabled{opacity:0.5;cursor:not-allowed;}
.spin-watch-btn{background:transparent;border:1px solid rgba(0,207,255,0.4);border-radius:12px;padding:13px;font-size:14px;font-weight:600;color:var(--ff-blue);cursor:pointer;display:flex;align-items:center;justify-content:center;gap:6px;margin:8px 16px 0;width:calc(100% - 32px);}
.spin-watch-btn:active{background:rgba(0,207,255,0.1);}
.win-overlay{position:absolute;inset:0;display:flex;align-items:center;justify-content:center;z-index:20;pointer-events:none;}
.win-toast{transform:scale(0);background:linear-gradient(135deg,#1a3a1a,#0d2a0d);border:2px solid var(--ff-green);border-radius:18px;padding:22px 40px;text-align:center;transition:transform 0.3s;}
.win-toast.show{transform:scale(1);}
.win-toast h3{font-size:26px;font-weight:800;color:var(--ff-green);}
.win-toast p{font-size:14px;color:var(--ff-muted);margin-top:4px;}

/* STATS */
.stat-cards{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px;}
.stat-card{background:var(--ff-card);border:1px solid rgba(0,207,255,0.15);border-radius:12px;padding:16px;text-align:center;}
.stat-card .val{font-size:24px;font-weight:800;color:var(--ff-gold);}
.stat-card .lbl{font-size:10px;color:var(--ff-muted);margin-top:3px;text-transform:uppercase;letter-spacing:0.5px;}
.timer-card{background:linear-gradient(135deg,#1a1a3a,#0d0d2a);border:1px solid rgba(155,89,255,0.3);border-radius:14px;padding:18px;text-align:center;margin-bottom:16px;}
.timer-card h3{font-size:13px;color:var(--ff-muted);margin-bottom:8px;text-transform:uppercase;letter-spacing:1px;}
.timer-display{font-size:36px;font-weight:800;color:var(--ff-purple);letter-spacing:3px;font-family:monospace;}
.history-title{font-size:13px;font-weight:600;color:var(--ff-muted);margin-bottom:8px;text-transform:uppercase;letter-spacing:1px;}
.history-item{background:var(--ff-card);border-radius:10px;padding:11px 14px;margin-bottom:6px;display:flex;justify-content:space-between;align-items:center;font-size:12px;}
.history-item .time{color:var(--ff-muted);}
.history-item .reward{color:var(--ff-gold);font-weight:700;}

/* SHOP */
.tab-row{display:flex;background:var(--ff-card);border-radius:12px;padding:4px;margin-bottom:16px;gap:4px;}
.tab-btn{flex:1;padding:9px;border:none;background:none;color:var(--ff-muted);font-size:12px;font-weight:600;border-radius:8px;cursor:pointer;transition:all 0.2s;}
.tab-btn.active{background:linear-gradient(135deg,var(--ff-orange),var(--ff-orange2));color:#fff;}
.shop-tab{display:none;}
.shop-tab.active{display:block;}
.diamond-pkg{background:var(--ff-card);border:1px solid rgba(255,215,0,0.2);border-radius:14px;padding:14px 16px;margin-bottom:10px;display:flex;align-items:center;gap:12px;}
.diamond-pkg.featured{border-color:var(--ff-gold);background:linear-gradient(135deg,#1a1400,#1a0d00);}
.pkg-icon{font-size:30px;width:50px;text-align:center;}
.pkg-info{flex:1;}
.pkg-info h3{font-size:14px;font-weight:700;}
.pkg-info p{font-size:11px;color:var(--ff-muted);margin-top:2px;}
.pkg-price{font-size:16px;font-weight:800;color:var(--ff-gold);margin-right:6px;}
.buy-btn{background:linear-gradient(135deg,var(--ff-orange),var(--ff-orange2));border:none;border-radius:8px;padding:9px 14px;font-size:12px;font-weight:700;color:#fff;cursor:pointer;white-space:nowrap;}
.id-input{background:var(--ff-card2);border:1px solid rgba(0,207,255,0.3);border-radius:10px;padding:11px 14px;color:var(--ff-text);font-size:13px;outline:none;width:100%;}
.id-input::placeholder{color:var(--ff-muted);}
.id-row{display:flex;gap:8px;margin-bottom:14px;}
.id-row .id-input{flex:1;}
.progress-wrap{margin:14px 0;}
.progress-bar-bg{background:var(--ff-card2);border-radius:20px;height:10px;overflow:hidden;margin:8px 0;}
.progress-bar{height:100%;border-radius:20px;background:linear-gradient(90deg,var(--ff-purple),var(--ff-blue));transition:width 0.3s ease;}
.timer-sm{font-size:13px;color:var(--ff-purple);font-family:monospace;text-align:center;margin-top:6px;}

/* PROFILE */
.profile-hero{background:linear-gradient(135deg,#1a2a4a,#0d1a33);border-radius:16px;padding:22px;text-align:center;margin-bottom:16px;border:1px solid rgba(0,207,255,0.1);}
.avatar{width:80px;height:80px;border-radius:50%;background:linear-gradient(135deg,var(--ff-orange),var(--ff-orange2));display:flex;align-items:center;justify-content:center;font-size:38px;margin:0 auto 12px;border:3px solid rgba(255,255,255,0.15);}
.profile-name{font-size:20px;font-weight:700;}
.profile-id{font-size:12px;color:var(--ff-muted);margin-top:4px;}
.profile-code{font-size:16px;font-weight:800;color:var(--ff-blue);background:rgba(0,207,255,0.1);border:1px solid rgba(0,207,255,0.3);border-radius:10px;padding:6px 16px;display:inline-block;margin-top:8px;letter-spacing:3px;font-family:monospace;}
.profile-stats{display:grid;grid-template-columns:1fr 1fr 1fr;gap:8px;margin-top:16px;}
.ps{background:rgba(0,0,0,0.3);border-radius:10px;padding:12px 6px;text-align:center;}
.ps .v{font-size:20px;font-weight:800;color:var(--ff-gold);}
.ps .l{font-size:9px;color:var(--ff-muted);text-transform:uppercase;letter-spacing:0.5px;margin-top:2px;}
.spent-card{background:var(--ff-card);border:1px solid rgba(255,215,0,0.2);border-radius:14px;padding:16px;margin-bottom:14px;}
.spent-card h3{font-size:12px;font-weight:600;color:var(--ff-muted);margin-bottom:12px;text-transform:uppercase;letter-spacing:1px;}
.spent-row{display:flex;justify-content:space-between;align-items:center;padding:9px 0;border-bottom:1px solid rgba(255,255,255,0.05);font-size:13px;}
.spent-row:last-child{border-bottom:none;}
.spent-row .amount{font-weight:700;color:var(--ff-gold);}

/* FLASH */
#flash{position:fixed;top:20px;left:50%;transform:translateX(-50%) translateY(-100px);background:linear-gradient(135deg,#1a3a1a,#0d2a0d);border:1px solid #00ff88;border-radius:14px;padding:12px 24px;color:#00ff88;font-size:14px;font-weight:700;z-index:9999;transition:transform 0.3s ease;pointer-events:none;white-space:nowrap;}
</style>
</head>
<body>
<div id="app">

<!-- FLASH -->
<div id="flash"></div>

<!-- LOGIN PAGE -->
<div id="loginPage">
  <div class="login-diamonds"><span>💎</span><span>💎</span><span>💎</span></div>
  <div class="login-title">FF DIAMOND</div>
  <div class="login-sub">Free Fire Daily Diamond Tips</div>

  <svg width="200" height="130" viewBox="0 0 200 130" style="margin-bottom:20px;">
    <rect width="200" height="130" rx="18" fill="#1a2340"/>
    <circle cx="100" cy="54" r="32" fill="#3a7bd5" opacity="0.85"/>
    <text x="100" y="64" text-anchor="middle" font-size="32" fill="white">🔥</text>
    <rect x="24" y="96" width="152" height="20" rx="5" fill="rgba(255,255,255,0.06)"/>
    <rect x="24" y="96" width="100" height="20" rx="5" fill="rgba(66,133,244,0.45)"/>
    <text x="100" y="110" text-anchor="middle" font-size="10" fill="rgba(255,255,255,0.55)">Signing in...</text>
  </svg>

  <button class="google-btn" onclick="doGoogleLogin()" id="googleBtn">
    <svg class="google-icon" viewBox="0 0 48 48">
      <path fill="#FFC107" d="M43.611,20.083H42V20H24v8h11.303c-1.649,4.657-6.08,8-11.303,8c-6.627,0-12-5.373-12-12c0-6.627,5.373-12,12-12c3.059,0,5.842,1.154,7.961,3.039l5.657-5.657C34.046,6.053,29.268,4,24,4C12.955,4,4,12.955,4,24c0,11.045,8.955,20,20,20c11.045,0,20-8.955,20-20C44,22.659,43.862,21.35,43.611,20.083z"/>
      <path fill="#FF3D00" d="M6.306,14.691l6.571,4.819C14.655,15.108,18.961,12,24,12c3.059,0,5.842,1.154,7.961,3.039l5.657-5.657C34.046,6.053,29.268,4,24,4C16.318,4,9.656,8.337,6.306,14.691z"/>
      <path fill="#4CAF50" d="M24,44c5.166,0,9.86-1.977,13.409-5.192l-6.19-5.238C29.211,35.091,26.715,36,24,36c-5.202,0-9.619-3.317-11.283-7.946l-6.522,5.025C9.505,39.556,16.227,44,24,44z"/>
      <path fill="#1976D2" d="M43.611,20.083H42V20H24v8h11.303c-0.792,2.237-2.231,4.166-4.087,5.571c0.001-0.001,0.002-0.001,0.003-0.002l6.19,5.238C36.971,39.205,44,34,44,24C44,22.659,43.862,21.35,43.611,20.083z"/>
    </svg>
    <div>
      <div class="google-btn-text">Continue with Google</div>
      <div class="google-btn-sub">Google арқылы кіру</div>
    </div>
  </button>
  <div class="login-note">This screen only appears on first launch.<br>Your progress is saved automatically.</div>
</div>

<!-- MAIN APP -->
<div id="mainApp" style="display:none;">

  <!-- PAGE 1: ADS -->
  <div class="page active" id="p1">
    <div class="topbar">
      <span class="topbar-title">💎 FF Diamond</span>
      <div class="diamond-badge">💎 <span id="d1bal">0</span></div>
    </div>
    <div class="content">
      <div class="ad-hero">
        <h2>Watch Ads — Earn Coins!</h2>
        <p>Each ad gives you a reward</p>
        <div class="ad-reward">+10 Coin / ad</div>
        <p style="font-size:12px;color:var(--ff-orange);">Today: <span id="adsWatched">0</span> ads &nbsp;|&nbsp; <span id="totalEarned">0 Coin</span> earned</p>
      </div>
      <div class="ad-box">
        <div class="ad-box-icon">📺</div>
        <div class="ad-box-info"><h3>Video Ad</h3><p>Watch 30 seconds, earn 10 Coin</p></div>
        <div class="ad-reward-tag">+10</div>
      </div>
      <div class="ad-box">
        <div class="ad-box-icon">🎮</div>
        <div class="ad-box-info"><h3>Game Ad</h3><p>Available every day</p></div>
        <div class="ad-reward-tag">+10</div>
      </div>
      <div class="ad-box">
        <div class="ad-box-icon">⭐</div>
        <div class="ad-box-info"><h3>Bonus Ad</h3><p>Extra spins for wheel</p></div>
        <div class="ad-reward-tag">+10</div>
      </div>
      <button class="watch-btn" id="watchAdBtn" onclick="watchAd()">
        ▶ WATCH AD — EARN 10 COIN
      </button>
    </div>
    <div class="nav" id="nav1"></div>
  </div>

  <!-- PAGE 2: SPIN -->
  <div class="page" id="p2">
    <div class="topbar">
      <span class="topbar-title">🎰 Spin &amp; Win</span>
      <div class="diamond-badge">💎 <span id="d2bal">0</span></div>
    </div>
    <div class="content">
      <div class="spin-header">
        <h2>SPIN &amp; WIN</h2>
        <div class="spin-remaining">🎯 <span id="spinCount">0</span> spins remaining</div>
      </div>
      <div class="wheel-wrap">
        <div class="wheel-pointer">▼</div>
        <canvas id="spinCanvas" width="300" height="300"></canvas>
        <div class="win-overlay">
          <div class="win-toast" id="winToast">
            <h3 id="winAmount">+20 Coin</h3>
            <p>Congratulations! 🎉</p>
          </div>
        </div>
      </div>
      <div class="spin-btn-wrap">
        <button class="spin-btn" id="spinBtn" onclick="doSpin()">SPIN THE WHEEL!</button>
      </div>
      <button class="spin-watch-btn" id="spinWatchBtn" onclick="watchAdForSpin()">
        ▶ Watch ad — get 1 free spin
      </button>
    </div>
    <div class="nav" id="nav2"></div>
  </div>

  <!-- PAGE 3: STATS -->
  <div class="page" id="p3">
    <div class="topbar">
      <span class="topbar-title">📊 Statistics</span>
      <div class="diamond-badge">💎 <span id="d3bal">0</span></div>
    </div>
    <div class="content">
      <div class="stat-cards">
        <div class="stat-card"><div class="val" id="s_ads">0</div><div class="lbl">Ads watched</div></div>
        <div class="stat-card"><div class="val" id="s_earned">0 Coin</div><div class="lbl">Total earned</div></div>
        <div class="stat-card"><div class="val" id="s_spins">0</div><div class="lbl">Spins used</div></div>
        <div class="stat-card"><div class="val" id="s_diamonds">0</div><div class="lbl">💎 Diamonds</div></div>
      </div>
      <div class="timer-card">
        <h3>⏱ NEXT REFRESH IN</h3>
        <div class="timer-display" id="mainTimer">24:00:00</div>
      </div>
      <div class="history-title">Recent Activity</div>
      <div id="historyList"><div style="text-align:center;color:var(--ff-muted);font-size:13px;padding:24px;">No activity yet</div></div>
    </div>
    <div class="nav" id="nav3"></div>
  </div>

  <!-- PAGE 4: SHOP -->
  <div class="page" id="p4">
    <div class="topbar">
      <span class="topbar-title">🛒 Shop</span>
      <div class="diamond-badge">💎 <span id="d4bal">0</span></div>
    </div>
    <div class="content">
      <div class="shop-tab active" id="tab-diamonds">
        <div class="id-row">
          <input class="id-input" id="gameId" placeholder="🎮 Enter your Game ID..." />
        </div>
        <div class="progress-wrap">
          <div style="display:flex;justify-content:space-between;font-size:11px;color:var(--ff-muted);">
            <span>Progress</span><span id="progressPct">0%</span>
          </div>
          <div class="progress-bar-bg"><div class="progress-bar" id="progressBar" style="width:0%"></div></div>
          <div class="timer-sm" id="shopTimer">⏱ 24:00:00</div>
        </div>
        <div class="diamond-pkg">
          <div class="pkg-icon">💎</div>
          <div class="pkg-info"><h3>100 Diamonds</h3><p>Starter pack</p></div>
          <span class="pkg-price">600 Coin</span>
          <button class="buy-btn" onclick="buyPackage(100,600)">Buy</button>
        </div>
        <div class="diamond-pkg featured">
          <div class="pkg-icon">💎💎</div>
          <div class="pkg-info"><h3>200 Diamonds</h3><p>⭐ Most popular</p></div>
          <span class="pkg-price">1200 Coin</span>
          <button class="buy-btn" onclick="buyPackage(200,1200)">Buy</button>
        </div>
        <div class="diamond-pkg">
          <div class="pkg-icon">💎💎💎</div>
          <div class="pkg-info"><h3>500 Diamonds</h3><p>Premium pack</p></div>
          <span class="pkg-price">3000 Coin</span>
          <button class="buy-btn" onclick="buyPackage(500,3000)">Buy</button>
        </div>
      </div>

    </div>
    <div class="nav" id="nav4"></div>
  </div>

  <!-- PAGE 5: PROFILE -->
  <div class="page" id="p5">
    <div class="topbar">
      <span class="topbar-title">👤 Profile</span>
      <div class="diamond-badge">💎 <span id="d5bal">0</span></div>
    </div>
    <div class="content">
      <div class="profile-hero">
        <div class="avatar">🔥</div>
        <div class="profile-name" id="pName">Player</div>
        <div class="profile-id">Game ID: <span id="pId">—</span></div>
        <div class="profile-code" id="pCode">—</div>
        <div class="profile-stats">
          <div class="ps"><div class="v" id="pAds">0</div><div class="l">Ads</div></div>
          <div class="ps"><div class="v" id="pDollars">0 Coin</div><div class="l">Earned</div></div>
          <div class="ps"><div class="v" id="pDiamonds">0</div><div class="l">💎</div></div>
        </div>
      </div>
      <div class="spent-card">
        <h3>💰 Purchase History</h3>
        <div id="spentHistory"><div style="text-align:center;color:var(--ff-muted);font-size:12px;padding:12px;">No history</div></div>
      </div>
      <div class="id-row">
        <input class="id-input" id="profileIdInput" placeholder="Save Game ID..." />
        <button class="buy-btn" onclick="saveProfileId()">Save</button>
      </div>
    </div>
    <div class="nav" id="nav5"></div>
  </div>

</div><!-- /mainApp -->
</div><!-- /app -->

<script>
var STORAGE_KEY='ff_diamond_v2';

/* ============================================= */
/* ADSTERRA SMARTLINK — батырма басқанда ашылады  */
/* ============================================= */
var ADSTERRA_SMARTLINK='https://www.effectivecpmnetwork.com/hsefgs7ghq?key=3599484f35ede989aec9a3a494d6a72c';
function openSmartlink(){
  window.open(ADSTERRA_SMARTLINK,'_blank');
}
/* ============================================= */

function genCode(){
  var c='ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789',r='';
  for(var i=0;i<8;i++) r+=c[Math.floor(Math.random()*c.length)];
  return r.slice(0,4)+'-'+r.slice(4);
}

function loadState(){
  try{var r=localStorage.getItem(STORAGE_KEY);if(r)return JSON.parse(r);}catch(e){}
  return null;
}
function saveState(){
  try{localStorage.setItem(STORAGE_KEY,JSON.stringify(state));}catch(e){}
}

var saved=loadState();
var state=saved||{
  balance:0,adsWatched:0,totalEarned:0,spins:0,
  diamonds:0,gameId:'',purchases:[],history:[],
  timer:86400,shopProgress:0,loggedIn:false,userCode:genCode()
};
if(!state.userCode) state.userCode=genCode();

var NAV=[
  {icon:'📢',label:'Ads'},{icon:'🎰',label:'Spin'},
  {icon:'📊',label:'Stats'},{icon:'🛒',label:'Shop'},{icon:'👤',label:'Profile'}
];

function buildNavs(){
  for(var n=1;n<=5;n++){
    var el=document.getElementById('nav'+n);
    el.innerHTML=NAV.map(function(item,i){
      return '<button class="nav-btn'+(i===(n-1)?' active':'')+'" onclick="gotoPage('+(i+1)+')">'
        +'<span style="display:block;font-size:20px;margin-bottom:2px;">'+item.icon+'</span>'
        +item.label+'</button>';
    }).join('');
  }
}

function gotoPage(n){
  document.querySelectorAll('.page').forEach(function(p){p.classList.remove('active');});
  document.getElementById('p'+n).classList.add('active');
  updateAll();
}

function doGoogleLogin(){
  var btn=document.getElementById('googleBtn');
  btn.style.opacity='0.6';btn.style.pointerEvents='none';
  btn.querySelector('.google-btn-text').textContent='Signing in...';
  setTimeout(function(){
    state.loggedIn=true;saveState();
    document.getElementById('loginPage').classList.add('hidden');
    document.getElementById('mainApp').style.display='block';
    buildNavs();drawWheel();updateAll();startTimer();
  },1800);
}

if(state.loggedIn){
  document.getElementById('loginPage').classList.add('hidden');
  document.getElementById('mainApp').style.display='block';
  buildNavs();
}

function updateAll(){
  var b=state.balance.toFixed(0);
  for(var n=1;n<=5;n++){var e=document.getElementById('d'+n+'bal');if(e)e.textContent=b;}
  setText('adsWatched',state.adsWatched);
  setText('totalEarned',state.totalEarned+' Coin');
  setText('spinCount',state.spins);
  setText('s_ads',state.adsWatched);setText('s_earned',state.totalEarned+' Coin');
  setText('s_spins',state.spins);setText('s_diamonds',state.diamonds);
  setText('pAds',state.adsWatched);setText('pDollars',state.totalEarned+' Coin');
  setText('pDiamonds',state.diamonds);
  setText('pId',state.gameId||'—');
  setText('pCode',state.userCode);
  if(state.gameId) setText('pName','Player #'+state.gameId.slice(0,6));
  var pb=document.getElementById('progressBar');if(pb)pb.style.width=state.shopProgress+'%';
  var pp=document.getElementById('progressPct');if(pp)pp.textContent=state.shopProgress+'%';
  updateHistory();updateSpentHistory();saveState();
}

function setText(id,val){var e=document.getElementById(id);if(e)e.textContent=val;}

function watchAd(){
  var btn=document.getElementById('watchAdBtn');
  if(btn.disabled)return;
  btn.disabled=true;btn.textContent='⏳ Loading ad...';
  openSmartlink(); /* ADSTERRA SMARTLINK ашылады */
  setTimeout(function(){
    state.adsWatched++;state.totalEarned+=10;state.balance+=10;
    addHistory('📺 Watched ad','+ 10 Coin');
    btn.disabled=false;btn.textContent='▶ WATCH AD — EARN 10 COIN';
    updateAll();flash('+10 Coin earned! 🎉');
  },2000);
}

function watchAdForSpin(){
  var btn=document.getElementById('spinWatchBtn');
  if(btn.disabled)return;
  btn.disabled=true;
  openSmartlink(); /* ADSTERRA SMARTLINK ашылады */
  setTimeout(function(){
    state.adsWatched++;state.totalEarned+=10;state.balance+=10;state.spins++;
    addHistory('📺 Ad → Got spin','+ 10 Coin + 1 spin');
    btn.disabled=false;updateAll();flash('+1 Spin earned!');
  },2000);
}

/* WHEEL */
var PRIZES=[1,5,10,15,20,5,10,15];
var COLORS=['#e74c3c','#3498db','#2ecc71','#f39c12','#9b59b6','#e67e22','#1abc9c','#c0392b'];
var spinning=false,currentAngle=0;

function drawWheel(){
  var c=document.getElementById('spinCanvas');if(!c)return;
  var ctx=c.getContext('2d'),cx=150,cy=150,r=138,seg=PRIZES.length;
  ctx.clearRect(0,0,300,300);
  for(var i=0;i<seg;i++){
    var s=currentAngle+i*(2*Math.PI/seg),e=s+(2*Math.PI/seg);
    ctx.beginPath();ctx.moveTo(cx,cy);ctx.arc(cx,cy,r,s,e);ctx.closePath();
    ctx.fillStyle=COLORS[i];ctx.fill();
    ctx.strokeStyle='rgba(255,255,255,0.25)';ctx.lineWidth=2;ctx.stroke();
    ctx.save();ctx.translate(cx,cy);ctx.rotate(s+(e-s)/2);
    ctx.fillStyle='#fff';ctx.font='bold 15px Segoe UI';
    ctx.textAlign='center';ctx.textBaseline='middle';
    ctx.fillText(PRIZES[i],r*0.64,0);ctx.restore();
  }
  ctx.beginPath();ctx.arc(cx,cy,24,0,2*Math.PI);
  ctx.fillStyle='#1a2340';ctx.fill();
  ctx.strokeStyle='rgba(0,207,255,0.7)';ctx.lineWidth=3;ctx.stroke();
  ctx.fillStyle='#00cfff';ctx.font='bold 11px Segoe UI';
  ctx.textAlign='center';ctx.textBaseline='middle';ctx.fillText('FF',cx,cy);
}

function doSpin(){
  if(spinning)return;
  if(state.spins<=0){flash('No spins! Watch an ad first.');return;}
  spinning=true;state.spins--;
  document.getElementById('spinBtn').disabled=true;
  var tot=8*2*Math.PI+Math.random()*2*Math.PI,start=null,dur=4200,init=currentAngle;
  function anim(ts){
    if(!start)start=ts;
    var el=ts-start,prog=Math.min(el/dur,1),ease=1-Math.pow(1-prog,4);
    currentAngle=init+tot*ease;drawWheel();
    if(prog<1){requestAnimationFrame(anim);}
    else{
      var norm=((currentAngle%(2*Math.PI))+2*Math.PI)%(2*Math.PI);
      var sa=2*Math.PI/PRIZES.length;
      var idx=Math.floor(((2*Math.PI-norm+sa/2)%(2*Math.PI))/sa)%PRIZES.length;
      var prize=PRIZES[idx];
      state.balance+=prize;state.totalEarned+=prize;
      addHistory('🎰 Spin won','+ '+prize+' Coin');
      setText('winAmount','+'+prize+' Coin');
      var toast=document.getElementById('winToast');
      toast.classList.add('show');
      setTimeout(function(){toast.classList.remove('show');spinning=false;document.getElementById('spinBtn').disabled=false;updateAll();},2200);
    }
  }
  requestAnimationFrame(anim);
}

function addHistory(label,val){
  var now=new Date(),time=now.getHours()+':'+String(now.getMinutes()).padStart(2,'0');
  state.history.unshift({label:label,val:val,time:time});
  if(state.history.length>20)state.history.pop();
}

function updateHistory(){
  var el=document.getElementById('historyList');if(!el)return;
  if(!state.history.length){
    el.innerHTML='<div style="text-align:center;color:var(--ff-muted);font-size:13px;padding:24px;">No activity yet</div>';return;
  }
  el.innerHTML=state.history.slice(0,10).map(function(h){
    return '<div class="history-item"><span>'+h.label+'</span><span class="reward">'+h.val+'</span><span class="time">'+h.time+'</span></div>';
  }).join('');
}

function updateSpentHistory(){
  var el=document.getElementById('spentHistory');if(!el)return;
  if(!state.purchases.length){
    el.innerHTML='<div style="text-align:center;color:var(--ff-muted);font-size:12px;padding:12px;">No history</div>';return;
  }
  el.innerHTML=state.purchases.map(function(p){
    return '<div class="spent-row"><span>'+p.label+'</span><span class="amount">'+p.cost+'</span></div>';
  }).join('');
}

function buyPackage(diamonds,cost){
  var id=document.getElementById('gameId').value.trim();
  if(!id){flash('Enter Game ID first!');return;}
  if(state.balance<cost){flash('Need '+cost+' Coin! Watch more ads.');return;}
  state.balance-=cost;state.diamonds+=diamonds;state.gameId=id;
  state.purchases.unshift({label:'💎 '+diamonds+' diamonds (ID:'+id+')',cost:'-'+cost+' Coin'});
  addHistory('💎 Bought '+diamonds+' diamonds','-'+cost+' Coin');
  state.shopProgress=Math.min(100,state.shopProgress+30);
  updateAll();flash(diamonds+' Diamonds added! 💎');
}

function animProg(bid,pid,target,ms){
  var bar=document.getElementById(bid),pct=document.getElementById(pid),cur=0,step=target/(ms/50);
  var iv=setInterval(function(){
    cur=Math.min(cur+step,target);
    bar.style.width=Math.round(cur)+'%';
    pct.textContent=Math.round(cur)+'%';
    if(cur>=target)clearInterval(iv);
  },50);
}

function saveProfileId(){
  var id=document.getElementById('profileIdInput').value.trim();
  if(!id){flash('Enter a Game ID!');return;}
  state.gameId=id;updateAll();flash('ID saved!');
}

/* TIMER */
function fmt(s){
  var h=Math.floor(s/3600),m=Math.floor((s%3600)/60),sec=s%60;
  return String(h).padStart(2,'0')+':'+String(m).padStart(2,'0')+':'+String(sec).padStart(2,'0');
}
function startTimer(){
  setInterval(function(){
    if(state.timer>0)state.timer--;else state.timer=86400;
    var t=fmt(state.timer);
    setText('mainTimer',t);
    setText('shopTimer','⏱ '+t);
    saveState();
  },1000);
}

/* FLASH */
var flashEl=document.getElementById('flash'),flashTm;
function flash(msg){
  clearTimeout(flashTm);
  flashEl.textContent=msg;
  flashEl.style.transform='translateX(-50%) translateY(0)';
  flashTm=setTimeout(function(){flashEl.style.transform='translateX(-50%) translateY(-100px)';},2400);
}

/* INIT */
if(state.loggedIn){
  drawWheel();updateAll();startTimer();
}
</script>
</body>
</html>

<!DOCTYPE html>
<html lang="zh-TW">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>貓窩裏｜到府寵物保姆預約</title>
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@300;400;500;700;900&display=swap" rel="stylesheet">
<!-- EmailJS SDK -->
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:'Noto Sans TC','Microsoft JhengHei',sans-serif;background:linear-gradient(160deg,#e8f5fd 0%,#fce8f0 45%,#fef6e4 100%);min-height:100vh;color:#3a2c2c}
.header{background:rgba(255,255,255,0.92);backdrop-filter:blur(12px);border-bottom:3px solid #c8e6f5;padding:14px 24px;display:flex;align-items:center;justify-content:space-between;position:sticky;top:0;z-index:50;box-shadow:0 2px 12px rgba(168,216,234,0.2)}
.logo{display:flex;align-items:center;gap:10px}
.logo-icon{font-size:1.6rem}
.logo-name{font-size:1.15rem;font-weight:900;color:#6baed6;line-height:1}
.logo-sub{font-size:0.68rem;color:#f4a0a0;letter-spacing:0.12em;font-weight:600}
.header-badge{background:linear-gradient(135deg,#a8d8ea,#f9c5c5);padding:5px 14px;border-radius:20px;font-size:0.72rem;color:white;font-weight:700}
.hero{position:relative;overflow:hidden;padding:44px 24px 38px;text-align:center}
.blob{position:absolute;border-radius:50%;pointer-events:none}
.blob1{top:-40px;left:-40px;width:200px;height:200px;background:radial-gradient(circle,#c8e6f588,transparent 70%)}
.blob2{top:0;right:-30px;width:160px;height:160px;background:radial-gradient(circle,#f9c5c588,transparent 70%)}
.blob3{bottom:-20px;left:35%;width:130px;height:130px;background:radial-gradient(circle,#fddcb588,transparent 70%)}
.paw-deco{position:absolute;opacity:0.13;pointer-events:none}
.hero-inner{position:relative;z-index:1}
.hero-emoji{font-size:3rem;margin-bottom:12px;display:block}
.hero h1{font-size:1.8rem;font-weight:900;line-height:1.35;margin-bottom:8px;background:linear-gradient(135deg,#6baed6,#f4a0a0);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.hero p{color:#6b4f4f;font-size:0.88rem;letter-spacing:0.06em}
.nav-tabs{display:flex;gap:0;background:rgba(255,255,255,0.85);border-radius:16px;padding:4px;margin:0 16px 4px;max-width:760px;margin-left:auto;margin-right:auto;box-shadow:0 2px 12px rgba(168,216,234,0.2);border:1.5px solid #c8e6f5}
.nav-tab{flex:1;padding:10px 4px;border:none;background:transparent;font-family:inherit;font-size:0.78rem;font-weight:700;color:#9c7c7c;cursor:pointer;border-radius:12px;transition:all .2s}
.nav-tab.active{background:linear-gradient(135deg,#a8d8ea,#f9c5c5);color:white;box-shadow:0 2px 8px rgba(168,216,234,0.4)}
.section{display:none;max-width:760px;margin:0 auto;padding:16px 16px 80px}
.section.active{display:block}
.sec-title{display:flex;align-items:center;gap:8px;margin:22px 0 10px;font-size:0.92rem;font-weight:700;color:#6b4f4f}
.sec-line{flex:1;height:1.5px;background:linear-gradient(to right,#c8e6f5,transparent);border-radius:2px}
.card{background:rgba(255,255,255,0.92);border-radius:20px;padding:20px;margin-bottom:16px;box-shadow:0 4px 20px rgba(168,216,234,0.18);border:1.5px solid rgba(168,216,234,0.25)}
.row2{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:12px}
.fgroup{margin-bottom:12px}
.fgroup:last-child{margin-bottom:0}
label.fl{display:block;font-size:0.8rem;font-weight:600;color:#6b4f4f;margin-bottom:5px}
input[type=text],input[type=tel],input[type=date],input[type=number],textarea,select{width:100%;padding:11px 15px;border:2px solid #c8e6f5;border-radius:14px;font-size:0.88rem;color:#3a2c2c;background:white;outline:none;font-family:inherit;transition:border-color .2s;-webkit-appearance:none;appearance:none}
input:focus,textarea:focus,select:focus{border-color:#6baed6;box-shadow:0 0 0 3px rgba(107,174,214,0.12)}
textarea{resize:vertical;min-height:80px}
.err-msg{font-size:0.74rem;color:#f4a0a0;margin-top:3px;display:none}
.err-input{border-color:#f4a0a0!important}

/* TRAVEL */
.km-row{display:flex;gap:10px;align-items:flex-end}
.km-input-wrap{flex:1}
.km-link{display:inline-flex;align-items:center;gap:6px;padding:11px 14px;border:2px solid #a8d8ea;border-radius:14px;background:linear-gradient(135deg,#a8d8ea,#c8e6f5);color:#2c6e9c;font-size:0.82rem;font-weight:700;cursor:pointer;white-space:nowrap;flex-shrink:0;text-decoration:none;transition:all .2s}
.km-link:hover{background:linear-gradient(135deg,#6baed6,#a8d8ea);color:white}
.km-result{margin-top:8px;border-radius:12px;padding:11px 14px;font-size:0.82rem;line-height:1.7}
.km-free{background:linear-gradient(135deg,#e8f8ee,#d4f0dc);border:1.5px solid #7dcf95;color:#2d7a4a}
.km-fee{background:linear-gradient(135deg,#fff3e0,#fde8c8);border:1.5px solid #f4b56a;color:#8a5a1a}

/* COUNT */
.count-wrap{display:flex;align-items:center;border:2px solid #c8e6f5;border-radius:14px;overflow:hidden;width:fit-content;margin-top:6px}
.cnt-btn{width:40px;height:40px;border:none;background:linear-gradient(135deg,#c8e6f5,#a8d8ea);color:#2c6e9c;font-size:1.2rem;cursor:pointer;font-weight:900;font-family:inherit}
.cnt-num{width:50px;text-align:center;font-weight:900;font-size:1rem;color:#2c6e9c;background:white;height:40px;line-height:40px;border-left:2px solid #c8e6f5;border-right:2px solid #c8e6f5}
.extra-note{margin-top:10px;background:linear-gradient(135deg,#fddcb555,#f9c5c544);border:1.5px solid #f4a0a055;border-radius:12px;padding:10px 14px;font-size:0.8rem;color:#6b4f4f}

/* SESSION */
.session-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:8px;margin-top:6px}
.session-btn{padding:10px 4px;border:2px solid #c8e6f5;border-radius:12px;background:white;color:#6b4f4f;font-family:inherit;font-size:0.82rem;cursor:pointer;font-weight:700;transition:all .2s}
.session-btn.active{border-color:#6baed6;background:linear-gradient(135deg,#c8e6f5,#a8d8ea);color:#2c6e9c}

/* SERVICE */
.svc-grid{display:grid;grid-template-columns:1fr 1fr 1fr;gap:10px;margin-bottom:14px}
.svc-card{padding:14px 10px;cursor:pointer;border-radius:16px;text-align:center;border:2.5px solid #c8e6f5;background:white;transition:all .2s}
.svc-card.active{border-color:#6baed6;background:linear-gradient(135deg,#c8e6f566,#a8d8ea44);box-shadow:0 4px 14px rgba(168,216,234,0.45)}
.svc-icon{font-size:1.4rem;margin-bottom:4px}
.svc-name{font-weight:700;font-size:0.82rem;color:#3a2c2c;margin-bottom:3px;line-height:1.3}
.svc-price{font-size:0.74rem;font-weight:700;color:#6baed6}
.svc-note{background:#f0faf6;border:1.5px solid rgba(168,216,234,0.35);border-radius:12px;padding:11px 14px;font-size:0.79rem;color:#6b4f4f;line-height:1.7}

/* ADDON */
.addon-item{display:flex;align-items:center;gap:12px;padding:12px 14px;margin-bottom:8px;border:2px solid #c8e6f5;border-radius:14px;cursor:pointer;background:white;transition:all .2s;user-select:none}
.addon-item:last-child{margin-bottom:0}
.addon-item.checked{border-color:#f4a0a0;background:linear-gradient(135deg,#f9c5c522,#fddcb522)}
.addon-check{width:22px;height:22px;border-radius:7px;flex-shrink:0;border:2px solid #c8e6f5;background:white;display:flex;align-items:center;justify-content:center;color:white;font-size:0.75rem;font-weight:700;transition:all .2s}
.addon-item.checked .addon-check{background:#f4a0a0;border-color:#f4a0a0}
.addon-name{font-size:0.88rem;font-weight:600;color:#3a2c2c}
.addon-price{font-size:0.76rem;font-weight:700;color:#f4a0a0}

/* URGENT */
.urgent-grid{display:grid;grid-template-columns:1fr 1fr 1fr;gap:10px}
.urgent-btn{padding:12px 8px;border:2px solid #c8e6f5;border-radius:14px;background:white;font-family:inherit;cursor:pointer;text-align:center;transition:all .2s}
.urgent-btn.sel-none{border-color:#7dcf95;background:linear-gradient(135deg,#e8f8ee,#d4f0dc)}
.urgent-btn.sel-48{border-color:#f4b56a;background:linear-gradient(135deg,#fff3e0,#fde8c8)}
.urgent-btn.sel-24{border-color:#f4a0a0;background:linear-gradient(135deg,#fff0f0,#fde0e0)}
.urgent-label{font-size:0.82rem;font-weight:700;color:#3a2c2c}
.urgent-sub{font-size:0.7rem;color:#9c7c7c;margin-top:2px}
.urgent-price{font-size:0.78rem;font-weight:700;margin-top:4px}

/* PRICE */
.price-box{background:linear-gradient(135deg,#6baed6,#5a9dbf 55%,#e8829a);border-radius:20px;padding:22px;margin-bottom:18px;box-shadow:0 6px 24px rgba(107,174,214,0.3)}
.price-title{font-size:0.85rem;color:rgba(255,255,255,0.8);margin-bottom:14px;font-weight:600;letter-spacing:0.06em}
.price-line{display:flex;justify-content:space-between;padding:7px 0;border-bottom:1px solid rgba(255,255,255,0.12);font-size:0.85rem;color:rgba(255,255,255,0.92)}
.price-line.indent{padding-left:14px;font-size:0.78rem;color:rgba(255,255,255,0.68)}
.price-total-row{display:flex;justify-content:space-between;align-items:center;padding-top:14px;margin-top:6px;border-top:2px solid rgba(255,255,255,0.3)}
.price-total-label{font-weight:700;color:white;font-size:0.95rem}
.price-total-num{font-size:2rem;font-weight:900;color:#ffe08a}

.disclaimer{background:rgba(249,197,197,0.15);border:1.5px solid rgba(244,160,160,0.25);border-radius:14px;padding:12px 16px;font-size:0.79rem;color:#6b4f4f;line-height:1.8;margin-bottom:20px}
.submit-btn{width:100%;padding:18px;background:linear-gradient(135deg,#f4a0a0,#f08080 50%,#fddcb5);color:white;border:none;border-radius:18px;font-family:inherit;font-size:1.05rem;font-weight:900;cursor:pointer;letter-spacing:0.1em;box-shadow:0 6px 20px rgba(244,160,160,0.45);transition:transform .15s,box-shadow .15s}
.submit-btn:hover{transform:translateY(-2px);box-shadow:0 10px 28px rgba(244,160,160,0.6)}
.submit-btn:disabled{opacity:.6;cursor:not-allowed;transform:none}

/* TEAM */
.team-hero{background:linear-gradient(135deg,#6baed6,#a8d8ea,#f9c5c5);border-radius:20px;padding:24px;margin-bottom:20px;text-align:center;color:white}
.team-hero h2{font-size:1.25rem;font-weight:900;margin-bottom:6px}
.team-hero p{font-size:0.84rem;opacity:.92;line-height:1.6}
.team-card{background:rgba(255,255,255,0.92);border-radius:20px;padding:20px;margin-bottom:14px;border:1.5px solid rgba(168,216,234,0.25);box-shadow:0 4px 16px rgba(168,216,234,0.15)}
.team-header{display:flex;align-items:flex-start;gap:14px;margin-bottom:12px}
.team-avatar{width:68px;height:68px;border-radius:18px;font-size:2.2rem;display:flex;align-items:center;justify-content:center;flex-shrink:0;box-shadow:0 4px 12px rgba(168,216,234,0.3)}
.team-name{font-size:1rem;font-weight:900;color:#3a2c2c;margin-bottom:3px}
.team-role{font-size:0.72rem;font-weight:700;padding:3px 10px;border-radius:20px;display:inline-block;margin-bottom:6px}
.team-bio{font-size:0.82rem;color:#6b4f4f;line-height:1.75}
.cert-list{display:flex;flex-wrap:wrap;gap:6px;margin-top:10px}
.cert-tag{font-size:0.7rem;padding:3px 10px;border-radius:20px;font-weight:600}

/* QUAL */
.qual-card{background:rgba(255,255,255,0.92);border-radius:20px;padding:20px;margin-bottom:14px;border:1.5px solid rgba(168,216,234,0.25);box-shadow:0 4px 16px rgba(168,216,234,0.12)}
.qual-item{display:flex;gap:14px;padding:12px 0;border-bottom:1px dashed #e8d5bc}
.qual-item:last-child{border-bottom:none;padding-bottom:0}
.qual-icon{font-size:1.4rem;flex-shrink:0;width:36px;text-align:center;margin-top:2px}
.qual-content h4{font-size:0.88rem;font-weight:700;color:#3a2c2c;margin-bottom:3px}
.qual-content p{font-size:0.79rem;color:#6b4f4f;line-height:1.65}
.qual-badge{display:inline-block;font-size:0.68rem;padding:2px 8px;border-radius:10px;background:linear-gradient(135deg,#a8d8ea,#c8e6f5);color:#2c6e9c;font-weight:700;margin-top:4px}

/* MODAL */
.overlay{display:none;position:fixed;inset:0;background:rgba(100,150,200,0.4);backdrop-filter:blur(6px);align-items:center;justify-content:center;z-index:200}
.overlay.show{display:flex}
.modal{background:white;border-radius:24px;padding:30px 22px;max-width:360px;width:92%;text-align:center;box-shadow:0 20px 60px rgba(107,174,214,0.35);border:3px solid #c8e6f5;animation:popIn .3s cubic-bezier(.34,1.56,.64,1);max-height:88vh;overflow-y:auto}
@keyframes popIn{from{transform:scale(.8);opacity:0}to{transform:scale(1);opacity:1}}
.modal-emoji{font-size:2.8rem;margin-bottom:10px}
.modal h2{font-size:1.15rem;font-weight:900;color:#6baed6;margin-bottom:10px}
.modal-inner{background:linear-gradient(135deg,rgba(200,230,245,.28),rgba(249,197,197,.22));border-radius:14px;padding:14px;margin-bottom:14px;text-align:left}
.modal-highlight{font-size:0.9rem;font-weight:700;color:#f4a0a0;margin-bottom:8px;text-align:center}
.modal-detail{font-size:0.81rem;color:#6b4f4f;line-height:1.9}
.modal-btn{padding:11px 26px;background:linear-gradient(135deg,#6baed6,#f4a0a0);color:white;border:none;border-radius:14px;font-family:inherit;font-size:0.88rem;font-weight:700;cursor:pointer}

@media(max-width:540px){
  .row2{grid-template-columns:1fr}
  .svc-grid{grid-template-columns:1fr 1fr}
  .urgent-grid{grid-template-columns:1fr}
  .session-grid{grid-template-columns:repeat(2,1fr)}
  .hero h1{font-size:1.5rem}
  .km-row{flex-direction:column}
  .km-link{width:100%;justify-content:center}
}
</style>
</head>
<body>

<div class="header">
  <div class="logo">
    <span class="logo-icon">🐱</span>
    <div>
      <div class="logo-name">貓窩裏</div>
      <div class="logo-sub">到府寵物保姆</div>
    </div>
  </div>
  <div class="header-badge">🏠 到府服務</div>
</div>

<div class="hero">
  <div class="blob blob1"></div><div class="blob blob2"></div><div class="blob blob3"></div>
  <span class="paw-deco" style="top:18px;left:12%;font-size:1.5rem">🐾</span>
  <span class="paw-deco" style="top:40px;right:15%;font-size:1.1rem">🐾</span>
  <span class="paw-deco" style="bottom:8px;left:44%;font-size:0.9rem">🐾</span>
  <div class="hero-inner">
    <span class="hero-emoji">🐱💕</span>
    <h1>讓毛孩在家<br>也有人陪伴 ✨</h1>
    <p>專業保姆到府服務 · 安心出門不擔心</p>
  </div>
</div>

<div class="nav-tabs">
  <button class="nav-tab active" onclick="showTab('booking')">🗓 立即預約</button>
  <button class="nav-tab" onclick="showTab('team')">👩‍⚕️ 保姆團隊</button>
  <button class="nav-tab" onclick="showTab('qual')">🏅 專業資歷</button>
</div>

<!-- ══════════════ 預約 ══════════════ -->
<div class="section active" id="tab-booking">

  <div class="sec-title">📋 基本資料 <div class="sec-line"></div></div>
  <div class="card">
    <div class="row2">
      <div class="fgroup">
        <label class="fl">飼主姓名 *</label>
        <input type="text" id="name" placeholder="請輸入姓名">
        <div class="err-msg" id="err-name">⚠ 請填寫姓名</div>
      </div>
      <div class="fgroup">
        <label class="fl">聯絡電話 *</label>
        <input type="tel" id="phone" placeholder="09XX-XXX-XXX">
        <div class="err-msg" id="err-phone">⚠ 請填寫電話</div>
      </div>
    </div>
    <div class="fgroup">
      <label class="fl">服務地址 *</label>
      <input type="text" id="address" placeholder="請輸入完整地址">
      <div class="err-msg" id="err-address">⚠ 請填寫地址</div>
    </div>

    <!-- 車馬費 -->
    <div class="fgroup">
      <label class="fl">車馬費計算　<span style="font-weight:400;color:#9c7c7c;font-size:0.74rem">5公里內免費，超出每公里 +NT$30</span></label>
      <div class="km-row">
        <div class="km-input-wrap">
          <input type="number" id="km-input" min="0" step="0.1" placeholder="請輸入與青雲宮的距離（公里）" oninput="calcKmFee()">
        </div>
        <a class="km-link" href="https://maps.google.com?saddr=高雄市大社區青雲宮" target="_blank">
          🗺 開啟 Google Maps
        </a>
      </div>
      <div style="font-size:0.74rem;color:#9c7c7c;margin-top:5px">👆 點按開啟地圖 → 輸入您的地址 → 查看距離後填入上方</div>
      <div id="km-result" style="display:none" class="km-result"></div>
    </div>
  </div>

  <div class="sec-title">📅 預約日期與次數 <div class="sec-line"></div></div>
  <div class="card">
    <div class="row2">
      <div class="fgroup">
        <label class="fl">開始日期 *</label>
        <input type="date" id="start-date" onchange="updateDays()">
        <div class="err-msg" id="err-start-date">⚠ 請選擇日期</div>
      </div>
      <div class="fgroup">
        <label class="fl">結束日期 *</label>
        <input type="date" id="end-date" onchange="updateDays()">
        <div class="err-msg" id="err-end-date">⚠ 請選擇日期</div>
      </div>
    </div>
    <div class="fgroup">
      <label class="fl">每天服務次數</label>
      <div class="session-grid">
        <button class="session-btn active" onclick="setSession(this,1)">1次</button>
        <button class="session-btn" onclick="setSession(this,2)">2次</button>
        <button class="session-btn" onclick="setSession(this,3)">3次</button>
        <button class="session-btn" onclick="setSession(this,4)">4次</button>
      </div>
    </div>
    <div id="days-badge" style="display:none;margin-top:4px;background:linear-gradient(135deg,#e8f5fd,#fce8f0);border:1.5px solid #c8e6f5;border-radius:12px;padding:10px 14px;font-size:0.82rem;color:#2c6e9c;font-weight:600"></div>
  </div>

  <div class="sec-title">⚡ 急件加收 <div class="sec-line"></div></div>
  <div class="card">
    <div class="urgent-grid">
      <button class="urgent-btn sel-none" onclick="setUrgent(this,'none',0)">
        <div class="urgent-label">一般預約</div>
        <div class="urgent-sub">48小時前下單</div>
        <div class="urgent-price" style="color:#7dcf95">免加收</div>
      </button>
      <button class="urgent-btn" onclick="setUrgent(this,'48',100)">
        <div class="urgent-label">⚡ 急件</div>
        <div class="urgent-sub">48小時內下單</div>
        <div class="urgent-price" style="color:#f4b56a">+NT$100</div>
      </button>
      <button class="urgent-btn" onclick="setUrgent(this,'24',200)">
        <div class="urgent-label">🔥 緊急</div>
        <div class="urgent-sub">24小時內下單</div>
        <div class="urgent-price" style="color:#f4a0a0">+NT$200</div>
      </button>
    </div>
  </div>

  <div class="sec-title">🐾 寵物資訊 <div class="sec-line"></div></div>
  <div class="card">
    <div class="fgroup">
      <label class="fl">寵物名字</label>
      <input type="text" id="petname" placeholder="例：小花、球球、麻糬">
    </div>
    <div class="fgroup">
      <label class="fl">貓咪數量 🐱</label>
      <div class="count-wrap">
        <button class="cnt-btn" onclick="changeCount('cat',-1)">−</button>
        <div class="cnt-num" id="cnt-cat">0</div>
        <button class="cnt-btn" onclick="changeCount('cat',1)">+</button>
      </div>
    </div>
    <div class="fgroup">
      <label class="fl">狗狗數量 🐶</label>
      <div class="count-wrap">
        <button class="cnt-btn" onclick="changeCount('dog',-1)">−</button>
        <div class="cnt-num" id="cnt-dog">0</div>
        <button class="cnt-btn" onclick="changeCount('dog',1)">+</button>
      </div>
    </div>
    <div class="fgroup">
      <label class="fl">其他寵物數量 🐾</label>
      <div class="count-wrap">
        <button class="cnt-btn" onclick="changeCount('other',-1)">−</button>
        <div class="cnt-num" id="cnt-other">0</div>
        <button class="cnt-btn" onclick="changeCount('other',1)">+</button>
      </div>
    </div>
    <div class="extra-note" id="extra-note" style="display:none">🐾 第三隻起加收：<span id="extra-text"></span></div>
  </div>

  <div class="sec-title">✨ 主要服務 <div class="sec-line"></div></div>
  <div class="card">
    <div class="svc-grid">
      <div class="svc-card active" id="svc-companion" onclick="setService('companion')">
        <div class="svc-icon">🏠</div>
        <div class="svc-name">到府陪伴</div>
        <div class="svc-price">NT$300 / 次</div>
      </div>
      <div class="svc-card" id="svc-walk" onclick="setService('walk')">
        <div class="svc-icon">🦮</div>
        <div class="svc-name">散步服務</div>
        <div class="svc-price">NT$200 / 次</div>
      </div>
      <div class="svc-card" id="svc-both" onclick="setService('both')">
        <div class="svc-icon">🏠🦮</div>
        <div class="svc-name">陪伴＋遛狗</div>
        <div class="svc-price">NT$500 / 次</div>
      </div>
    </div>
    <div class="svc-note">
      🏠 到府陪伴：餵食、清潔、陪玩、觀察身體狀況<br>
      🦮 散步服務：陪同外出散步、如廁<br>
      🏠🦮 陪伴＋遛狗：包含以上全部服務
    </div>
  </div>

  <div class="sec-title">➕ 加購服務（每天計費，可複選） <div class="sec-line"></div></div>
  <div class="card">
    <di

<!DOCTYPE html>
<html lang="zh-TW">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>兒童自律公約</title>
<link href="https://fonts.googleapis.com/css2?family=Nunito:wght@700;800;900&family=Noto+Sans+TC:wght@400;500;700;900&display=swap" rel="stylesheet">
<style>
*{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent;}
:root{
  --pink:#E84D8A;
  --pink2:#F472B6;
  --pink-light:#FFB3D4;
  --purple:#9B5DE5;
  --purple2:#C084FC;
  --purple-light:#E9D5FF;
  --bg:#F8F0FF;
  --text:#2D1B69;
  --gray:#B0A0C0;
  --orange:#F59E0B;
  --green:#10B981;
  --grad:linear-gradient(135deg,#FF6BAE 0%,#C084FC 100%);
}
body{font-family:'Noto Sans TC','Nunito',sans-serif;background:var(--bg);min-height:100vh;overflow-x:hidden;}
.page{display:none;flex-direction:column;min-height:100vh;padding-bottom:80px;}
.page.active{display:flex;}
.nav{
  position:fixed;bottom:0;left:0;right:0;background:#fff;
  border-top:2px solid #F3E8FF;display:flex;z-index:200;
  padding-bottom:env(safe-area-inset-bottom,0px);
  box-shadow:0 -4px 20px rgba(155,93,229,.1);
}
.nav-btn{
  flex:1;display:flex;flex-direction:column;align-items:center;
  padding:10px 0 8px;gap:3px;cursor:pointer;
  border:none;background:none;transition:all .2s;
}
.nav-btn .n-icon{font-size:24px;transition:transform .2s;}
.nav-btn .n-label{font-size:10px;font-weight:700;color:var(--gray);}
.nav-btn.active .n-label{color:var(--purple);}
.nav-btn.active .n-icon{transform:scale(1.15);}
.section-pad{padding:0 14px;}
.cards-row{display:grid;grid-template-columns:1fr 1fr;gap:10px;padding:16px 14px 0;}
.kid-card{
  background:#fff;border-radius:22px;padding:18px 12px 16px;
  text-align:center;position:relative;overflow:hidden;
  box-shadow:0 4px 20px rgba(155,93,229,.12);cursor:pointer;
  transition:transform .2s;
}
.kid-card:active{transform:scale(.97);}
.kid-card.hong-card{border-top:4px solid var(--pink);}
.kid-card.yu-card{border-top:4px solid var(--purple);}
.kid-card .blob{
  position:absolute;top:-20px;right:-20px;width:70px;height:70px;
  border-radius:50%;opacity:.15;
}
.hong-card .blob{background:var(--pink);}
.yu-card .blob{background:var(--purple);}
.kid-avatar{
  width:52px;height:52px;border-radius:50%;
  display:flex;align-items:center;justify-content:center;
  font-size:26px;margin:0 auto 8px;
}
.hong-card .kid-avatar{background:linear-gradient(135deg,#FFB3D4,#E84D8A);}
.yu-card .kid-avatar{background:linear-gradient(135deg,#E9D5FF,#9B5DE5);}
.kid-name{font-size:14px;font-weight:900;color:var(--text);margin-bottom:4px;}
.kid-pts{font-size:46px;font-weight:900;line-height:1;font-family:'Nunito',sans-serif;}
.hong-card .kid-pts{color:var(--pink);}
.yu-card .kid-pts{color:var(--purple);}
.pts-label{font-size:11px;color:var(--gray);margin-top:2px;}
.week-wrap{
  margin:12px 14px 0;background:#fff;border-radius:20px;
  padding:14px 10px;box-shadow:0 4px 16px rgba(155,93,229,.1);
}
.week-row{display:flex;gap:4px;}
.day-cell{
  flex:1;display:flex;flex-direction:column;align-items:center;gap:4px;
  cursor:pointer;padding:8px 2px;border-radius:14px;
  transition:all .2s;border:2px solid transparent;
}
.day-cell:active{background:#F9F0FF;}
.day-cell .d-circle{
  width:32px;height:32px;border-radius:50%;
  display:flex;align-items:center;justify-content:center;
  font-size:15px;font-weight:800;color:var(--gray);
  background:#F3E8FF;transition:all .2s;
}
.day-cell .d-label{font-size:10px;font-weight:700;color:var(--gray);}
.day-cell.done .d-circle{background:var(--pink2);color:#fff;}
.day-cell.today{border-color:var(--purple2);}
.day-cell.today .d-label{color:var(--purple);font-weight:900;}
.day-cell.today .d-circle{background:var(--purple);color:#fff;}
.day-cell.done.today .d-circle{background:linear-gradient(135deg,var(--pink),var(--purple));}
.kid-tabs{display:flex;gap:10px;padding:14px 14px 0;}
.kid-tab{
  flex:1;display:flex;align-items:center;justify-content:center;gap:6px;
  padding:11px 8px;border-radius:50px;border:2px solid #E9D5FF;
  font-size:14px;font-weight:800;color:var(--gray);
  cursor:pointer;transition:all .25s;background:#fff;font-family:inherit;
}
.kid-tab.active.ht{background:linear-gradient(135deg,#FFB3D4,#E84D8A);border-color:transparent;color:#fff;box-shadow:0 4px 16px rgba(232,77,138,.35);}
.kid-tab.active.yt{background:linear-gradient(135deg,#E9D5FF,#9B5DE5);border-color:transparent;color:#fff;box-shadow:0 4px 16px rgba(155,93,229,.35);}
.task-header{margin:14px 14px 10px;display:flex;align-items:center;gap:10px;}
.task-header-text{font-size:16px;font-weight:900;color:var(--text);}
.task-count{background:var(--purple);color:#fff;font-size:12px;font-weight:800;border-radius:50px;padding:2px 10px;}
.task-hint{
  margin:0 14px 10px;background:linear-gradient(135deg,#FFF5F9,#F9F0FF);
  border-radius:14px;padding:10px 14px;font-size:13px;font-weight:700;
  color:var(--purple);border-left:4px solid var(--purple2);
}
.tasks-list{padding:0 14px;display:flex;flex-direction:column;gap:8px;}
.task-row{
  background:#fff;border-radius:16px;padding:14px 14px 14px 12px;
  display:flex;align-items:center;gap:12px;
  box-shadow:0 2px 12px rgba(155,93,229,.08);
  border:2px solid transparent;cursor:pointer;transition:all .2s;
}
.task-row:active{transform:scale(.98);}
.task-row.done{border-color:#D1FAE5;background:#F0FDF4;}
.task-row.ht{border-left:4px solid var(--pink-light);}
.task-row.ht.done{border-left:4px solid var(--green);}
.task-row.yt{border-left:4px solid var(--purple-light);}
.task-row.yt.done{border-left:4px solid var(--green);}
.check-btn{
  width:30px;height:30px;border-radius:50%;border:2.5px solid var(--pink-light);
  display:flex;align-items:center;justify-content:center;flex-shrink:0;
  transition:all .2s;font-size:16px;color:transparent;
}
.task-row.done .check-btn{background:var(--green);border-color:var(--green);color:#fff;}
.task-name{flex:1;font-size:14px;font-weight:700;color:var(--text);}
.task-row.done .task-name{color:#6B7280;text-decoration:line-through;}
.pts-chip{
  display:flex;align-items:center;gap:3px;background:#FFF3E0;
  border-radius:50px;padding:4px 10px;font-size:13px;font-weight:800;color:var(--orange);
}
.task-row.done .pts-chip{background:#D1FAE5;color:var(--green);}
.page-title-bar{
  background:var(--grad);padding:20px 16px 14px;
  font-size:18px;font-weight:900;color:#fff;
  display:flex;align-items:center;gap:8px;
}
.kid-select-row{display:flex;gap:10px;padding:14px 14px 4px;}
.ks-btn{
  flex:1;padding:10px;border-radius:14px;border:2px solid #E9D5FF;
  font-size:14px;font-weight:800;cursor:pointer;background:#fff;
  transition:all .2s;color:var(--gray);font-family:inherit;
}
.ks-btn.active.h{background:linear-gradient(135deg,#FFB3D4,#E84D8A);color:#fff;border-color:transparent;}
.ks-btn.active.y{background:linear-gradient(135deg,#E9D5FF,#9B5DE5);color:#fff;border-color:transparent;}
.redeem-grid{padding:0 14px;display:flex;flex-direction:column;gap:10px;}
.reward-card{
  background:#fff;border-radius:18px;padding:14px 16px;
  display:flex;align-items:center;gap:14px;
  box-shadow:0 2px 12px rgba(155,93,229,.1);border:2px solid #F3E8FF;
}
.r-icon{font-size:32px;flex-shrink:0;}
.r-info{flex:1;}
.r-name{font-size:15px;font-weight:800;color:var(--text);}
.r-cost{font-size:12px;color:var(--gray);margin-top:2px;}
.r-btn{
  padding:9px 16px;border-radius:50px;border:none;
  font-size:13px;font-weight:800;cursor:pointer;transition:all .2s;font-family:inherit;
}
.r-btn.can{background:var(--grad);color:#fff;box-shadow:0 4px 14px rgba(155,93,229,.3);}
.r-btn.can:active{transform:scale(.95);}
.r-btn.cant{background:#F3F4F6;color:#D1D5DB;cursor:not-allowed;}
.sec-label{font-size:14px;font-weight:900;color:var(--text);padding:12px 14px 6px;display:flex;align-items:center;gap:6px;}
.tickets-wrap{padding:0 14px;display:flex;flex-direction:column;gap:8px;}
.ticket{
  background:#fff;border-radius:16px;padding:12px 14px;
  display:flex;align-items:center;gap:12px;
  border:2px solid #F3E8FF;position:relative;overflow:hidden;
}
.ticket::before{content:'';position:absolute;left:0;top:0;bottom:0;width:5px;background:var(--grad);}
.ticket.used::before{background:#D1D5DB;}
.ticket.used{opacity:.6;}
.t-icon{font-size:24px;}
.t-info{flex:1;}
.t-name{font-size:14px;font-weight:700;color:var(--text);}
.t-meta{font-size:11px;color:var(--gray);margin-top:2px;}
.t-tag{font-size:10px;font-weight:800;padding:4px 9px;border-radius:50px;white-space:nowrap;}
.t-tag.pending{background:#FFF0FA;color:var(--pink);border:1.5px solid var(--pink-light);}
.t-tag.confirmed{background:#F0F0F0;color:#aaa;border:1.5px solid #ddd;}
.parent-locked{
  flex:1;display:flex;flex-direction:column;align-items:center;
  justify-content:center;padding:40px 30px;gap:14px;
}
.numpad{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;width:100%;max-width:280px;}
.num-btn{
  padding:16px;border-radius:16px;border:2px solid #E9D5FF;
  font-size:22px;font-weight:800;cursor:pointer;background:#fff;
  transition:all .15s;font-family:inherit;color:var(--text);
}
.num-btn:active{transform:scale(.93);background:var(--purple-light);}
.num-btn.del{font-size:18px;color:var(--pink);}
.pw-dots{display:flex;gap:14px;justify-content:center;}
.pw-dot{width:16px;height:16px;border-radius:50%;border:2.5px solid var(--purple-light);transition:all .2s;}
.pw-dot.filled{background:var(--purple);border-color:var(--purple);}
.btn-login{
  width:100%;max-width:280px;padding:15px;border-radius:16px;border:none;
  background:var(--grad);color:#fff;font-size:16px;font-weight:900;
  cursor:pointer;font-family:inherit;box-shadow:0 6px 20px rgba(155,93,229,.35);
}
.btn-login:active{transform:scale(.97);}
.err{color:var(--pink);font-size:13px;font-weight:700;min-height:20px;text-align:center;}
.panel-header{
  background:var(--grad);padding:20px 16px 16px;
  display:flex;align-items:center;gap:10px;
}
.panel-header-title{font-size:18px;font-weight:900;color:#fff;}
.logout-btn{
  margin-left:auto;background:rgba(255,255,255,.3);
  border:2px solid rgba(255,255,255,.5);border-radius:50px;
  padding:6px 14px;color:#fff;font-size:12px;font-weight:800;
  cursor:pointer;font-family:inherit;
}
.p-section{margin:12px 14px 0;background:#fff;border-radius:20px;overflow:hidden;box-shadow:0 2px 12px rgba(155,93,229,.08);border:2px solid #F3E8FF;}
.p-sec-title{padding:13px 16px;font-size:14px;font-weight:900;color:var(--text);background:#FAFAFF;border-bottom:2px solid #F3E8FF;display:flex;align-items:center;gap:6px;}
.p-item{display:flex;align-items:center;gap:10px;padding:12px 16px;border-bottom:1.5px solid #F9F0FF;}
.p-item:last-child{border-bottom:none;}
.p-item-icon{font-size:20px;flex-shrink:0;}
.p-item-info{flex:1;}
.p-item-name{font-size:14px;font-weight:700;color:var(--text);}
.p-item-sub{font-size:11px;color:var(--gray);margin-top:1px;}
.ibt{width:34px;height:34px;border-radius:10px;border:none;display:flex;align-items:center;justify-content:center;font-size:15px;cursor:pointer;transition:all .2s;flex-shrink:0;}
.ibt:active{transform:scale(.9);}
.ibt.edit{background:#F3E8FF;color:var(--purple);}
.ibt.del{background:#FFF0F5;color:var(--pink);}
.ibt.ok{background:#D1FAE5;color:var(--green);}
.ibt.rej{background:#FFF0F5;color:var(--pink);}
.add-form{padding:12px 14px;background:#FAFAFF;border-top:2px solid #F3E8FF;}
.add-row{display:flex;gap:8px;margin-bottom:8px;}
.add-row:last-child{margin-bottom:0;}
.inp{flex:1;padding:10px 12px;border-radius:12px;border:2px solid #E9D5FF;font-size:13px;font-family:inherit;outline:none;min-width:0;}
.inp:focus{border-color:var(--purple);}
.inp.sm{max-width:70px;}
.inp.md{max-width:90px;}
.sel{flex:1;padding:10px 12px;border-radius:12px;border:2px solid #E9D5FF;font-size:13px;font-family:inherit;outline:none;background:#fff;cursor:pointer;}
.add-btn{padding:10px 16px;border-radius:12px;border:none;background:var(--grad);color:#fff;font-size:13px;font-weight:800;cursor:pointer;font-family:inherit;white-space:nowrap;transition:all .2s;}
.add-btn:active{transform:scale(.95);}
.log-item{display:flex;align-items:center;gap:10px;padding:10px 16px;border-bottom:1.5px solid #F9F0FF;}
.log-item:last-child{border-bottom:none;}
.log-info{flex:1;}
.log-who{font-size:13px;font-weight:700;color:var(--text);}
.log-reason{font-size:11px;color:var(--gray);}
.log-date{font-size:10px;color:#ccc;}
.log-pts{font-size:13px;font-weight:800;padding:3px 8px;border-radius:50px;color:#fff;white-space:nowrap;}
.log-pts.pos{background:var(--green);}
.log-pts.neg{background:var(--pink);}
.overlay{display:none;position:fixed;inset:0;z-index:500;background:rgba(0,0,0,.45);backdrop-filter:blur(6px);align-items:center;justify-content:center;padding:20px;}
.overlay.open{display:flex;}
.modal{background:#fff;border-radius:24px;padding:26px;width:100%;max-width:360px;animation:popIn .3s cubic-bezier(.34,1.56,.64,1);}
@keyframes popIn{from{transform:scale(.85);opacity:0;}to{transform:scale(1);opacity:1;}}
.modal h3{font-size:18px;font-weight:900;color:var(--text);margin-bottom:16px;text-align:center;}
.modal-inp{width:100%;padding:12px 14px;border-radius:14px;border:2.5px solid #E9D5FF;font-size:15px;font-family:inherit;outline:none;margin-bottom:10px;}
.modal-inp:focus{border-color:var(--purple);}
.m-btn{width:100%;padding:13px;border-radius:14px;border:none;font-size:15px;font-weight:800;cursor:pointer;font-family:inherit;margin-bottom:8px;transition:all .2s;}
.m-btn:active{transform:scale(.97);}
.m-btn.primary{background:var(--grad);color:#fff;box-shadow:0 6px 20px rgba(155,93,229,.3);}
.m-btn.secondary{background:#F3F4F6;color:var(--gray);border:2px solid #E9D5FF;}
.m-btn.danger{background:var(--pink);color:#fff;}
.sheet-overlay{display:none;position:fixed;inset:0;z-index:400;background:rgba(0,0,0,.35);backdrop-filter:blur(4px);align-items:flex-end;justify-content:center;}
.sheet-overlay.open{display:flex;}
.sheet{background:#fff;border-radius:24px 24px 0 0;width:100%;max-width:480px;padding:20px;max-height:70vh;overflow-y:auto;animation:slideUp .3s cubic-bezier(.34,1.56,.64,1);}
@keyframes slideUp{from{transform:translateY(100%);}to{transform:translateY(0);}}
.sheet-title{font-size:17px;font-weight:900;color:var(--text);margin-bottom:14px;display:flex;align-items:center;justify-content:space-between;}
.sheet-close{background:#F3E8FF;border:none;font-size:16px;cursor:pointer;color:var(--gray);width:32px;height:32px;border-radius:50%;display:flex;align-items:center;justify-content:center;}
.sheet-task{display:flex;align-items:center;gap:10px;padding:10px 12px;border-radius:14px;margin-bottom:6px;border:2px solid #F3E8FF;background:#FAFAFF;}
.sheet-task.done{background:#F0FDF4;border-color:#BBF7D0;}
.toast{position:fixed;top:16px;left:50%;transform:translateX(-50%) translateY(-70px);background:linear-gradient(135deg,var(--pink),var(--purple));color:#fff;padding:11px 24px;border-radius:50px;font-size:14px;font-weight:800;box-shadow:0 8px 30px rgba(155,93,229,.4);z-index:999;transition:transform .35s cubic-bezier(.34,1.56,.64,1);white-space:nowrap;pointer-events:none;}
.toast.show{transform:translateX(-50%) translateY(0);}
.empty{text-align:center;padding:24px;color:var(--gray);font-size:14px;}
.empty-e{font-size:36px;display:block;margin-bottom:8px;}
</style>
</head>
<body>

<div class="toast" id="toast"></div>

<!-- ── HOME PAGE ── -->
<div class="page active" id="pg-home">
  <div style="background:var(--grad);padding:18px 16px 14px;display:flex;align-items:center;justify-content:space-between;">
    <div>
      <div style="font-size:19px;font-weight:900;color:#fff;">✨ 自律生活公約</div>
      <div style="font-size:12px;color:rgba(255,255,255,.8);margin-top:2px;">每天進步一點點！</div>
    </div>
    <div style="font-size:11px;color:rgba(255,255,255,.8);" id="today-label"></div>
  </div>
  <div class="cards-row">
    <div class="kid-card hong-card" onclick="switchKidTab('hong')">
      <div class="blob"></div>
      <div class="kid-avatar">🦁</div>
      <div class="kid-name">泓愷</div>
      <div class="kid-pts" id="pts-hong">0</div>
      <div class="pts-label">⭐ 累積點數</div>
    </div>
    <div class="kid-card yu-card" onclick="switchKidTab('yu')">
      <div class="blob"></div>
      <div class="kid-avatar">🐯</div>
      <div class="kid-name">昱廷</div>
      <div class="kid-pts" id="pts-yu">0</div>
      <div class="pts-label">⭐ 累積點數</div>
    </div>
  </div>
  <div class="week-wrap">
    <div class="week-row" id="week-bar"></div>
  </div>
  <div class="kid-tabs">
    <button class="kid-tab ht active" id="tab-hong" onclick="switchKidTab('hong')">🦁 泓愷</button>
    <button class="kid-tab yt" id="tab-yu" onclick="switchKidTab('yu')">🐯 昱廷</button>
  </div>
  <div class="task-header section-pad">
    <span style="font-size:22px">📋</span>
    <span class="task-header-text">今日任務</span>
    <span class="task-count" id="task-count">0/0</span>
  </div>
  <div class="task-hint section-pad">⚡ 完成任務得點數！</div>
  <div class="tasks-list" id="home-tasks"></div>
  <div style="height:10px"></div>
</div>

<!-- ── REDEEM PAGE ── -->
<div class="page" id="pg-redeem">
  <div class="page-title-bar">🎁 兌換中心</div>
  <div class="kid-select-row">
    <button class="ks-btn h active" id="rs-hong" onclick="switchRedeemKid('hong')">🦁 泓愷</button>
    <button class="ks-btn y" id="rs-yu" onclick="switchRedeemKid('yu')">🐯 昱廷</button>
  </div>
  <div class="sec-label">🛒 可兌換獎勵</div>
  <div class="redeem-grid" id="redeem-available"></div>
  <div class="sec-label">🎫 我的獎勵券</div>
  <div class="tickets-wrap" id="redeem-tickets"></div>
  <div style="height:10px"></div>
</div>

<!-- ── PARENT PAGE ── -->
<div class="page" id="pg-parent">
  <div class="parent-locked" id="parent-locked">
    <div style="font-size:60px">🔐</div>
    <div style="font-size:22px;font-weight:900;color:var(--text);">家長專區</div>
    <div style="font-size:14px;color:var(--gray);text-align:center;">請輸入3位密碼進入管理介面</div>
    <div class="pw-dots">
      <div class="pw-dot" id="dot0"></div>
      <div class="pw-dot" id="dot1"></div>
      <div class="pw-dot" id="dot2"></div>
    </div>
    <div class="err" id="pw-err"></div>
    <div class="numpad">
      <button class="num-btn" onclick="numPress(1)">1</button>
      <button class="num-btn" onclick="numPress(2)">2</button>
      <button class="num-btn" onclick="numPress(3)">3</button>
      <button class="num-btn" onclick="numPress(4)">4</button>
      <button class="num-btn" onclick="numPress(5)">5</button>
      <button class="num-btn" onclick="numPress(6)">6</button>
      <button class="num-btn" onclick="numPress(7)">7</button>
      <button class="num-btn" onclick="numPress(8)">8</button>
      <button class="num-btn" onclick="numPress(9)">9</button>
      <button class="num-btn" style="grid-column:2" onclick="numPress(0)">0</button>
      <button class="num-btn del" style="grid-column:3" onclick="numDel()">⌫</button>
    </div>
    <button class="btn-login" onclick="doLogin()">🔓 登入</button>
  </div>
  <div id="parent-panel" style="display:none;padding-bottom:20px;">
    <div class="panel-header">
      <div class="panel-header-title">👑 家長管理介面</div>
      <button class="logout-btn" onclick="doLogout()">登出</button>
    </div>
    <div class="p-section">
      <div class="p-sec-title">⏳ 待確認兌換申請</div>
      <div id="p-pending"></div>
    </div>
    <div class="p-section">
      <div class="p-sec-title">💰 點數調整（獎懲）</div>
      <div class="add-form">
        <div class="add-row">
          <select class="sel" id="adj-kid"><option value="hong">🦁 泓愷</option><option value="yu">🐯 昱廷</option></select>
          <input class="inp md" type="number" id="adj-pts" placeholder="點數（負=扣）">
        </div>
        <div class="add-row">
          <input class="inp" type="text" id="adj-reason" placeholder="原因說明">
          <button class="add-btn" onclick="adjustPts()">確認</button>
        </div>
      </div>
    </div>
    <div class="p-section">
      <div class="p-sec-title">📋 任務管理</div>
      <div id="p-tasks"></div>
      <div class="add-form">
        <div class

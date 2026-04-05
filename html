<!DOCTYPE html>
<html lang="zh-TW">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>🐾 貓窩社群小編系統</title>
<link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800;900&family=Noto+Sans+TC:wght@400;500;700;900&display=swap" rel="stylesheet">
<style>
:root {
  --pink:#FFB5C8; --pink2:#FF8FAB; --pink-bg:#FFF0F4;
  --blue:#A8D8EA; --blue2:#7EC8E3; --blue-bg:#EEF8FC;
  --mint:#B5EAD7; --mint2:#7DDBB0;
  --lemon:#FFEAA7; --lemon2:#FFD93D;
  --lav:#C3B1E1; --lav2:#A084CA;
  --peach:#FFCBA4; --peach2:#FFB07C;
  --cream:#FFFDF9; --white:#fff;
  --text:#5D4E75; --text2:#8B7BA8; --text3:#B3A5C8;
  --border:#EDD9F0;
  --shadow:rgba(180,140,220,.15); --shadow2:rgba(255,182,200,.25);
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--cream);color:var(--text);font-family:'Nunito','Noto Sans TC',sans-serif;min-height:100vh;overflow-x:hidden}
body::before{content:'';position:fixed;inset:0;background:radial-gradient(ellipse 80% 60% at 10% 0%,rgba(255,181,200,.18),transparent 60%),radial-gradient(ellipse 60% 50% at 90% 0%,rgba(168,216,234,.18),transparent 60%),radial-gradient(ellipse 50% 40% at 50% 100%,rgba(181,234,215,.15),transparent 60%),var(--cream);pointer-events:none;z-index:0}
.bubbles{position:fixed;inset:0;pointer-events:none;z-index:0;overflow:hidden}
.bubble{position:absolute;border-radius:50%;opacity:.22;animation:floatB linear infinite}
@keyframes floatB{0%{transform:translateY(110vh) scale(.5);opacity:0}10%{opacity:.22}90%{opacity:.22}100%{transform:translateY(-10vh) scale(1.2);opacity:0}}

/* HEADER */
header{position:sticky;top:0;z-index:200;background:rgba(255,255,255,.88);backdrop-filter:blur(16px);border-bottom:2px dashed var(--border);padding:0 28px;height:68px;display:flex;align-items:center;justify-content:space-between}
.logo{display:flex;align-items:center;gap:12px}
.logo-blob{width:44px;height:44px;background:linear-gradient(135deg,var(--pink),var(--blue));border-radius:50% 50% 50% 50%/60% 60% 40% 40%;display:flex;align-items:center;justify-content:center;font-size:22px;box-shadow:0 4px 12px var(--shadow2);animation:blobP 3s ease-in-out infinite}
@keyframes blobP{0%,100%{border-radius:50% 50% 50% 50%/60% 60% 40% 40%}50%{border-radius:60% 40% 60% 40%/40% 60% 40% 60%}}
.logo-name{font-size:20px;font-weight:900;background:linear-gradient(135deg,var(--pink2),var(--lav2));-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.logo-en{font-size:10px;color:var(--text3);font-weight:700;letter-spacing:.12em}
.hpills{display:flex;gap:8px}
.pill{padding:6px 14px;border-radius:20px;font-size:12px;font-weight:800;border:none;cursor:default;white-space:nowrap;font-family:inherit}
.ppink{background:var(--pink);color:#fff}
.pblue{background:var(--blue2);color:#fff}

/* LAYOUT */
.layout{display:grid;grid-template-columns:250px 1fr;min-height:calc(100vh - 68px);position:relative;z-index:1}

/* SIDEBAR */
.sidebar{background:rgba(255,255,255,.7);backdrop-filter:blur(12px);border-right:2px dashed var(--border);padding:20px 14px;display:flex;flex-direction:column;gap:3px;position:sticky;top:68px;height:calc(100vh - 68px);overflow-y:auto}
.sb-deco{text-align:center;padding:10px 0 18px;border-bottom:2px dashed var(--border);margin-bottom:14px}
.sb-cat{font-size:46px;display:inline-block;animation:sway 4s ease-in-out infinite}
@keyframes sway{0%,100%{transform:rotate(-5deg)}50%{transform:rotate(5deg)}}
.sb-deco p{font-size:11px;color:var(--text3);font-weight:700;margin-top:4px}
.nsec{font-size:10px;font-weight:800;letter-spacing:.12em;color:var(--text3);padding:10px 10px 4px;text-transform:uppercase}
.nitem{display:flex;align-items:center;gap:9px;padding:9px 12px;border-radius:14px;cursor:pointer;font-size:13px;font-weight:700;color:var(--text2);transition:all .2s;border:2px solid transparent}
.nitem:hover{background:var(--pink-bg);color:var(--pink2)}
.nitem.active{background:linear-gradient(135deg,var(--pink-bg),var(--blue-bg));border-color:var(--pink);color:var(--pink2)}
.nitem .ne{font-size:17px}
.nbadge{margin-left:auto;background:var(--pink2);color:#fff;font-size:9px;font-weight:900;padding:2px 6px;border-radius:10px}

/* CONTENT */
.content{padding:26px 30px 80px;overflow-y:auto}
.page{display:none;animation:pgIn .3s ease}
.page.active{display:block}
@keyframes pgIn{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:translateY(0)}}

/* PAGE HERO */
.hero{display:flex;align-items:flex-start;gap:18px;margin-bottom:24px;padding:22px 26px;background:#fff;border-radius:22px;border:2px solid var(--border);box-shadow:0 6px 24px var(--shadow);position:relative;overflow:hidden}
.hero::after{content:'';position:absolute;right:-20px;top:-20px;width:110px;height:110px;border-radius:50%;background:linear-gradient(135deg,var(--pink),var(--lemon));opacity:.12}
.hero-icon{font-size:50px;line-height:1;flex-shrink:0}
.hero-title{font-size:24px;font-weight:900;color:var(--text);margin-bottom:4px}
.hero-desc{font-size:13px;color:var(--text2);line-height:1.7;font-weight:600}

/* CARD */
.card{background:#fff;border-radius:20px;border:2px solid var(--border);padding:20px 22px;margin-bottom:16px;box-shadow:0 4px 16px var(--shadow);transition:box-shadow .2s}
.card:hover{box-shadow:0 8px 28px var(--shadow2)}
.ch{display:flex;align-items:center;gap:10px;margin-bottom:16px}
.ci{width:34px;height:34px;border-radius:11px;display:flex;align-items:center;justify-content:center;font-size:17px;flex-shrink:0}
.cip{background:var(--pink-bg)} .cib{background:var(--blue-bg)} .cim{background:rgba(181,234,215,.25)} .cil{background:rgba(255,234,167,.3)} .civ{background:rgba(195,177,225,.2)}
.ctitle{font-size:14px;font-weight:900;color:var(--text)}
.csub{font-size:11px;color:var(--text3);font-weight:600}

/* GRID */
.g2{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.g3{display:grid;grid-template-columns:1fr 1fr 1fr;gap:12px}
.g4{display:grid;grid-template-columns:repeat(4,1fr);gap:12px}

/* BUTTONS */
.btn{display:inline-flex;align-items:center;gap:7px;padding:10px 20px;border-radius:50px;font-size:13px;font-weight:800;font-family:inherit;cursor:pointer;border:none;transition:all .2s}
.btn:active{transform:scale(.96)}
.bpink{background:linear-gradient(135deg,var(--pink2),#ff6b9d);color:#fff;box-shadow:0 4px 14px rgba(255,100,150,.35)}
.bpink:hover{transform:translateY(-2px);box-shadow:0 6px 20px rgba(255,100,150,.45)}
.bblue{background:linear-gradient(135deg,var(--blue2),#5bb8d4);color:#fff;box-shadow:0 4px 14px rgba(100,180,220,.35)}
.bblue:hover{transform:translateY(-2px)}
.bmint{background:linear-gradient(135deg,var(--mint2),#5dc99a);color:#fff;box-shadow:0 4px 14px rgba(100,200,160,.35)}
.bmint:hover{transform:translateY(-2px)}
.bghost{background:#fff;color:var(--text2);border:2px solid var(--border)}
.bghost:hover{border-color:var(--pink);color:var(--pink2)}
.blemon{background:linear-gradient(135deg,var(--lemon2),#ffb347);color:#fff}
.blav{background:linear-gradient(135deg,var(--lav),var(--lav2));color:#fff}
.bsm{padding:7px 14px;font-size:12px}
.bxs{padding:5px 10px;font-size:11px}

/* FORM */
.fg{margin-bottom:14px}
label{display:block;font-size:12px;font-weight:800;color:var(--text2);margin-bottom:5px;letter-spacing:.05em}
input,textarea,select{width:100%;background:var(--pink-bg);border:2px solid var(--border);border-radius:13px;padding:9px 13px;color:var(--text);font-family:inherit;font-size:13px;font-weight:600;outline:none;transition:all .2s;-webkit-appearance:none}
input:focus,textarea:focus,select:focus{border-color:var(--pink);background:#fff;box-shadow:0 0 0 4px rgba(255,143,171,.12)}
textarea{resize:vertical;line-height:1.7}
select{cursor:pointer}

/* POST TYPE CARDS */
.tcards{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:18px}
.tcard{border:3px solid var(--border);border-radius:18px;padding:16px;cursor:pointer;transition:all .25s;text-align:center;background:#fff;position:relative;overflow:hidden}
.tcard:hover,.tcard.sel{transform:translateY(-3px);box-shadow:0 8px 24px var(--shadow2)}
.tcard.nanny.sel{border-color:var(--pink2);background:rgba(255,181,200,.08)}
.tcard.foster.sel{border-color:var(--blue2);background:rgba(168,216,234,.1)}
.tcard-em{font-size:34px;margin-bottom:9px;display:block}
.tcard-t{font-size:14px;font-weight:900;color:var(--text);margin-bottom:3px}
.tcard-d{font-size:11px;color:var(--text2);font-weight:600;line-height:1.5}
.tcbadge{position:absolute;top:10px;right:10px;background:var(--pink);color:#fff;font-size:9px;font-weight:900;padding:3px 7px;border-radius:10px}

/* PLATFORM PILLS */
.platrow{display:flex;gap:7px;flex-wrap:wrap;margin-bottom:16px}
.pbtn{padding:8px 15px;border-radius:50px;font-size:12px;font-weight:800;font-family:inherit;cursor:pointer;border:2px solid var(--border);background:#fff;color:var(--text3);transition:all .2s;display:flex;align-items:center;gap:5px}
.pbtn:hover{border-color:var(--pink);color:var(--pink2)}
.pbtn.active.fb{background:#1877f2;border-color:#1877f2;color:#fff}
.pbtn.active.ig{background:linear-gradient(135deg,#f09433,#e6683c,#dc2743,#cc2366);border-color:#dc2743;color:#fff}
.pbtn.active.th{background:#111;border-color:#111;color:#fff}

/* POST OUTPUT */
.post-out{border:3px dashed var(--border);border-radius:18px;padding:20px;min-height:130px;background:linear-gradient(135deg,var(--pink-bg),var(--blue-bg));font-size:14px;line-height:1.9;font-weight:600;white-space:pre-wrap;word-break:break-word;position:relative}
.post-out:empty::before{content:'貼文將顯示在這裡 ✨';color:var(--text3);font-style:italic}
.out-acts{display:flex;gap:8px;margin-top:11px;flex-wrap:wrap}
.charcount{text-align:right;font-size:11px;font-weight:700;color:var(--text3);margin-top:4px}

/* TABS */
.tabrow{display:flex;gap:0;margin-bottom:14px;background:var(--pink-bg);border-radius:15px;padding:4px;border:2px solid var(--border)}
.tabi{flex:1;text-align:center;padding:8px 10px;border-radius:11px;font-size:12px;font-weight:800;cursor:pointer;color:var(--text3);transition:all .2s}
.tabi.active{background:#fff;color:var(--pink2);box-shadow:0 2px 8px var(--shadow)}

/* TOPIC ITEMS */
.titem{display:flex;align-items:center;gap:11px;padding:11px 13px;border-radius:13px;border:2px solid var(--border);margin-bottom:7px;cursor:pointer;background:#fff;transition:all .2s}
.titem:hover,.titem.sel{border-color:var(--pink);background:var(--pink-bg);transform:translateX(4px)}
.titem.foster:hover,.titem.foster.sel{border-color:var(--blue2);background:var(--blue-bg)}
.tdot{width:9px;height:9px;border-radius:50%;flex-shrink:0}
.tdp{background:var(--pink2)} .tdb{background:var(--blue2)}
.ttext{font-size:13px;font-weight:700;flex:1;color:var(--text)}
.tbadge{font-size:10px;font-weight:800;padding:3px 8px;border-radius:10px}
.tb-hot{background:rgba(255,143,171,.2);color:var(--pink2)}
.tb-up{background:rgba(126,200,163,.2);color:var(--mint2)}
.tb-new{background:rgba(168,216,234,.25);color:var(--blue2)}

/* STATS */
.sblob{background:#fff;border-radius:18px;border:2px solid var(--border);padding:18px;text-align:center;box-shadow:0 4px 16px var(--shadow);transition:transform .2s;position:relative;overflow:hidden}
.sblob:hover{transform:translateY(-3px)}
.sblob::before{content:'';position:absolute;inset:-1px;border-radius:18px;opacity:.11;z-index:0}
.sbp::before{background:linear-gradient(135deg,var(--pink),var(--lemon))}
.sbb::before{background:linear-gradient(135deg,var(--blue),var(--mint))}
.sbm::before{background:linear-gradient(135deg,var(--mint),var(--lemon))}
.sbv::before{background:linear-gradient(135deg,var(--lav),var(--blue))}
.sblob>*{position:relative;z-index:1}
.sem{font-size:26px;margin-bottom:7px;display:block}
.snum{font-size:34px;font-weight:900;line-height:1;margin-bottom:3px}
.snp{color:var(--pink2)}.snb{color:var(--blue2)}.snm{color:var(--mint2)}.snv{color:var(--lav2)}
.slabel{font-size:12px;font-weight:800;color:var(--text2)}
.ssub{font-size:11px;color:var(--text3);margin-top:3px;font-weight:600}

/* PROGRESS */
.pw{margin:7px 0}
.ph{display:flex;justify-content:space-between;font-size:12px;font-weight:800;color:var(--text2);margin-bottom:5px}
.pb{height:10px;background:var(--pink-bg);border-radius:10px;overflow:hidden;border:1px solid var(--border)}
.pf{height:100%;border-radius:10px;transition:width .8s cubic-bezier(.17,.67,.35,1.1)}
.pfp{background:linear-gradient(90deg,var(--pink),var(--pink2))}
.pfb{background:linear-gradient(90deg,var(--blue),var(--blue2))}
.pfm{background:linear-gradient(90deg,var(--mint),var(--mint2))}

/* WEEK */
.wgrid{display:grid;grid-template-columns:repeat(7,1fr);gap:6px;margin-top:13px}
.dcol{display:flex;flex-direction:column;gap:6px}
.dhead{text-align:center;font-size:11px;font-weight:900;color:var(--text3);padding:7px 3px;background:var(--pink-bg);border-radius:9px}
.dhead.today{background:linear-gradient(135deg,var(--pink),var(--blue));color:#fff}
.dpost{background:#fff;border:2px solid var(--border);border-radius:11px;padding:7px 6px;font-size:10px;font-weight:700;cursor:pointer;transition:all .2s;line-height:1.4}
.dpost:hover{transform:scale(1.04);box-shadow:0 4px 10px var(--shadow2)}
.dpost.nanny{border-left:4px solid var(--pink2)}
.dpost.foster{border-left:4px solid var(--blue2)}
.dpt{font-size:10px;font-weight:900;margin-bottom:2px}
.dptn{color:var(--pink2)}.dptf{color:var(--blue2)}
.dptx{color:var(--text2);font-size:10px}

/* TAGS */
.tagcloud{display:flex;flex-wrap:wrap;gap:7px}
.tchip{padding:5px 12px;border-radius:50px;font-size:12px;font-weight:800;font-family:inherit;cursor:pointer;border:2px solid var(--border);background:#fff;color:var(--text2);transition:all .18s}
.tchip:hover{border-color:var(--pink);color:var(--pink2)}
.tchip.sel{background:var(--pink);border-color:var(--pink);color:#fff;box-shadow:0 3px 10px var(--shadow2)}
.tchip.foster.sel{background:var(--blue2);border-color:var(--blue2)}

/* TIP BOX */
.tip{border-radius:15px;padding:13px 16px;font-size:13px;font-weight:700;line-height:1.7;margin-bottom:13px;display:flex;gap:11px;align-items:flex-start}
.tipicon{font-size:20px;flex-shrink:0;margin-top:1px}
.tp{background:rgba(255,181,200,.2);border:2px solid rgba(255,143,171,.35);color:var(--text)}
.tb2{background:rgba(168,216,234,.2);border:2px solid rgba(126,200,227,.35);color:var(--text)}
.tm{background:rgba(181,234,215,.25);border:2px solid rgba(125,219,176,.4);color:var(--text)}
.tl{background:rgba(255,234,167,.3);border:2px solid rgba(255,217,61,.35);color:var(--text)}

/* TIME SLOTS */
.tslot{display:flex;align-items:center;gap:14px;padding:14px 16px;border-radius:15px;border:2px solid var(--border);margin-bottom:9px;background:#fff;transition:all .2s}
.tslot:hover{border-color:var(--pink);box-shadow:0 4px 16px var(--shadow2)}
.tstime{font-size:24px;font-weight:900;color:var(--pink2);min-width:72px}
.tsinfo{flex:1}
.tstitle{font-size:13px;font-weight:800;color:var(--text);margin-bottom:3px}
.tsdesc{font-size:11px;color:var(--text3);font-weight:600;line-height:1.5}
.tsplats{display:flex;gap:5px}
.tsplat{width:25px;height:25px;border-radius:7px;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:900;color:#fff}
.tpfb{background:#1877f2}.tpig{background:linear-gradient(135deg,#f09433,#dc2743)}.tpth{background:#333}

/* CHECKLIST */
.crow{display:flex;align-items:center;gap:10px;padding:9px 0;border-bottom:1px dashed var(--border);font-size:13px;font-weight:700;cursor:pointer}
.crow:last-child{border-bottom:none}
.cbox{width:22px;height:22px;border-radius:7px;border:2px solid var(--border);background:#fff;display:flex;align-items:center;justify-content:center;flex-shrink:0;transition:all .2s;font-size:13px}
.crow.done .cbox{background:var(--mint2);border-color:var(--mint2);color:#fff}
.crow.done .clabel{text-decoration:line-through;color:var(--text3)}

/* FORMULA */
.fstep{display:flex;align-items:flex-start;gap:13px;padding:11px 0;border-bottom:1px dashed var(--border)}
.fstep:last-child{border-bottom:none}
.fnum{width:27px;height:27px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:900;flex-shrink:0;color:#fff}
.ftitle{font-size:13px;font-weight:800;color:var(--text);margin-bottom:2px}
.fdesc{font-size:12px;color:var(--text2);font-weight:600;line-height:1.6}

/* STRATEGY */
.pstrat{border-radius:17px;padding:16px;margin-bottom:11px;border:2px solid transparent}
.psfb{background:rgba(24,119,242,.06);border-color:rgba(24,119,242,.2)}
.psig{background:rgba(220,39,67,.06);border-color:rgba(220,39,67,.2)}
.psth{background:rgba(50,50,50,.05);border-color:rgba(50,50,50,.15)}
.pst{font-size:14px;font-weight:900;margin-bottom:7px;display:flex;align-items:center;gap:7px}
.psfb .pst{color:#1877f2}.psig .pst{color:#dc2743}.psth .pst{color:#333}
.psul{list-style:none}
.psul li{font-size:12px;font-weight:600;color:var(--text2);padding:3px 0;display:flex;align-items:flex-start;gap:7px;line-height:1.6}
.psul li::before{content:'🌸';flex-shrink:0;font-size:10px;margin-top:3px}

/* ORDER DOTS */
.odots{display:flex;gap:4px;flex-wrap:wrap;margin-top:13px}
.odot{width:31px;height:31px;border-radius:50%;border:3px solid var(--border);background:#fff;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:900;color:var(--text3);cursor:pointer;transition:all .2s}
.odot.done{background:linear-gradient(135deg,var(--pink),var(--lemon));border-color:var(--pink);color:#fff}
.odot:hover{border-color:var(--pink)}

/* IDEA CARDS */
.icard{background:#fff;border:2px solid var(--border);border-radius:15px;padding:15px;cursor:pointer;transition:all .2s;position:relative}
.icard:hover{border-color:var(--pink);transform:translateY(-3px);box-shadow:0 6px 20px var(--shadow2)}
.iem{font-size:22px;margin-bottom:7px}
.it{font-size:13px;font-weight:900;color:var(--text);margin-bottom:3px}
.id{font-size:11px;color:var(--text2);font-weight:600;line-height:1.5}
.ibadge{position:absolute;top:9px;right:9px;font-size:9px;font-weight:900;padding:3px 7px;border-radius:10px}
.ibn{background:var(--pink-bg);color:var(--pink2);border:1px solid var(--pink)}
.ibf{background:var(--blue-bg);color:var(--blue2);border:1px solid var(--blue2)}

/* MONTH TABLE */
.mtable{width:100%;border-collapse:collapse}
.mtable th{background:linear-gradient(135deg,var(--pink-bg),var(--blue-bg));font-size:11px;font-weight:900;color:var(--text2);padding:9px 11px;text-align:left;border-bottom:2px solid var(--border)}
.mtable td{padding:9px 11px;border-bottom:1px dashed var(--border);font-size:12px;font-weight:600;color:var(--text);vertical-align:top}
.mtable tr:hover td{background:var(--pink-bg)}

/* TOAST */
.toast{position:fixed;bottom:88px;right:22px;background:linear-gradient(135deg,var(--mint2),var(--blue2));color:#fff;padding:12px 20px;border-radius:50px;font-size:13px;font-weight:800;box-shadow:0 6px 24px rgba(100,200,160,.4);z-index:999;opacity:0;transform:translateY(10px);transition:all .3s;pointer-events:none}
.toast.show{opacity:1;transform:translateY(0)}

/* TICKER */
.ticker-bar{position:fixed;bottom:0;left:0;right:0;z-index:100;background:linear-gradient(135deg,var(--pink),var(--blue),var(--mint),var(--lemon));padding:8px 0;overflow:hidden;border-top:2px solid rgba(255,255,255,.4)}
.ticker-in{display:flex;gap:30px;animation:tick 28s linear infinite;width:max-content}
@keyframes tick{from{transform:translateX(0)}to{transform:translateX(-50%)}}
.titem{font-size:12px;font-weight:800;color:#fff;white-space:nowrap}

/* MISC */
.divider{height:2px;background:linear-gradient(90deg,var(--pink-bg),var(--border),var(--blue-bg));border-radius:2px;margin:18px 0}
.flex{display:flex}.ic{align-items:center}.jb{justify-content:space-between}
.gap8{gap:8px}.gap12{gap:12px}
.mb12{margin-bottom:12px}.mb16{margin-bottom:16px}.mb20{margin-bottom:20px}
.mt8{margin-top:8px}.mt12{margin-top:12px}
.tc{text-align:center}
.hidden{display:none!important}
.fade{animation:pgIn .3s ease}
::-webkit-scrollbar{width:7px}
::-webkit-scrollbar-track{background:var(--pink-bg)}
::-webkit-scrollbar-thumb{background:var(--pink);border-radius:10px}
</style>
</head>
<body>

<div class="bubbles" id="bubbles"></div>
<div class="toast" id="toast">✅ 已複製到剪貼簿！</div>

<!-- HEADER -->
<header>
  <div class="logo">
    <div class="logo-blob">🐱</div>
    <div>
      <div class="logo-name">貓窩社群小編系統 ✨</div>
      <div class="logo-en">CAT NEST SOCIAL MEDIA STUDIO — OFFLINE VERSION</div>
    </div>
  </div>
  <div class="hpills">
    <div class="pill ppink">🎯 目標 20 單 / 月</div>
    <div class="pill pblue">📱 FB · IG · 脆</div>
  </div>
</header>

<div class="layout">

<!-- SIDEBAR -->
<aside class="sidebar">
  <div class="sb-deco">
    <div class="sb-cat">🐈</div>
    <p>今天也要努力發文喵～</p>
  </div>
  <div class="nsec">✍️ 創作工具</div>
  <div class="nitem active" onclick="nav(this,'posts')"><span class="ne">📋</span> 現成貼文範本 <span class="nbadge">60篇</span></div>
  <div class="nitem" onclick="nav(this,'ideabank')"><span class="ne">💡</span> 貼文靈感庫</div>
  <div class="nitem" onclick="nav(this,'hashtags')"><span class="ne">🏷️</span> Hashtag 工具</div>
  <div class="nsec">📅 排程規劃</div>
  <div class="nitem" onclick="nav(this,'planner')"><span class="ne">🗓️</span> 週排程日曆</div>
  <div class="nitem" onclick="nav(this,'monthly')"><span class="ne">📆</span> 月度作戰計畫</div>
  <div class="nsec">📊 追蹤成效</div>
  <div class="nitem" onclick="nav(this,'dashboard')"><span class="ne">📈</span> 業績看板</div>
  <div class="nitem" onclick="nav(this,'checklist')"><span class="ne">✅</span> 每日發文清單</div>
  <div class="nsec">🗺️ 策略指南</div>
  <div class="nitem" onclick="nav(this,'strategy')"><span class="ne">🌈</span> 平台策略指南</div>
  <div class="nitem" onclick="nav(this,'formula')"><span class="ne">🧪</span> 貼文公式</div>
</aside>

<!-- CONTENT -->
<main class="content">

<!-- ══════ PAGE: POSTS ══════ -->
<div id="pg-posts" class="page active">
  <div class="hero">
    <div class="hero-icon">📋</div>
    <div>
      <div class="hero-title">現成貼文範本庫</div>
      <div class="hero-desc">60 篇精心撰寫的貼文範本，依平台分類！選好→自訂→複製貼上，馬上發文 🌸<br>粉色框可以直接編輯修改內容喔！</div>
    </div>
  </div>

  <!-- 篩選 -->
  <div class="card">
    <div class="ch"><div class="ci cip">🔍</div><div><div class="ctitle">選擇類型與平台</div></div></div>
    <div class="tcards">
      <div class="tcard nanny sel" id="tc-nanny" onclick="selType('nanny')">
        <div class="tcbadge">主力接單</div>
        <span class="tcard-em">🏠</span>
        <div class="tcard-t">到府寵物保母</div>
        <div class="tcard-d">主打到府服務<br>目標每月接滿 20 單</div>
      </div>
      <div class="tcard foster" id="tc-foster" onclick="selType('foster')">
        <span class="tcard-em">🐱</span>
        <div class="tcard-t">中途之家貓咪</div>
        <div class="tcard-d">待認養毛孩介紹<br>增粉互動暖帳號</div>
      </div>
    </div>
    <div class="platrow">
      <button class="pbtn active fb" id="pb-fb" onclick="selPlat('fb')">📘 Facebook</button>
      <button class="pbtn active ig" id="pb-ig" onclick="selPlat('ig')">📸 Instagram</button>
      <button class="pbtn active th" id="pb-th" onclick="selPlat('th')">🧵 Threads 脆</button>
    </div>
  </div>

  <!-- 範本列表 -->
  <div id="postList"></div>

  <div class="tip tp"><span class="tipicon">💡</span><div><strong>使用方式：</strong>點「使用這篇」貼文會出現在下方編輯區，你可以直接修改（粉色框可輸入），改完再點複製！</div></div>

  <!-- 編輯區 -->
  <div class="card" id="editArea" style="display:none">
    <div class="ch"><div class="ci cil">✏️</div><div><div class="ctitle">編輯 & 複製貼文</div><div class="csub">直接在框內修改，改好再複製！</div></div></div>
    <div class="tabrow" id="editTabs"></div>
    <textarea id="editText" rows="10" style="font-size:14px;line-height:1.9"></textarea>
    <div class="charcount" id="editCount">0 字</div>
    <div class="out-acts">
      <button class="btn bpink bsm" onclick="copyEdit()">📋 複製貼文</button>
      <button class="btn bblue bsm" onclick="copyWithTags()">📋 複製貼文＋Hashtag</button>
      <button class="btn bghost bsm" onclick="clearEdit()">🗑️ 清除</button>
    </div>
  </div>
</div>

<!-- ══════ PAGE: IDEABANK ══════ -->
<div id="pg-ideabank" class="page">
  <div class="hero">
    <div class="hero-icon">💡</div>
    <div>
      <div class="hero-title">貼文靈感庫</div>
      <div class="hero-desc">點擊靈感卡片，貼文範本馬上顯示在下方！</div>
    </div>
  </div>
  <div class="card">
    <div class="ch"><div class="ci cip">🏠</div><div><div class="ctitle">保母服務靈感 × 12</div></div></div>
    <div class="g3" id="nannyIdeas"></div>
  </div>
  <div class="card">
    <div class="ch"><div class="ci cib">🐱</div><div><div class="ctitle">中途認養靈感 × 10</div></div></div>
    <div class="g3" id="fosterIdeas"></div>
  </div>
  <div class="card" id="ideaOut" style="display:none">
    <div class="ch"><div class="ci cil">✏️</div><div><div class="ctitle">靈感範本編輯區</div></div></div>
    <div class="tabrow" id="ideaTabs"></div>
    <textarea id="ideaText" rows="10" style="font-size:14px;line-height:1.9"></textarea>
    <div class="charcount" id="ideaCount">0 字</div>
    <div class="out-acts">
      <button class="btn bpink bsm" onclick="copyIdea()">📋 複製</button>
      <button class="btn bblue bsm" onclick="copyIdeaWithTags()">📋 複製＋Hashtag</button>
    </div>
  </div>
</div>

<!-- ══════ PAGE: HASHTAGS ══════ -->
<div id="pg-hashtags" class="page">
  <div class="hero">
    <div class="hero-icon">🏷️</div>
    <div>
      <div class="hero-title">Hashtag 工具</div>
      <div class="hero-desc">勾選標籤，一鍵複製整組！</div>
    </div>
  </div>
  <div class="g2 mb16">
    <div class="card">
      <div class="ch"><div class="ci cip">🏠</div><div><div class="ctitle">保母服務標籤</div></div></div>
      <div class="tagcloud" id="nannyTags"></div>
    </div>
    <div class="card">
      <div class="ch"><div class="ci cib">🐱</div><div><div class="ctitle">中途認養標籤</div></div></div>
      <div class="tagcloud" id="fosterTags"></div>
    </div>
  </div>
  <div class="card">
    <div class="ch"><div class="ci cil">📋</div><div><div class="ctitle">已選標籤組合</div><div class="csub">IG：15–20個 ／ FB：3–5個 ／ 脆：1–3個</div></div></div>
    <div id="tagOut" style="background:var(--pink-bg);border:2px dashed var(--border);border-radius:13px;padding:15px;font-size:13px;font-weight:700;color:var(--pink2);min-height:55px;line-height:2;word-break:break-word">點擊上方標籤來組合...</div>
    <div class="flex gap8 mt12">
      <button class="btn bpink bsm" onclick="copyAllTags()">📋 複製全部</button>
      <button class="btn bblue bsm" onclick="copyIGTags()">📸 複製IG版（15個）</button>
      <button class="btn bghost bsm" onclick="clearAllTags()">🗑️ 清除</button>
    </div>
  </div>
  <div class="tip tl"><span class="tipicon">💡</span><div><strong>策略：</strong>IG 混合大量詞＋中量詞＋小眾詞效果最好 ／ FB 3–5個就夠 ／ 脆自然嵌入1–3個</div></div>
</div>

<!-- ══════ PAGE: PLANNER ══════ -->
<div id="pg-planner" class="page">
  <div class="hero"><div class="hero-icon">🗓️</div><div><div class="hero-title">週排程日曆</div><div class="hero-desc">每天早晚兩篇，保母接單＋中途貓咪同步進行！</div></div></div>
  <div class="card">
    <div class="ch"><div class="ci cip">⏰</div><div><div class="ctitle">最佳發文時間</div></div></div>
    <div class="tslot"><div class="tstime">08:00</div><div class="tsinfo"><div class="tstitle">🌅 早安貼文 — <span style="color:var(--pink2)">到府保母服務</span></div><div class="tsdesc">上班族通勤滑手機高峰 ／ 觸及廣、轉發率高</div></div><div class="tsplats"><div class="tsplat tpfb">F</div><div class="tsplat tpig">I</div><div class="tsplat tpth">脆</div></div></div>
    <div class="tslot"><div class="tstime" style="color:var(--blue2)">20:30</div><div class="tsinfo"><div class="tstitle">🌙 晚安貼文 — <span style="color:var(--blue2)">中途貓咪日常</span></div><div class="tsdesc">全天最高互動黃金時段 ／ 情感共鳴最強</div></div><div class="tsplats"><div class="tsplat tpfb">F</div><div class="tsplat tpig">I</div><div class="tsplat tpth">脆</div></div></div>
  </div>
  <div class="card">
    <div class="ch"><div class="ci cib">📆</div><div><div class="ctitle">本週貼文主題日曆</div></div></div>
    <div class="wgrid">
      <div class="dcol"><div class="dhead today">一</div><div class="dpost nanny"><div class="dpt dptn">08:00</div><div class="dptx">🏠 保母｜週一出遊計畫提醒</div></div><div class="dpost foster"><div class="dpt dptf">20:30</div><div class="dptx">🐱 中途｜本週明星貓登場！</div></div></div>
      <div class="dcol"><div class="dhead">二</div><div class="dpost nanny"><div class="dpt dptn">08:00</div><div class="dptx">🏠 保母｜客戶回饋分享</div></div><div class="dpost foster"><div class="dpt dptf">20:30</div><div class="dptx">🐱 中途｜今日萌照大公開</div></div></div>
      <div class="dcol"><div class="dhead">三</div><div class="dpost nanny"><div class="dpt dptn">08:00</div><div class="dptx">🏠 保母｜服務流程透明化</div></div><div class="dpost foster"><div class="dpt dptf">20:30</div><div class="dptx">🐱 中途｜認養資訊說明</div></div></div>
      <div class="dcol"><div class="dhead">四</div><div class="dpost nanny"><div class="dpt dptn">08:00</div><div class="dptx">🏠 保母｜熱門話題切入</div></div><div class="dpost foster"><div class="dpt dptf">20:30</div><div class="dptx">🐱 中途｜領養代替購買</div></div></div>
      <div class="dcol"><div class="dhead">五</div><div class="dpost nanny"><div class="dpt dptn">08:00</div><div class="dptx">🏠 保母｜週末預約開放</div></div><div class="dpost foster"><div class="dpt dptf">20:30</div><div class="dptx">🐱 中途｜貓咪個性介紹</div></div></div>
      <div class="dcol"><div class="dhead">六</div><div class="dpost nanny"><div class="dpt dptn">10:00</div><div class="dptx">🏠 保母｜服務實況</div></div><div class="dpost foster"><div class="dpt dptf">20:30</div><div class="dptx">🐱 中途｜週末互動</div></div></div>
      <div class="dcol"><div class="dhead">日</div><div class="dpost nanny"><div class="dpt dptn">10:00</div><div class="dptx">🏠 保母｜下週名額</div></div><div class="dpost foster"><div class="dpt dptf">20:30</div><div class="dptx">🐱 中途｜本週感謝</div></div></div>
    </div>
  </div>
  <div class="tip tp"><span class="tipicon">🎯</span><div><strong>每月20單拆解：</strong>每週5單 ＝ 每天0.7個詢問。每篇保母貼文都要有明確 CTA！</div></div>
</div>

<!-- ══════ PAGE: MONTHLY ══════ -->
<div id="pg-monthly" class="page">
  <div class="hero"><div class="hero-icon">📆</div><div><div class="hero-title">月度作戰計畫</div><div class="hero-desc">每月三階段衝刺，穩定達成20單目標！</div></div></div>
  <div class="card">
    <div class="ch"><div class="ci cip">🗓️</div><div><div class="ctitle">三階段衝刺策略</div></div></div>
    <div class="g3">
      <div style="border:2px solid var(--pink2);border-radius:15px;padding:16px;background:rgba(255,181,200,.08)">
        <div style="font-size:20px;font-weight:900;color:var(--pink2);margin-bottom:3px">1–10日</div>
        <div style="font-size:11px;font-weight:900;color:var(--pink);margin-bottom:10px;letter-spacing:.08em">🔥 衝刺開單期</div>
        <div style="font-size:12px;color:var(--text2);font-weight:600;line-height:1.8">✅ 保母貼文加倍<br>✅ 每篇強 CTA<br>✅ 推早鳥優惠<br>✅ 主動在社團發文<br>🎯 目標：拿到8–10單</div>
      </div>
      <div style="border:2px solid var(--mint2);border-radius:15px;padding:16px;background:rgba(181,234,215,.1)">
        <div style="font-size:20px;font-weight:900;color:var(--mint2);margin-bottom:3px">11–20日</div>
        <div style="font-size:11px;font-weight:900;color:var(--mint2);margin-bottom:10px;letter-spacing:.08em">🌿 維持互動期</div>
        <div style="font-size:12px;color:var(--text2);font-weight:600;line-height:1.8">✅ 保母+中途均衡<br>✅ 分享客戶見證<br>✅ 互動問答增黏著<br>✅ Reels/短影音<br>🎯 目標：再拿7–8單</div>
      </div>
      <div style="border:2px solid var(--lemon2);border-radius:15px;padding:16px;background:rgba(255,234,167,.15)">
        <div style="font-size:20px;font-weight:900;color:#c47f00;margin-bottom:3px">21–31日</div>
        <div style="font-size:11px;font-weight:900;color:var(--lemon2);margin-bottom:10px;letter-spacing:.08em">⚡ 收尾衝刺期</div>
        <div style="font-size:12px;color:var(--text2);font-weight:600;line-height:1.8">✅ 月底限時優惠<br>✅ 未達標加強保母<br>✅ 開放下月預約<br>✅ 感謝回饋文<br>🎯 目標：湊滿20單</div>
      </div>
    </div>
  </div>
  <div class="card">
    <div class="ch"><div class="ci cim">📊</div><div><div class="ctitle">每月主題規劃</div></div></div>
    <table class="mtable">
      <thead><tr><th>週次</th><th>保母主題</th><th>中途主題</th><th>特殊行動</th></tr></thead>
      <tbody>
        <tr><td><span style="color:var(--pink2);font-weight:900">第一週</span></td><td>連假預約倒數</td><td>本月明星貓介紹</td><td>📢 加入3個寵物社團</td></tr>
        <tr><td><span style="color:var(--blue2);font-weight:900">第二週</span></td><td>服務流程+收費說明</td><td>認養成功故事</td><td>🤝 與其他帳號互動</td></tr>
        <tr><td><span style="color:var(--mint2);font-weight:900">第三週</span></td><td>客戶見證回饋</td><td>貓咪萌照日常</td><td>📹 製作一支短 Reels</td></tr>
        <tr><td><span style="color:var(--lav2);font-weight:900">第四週</span></td><td>月底優惠+下月預約</td><td>本月中途成果回顧</td><td>🎉 感謝粉絲互動貼</td></tr>
      </tbody>
    </table>
  </div>
</div>

<!-- ══════ PAGE: DASHBOARD ══════ -->
<div id="pg-dashboard" class="page">
  <div class="hero"><div class="hero-icon">📈</div><div><div class="hero-title">業績看板</div><div class="hero-desc">追蹤每月接單目標進度！</div></div></div>
  <div class="g4 mb20">
    <div class="sblob sbp"><span class="sem">🎯</span><div class="snum snp">20</div><div class="slabel">本月目標單數</div><div class="ssub">每月保母接單</div></div>
    <div class="sblob sbb"><span class="sem">✅</span><div class="snum snb" id="onum">0</div><div class="slabel">本月已接單</div><div class="ssub" id="ostatus">⏳ 開始接單吧！</div></div>
    <div class="sblob sbm"><span class="sem">📱</span><div class="snum snm" id="pnum">0</div><div class="slabel">本月已發文</div><div class="ssub">目標 60 篇 / 月</div></div>
    <div class="sblob sbv"><span class="sem">💬</span><div class="snum snv" id="inum">0</div><div class="slabel">本月詢問數</div><div class="ssub">轉換率追蹤</div></div>
  </div>
  <div class="card">
    <div class="ch"><div class="ci cip">📊</div><div><div class="ctitle">進度追蹤器</div></div></div>
    <div class="pw mb16"><div class="ph"><span>🏠 保母接單目標</span><span id="opct">0 / 20 單</span></div><div class="pb"><div class="pf pfp" id="obar" style="width:0%"></div></div></div>
    <div class="pw mb16"><div class="ph"><span>📱 發文目標</span><span id="ppct">0 / 60 篇</span></div><div class="pb"><div class="pf pfb" id="pbar" style="width:0%"></div></div></div>
    <div class="pw"><div class="ph"><span>💬 詢問轉換率</span><span id="conv">0%</span></div><div class="pb"><div class="pf pfm" id="cbar" style="width:0%"></div></div></div>
    <div class="divider"></div>
    <div class="g3">
      <div class="fg"><label>✅ 更新接單數</label><div class="flex gap8 ic"><input type="number" id="inO" min="0" max="50" value="0" style="text-align:center;font-size:18px;font-weight:900;width:80px"><button class="btn bpink bsm" onclick="updateStats()">更新</button></div></div>
      <div class="fg"><label>📱 更新發文數</label><div class="flex gap8 ic"><input type="number" id="inP" min="0" max="120" value="0" style="text-align:center;font-size:18px;font-weight:900;width:80px"><button class="btn bblue bsm" onclick="updateStats()">更新</button></div></div>
      <div class="fg"><label>💬 更新詢問數</label><div class="flex gap8 ic"><input type="number" id="inI" min="0" max="100" value="0" style="text-align:center;font-size:18px;font-weight:900;width:80px"><button class="btn bmint bsm" onclick="updateStats()">更新</button></div></div>
    </div>
  </div>
  <div class="card">
    <div class="ch"><div class="ci cil">🐾</div><div><div class="ctitle">接單點點追蹤</div><div class="csub">達成一單就點一個格子！</div></div></div>
    <div class="odots" id="odots"></div>
  </div>
</div>

<!-- ══════ PAGE: CHECKLIST ══════ -->
<div id="pg-checklist" class="page">
  <div class="hero"><div class="hero-icon">✅</div><div><div class="hero-title">每日發文清單</div><div class="hero-desc">點擊打勾，今天的任務完成了嗎？</div></div></div>
  <div class="g2">
    <div class="card">
      <div class="ch"><div class="ci cip">☀️</div><div><div class="ctitle">早上任務（8:00前）</div></div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">🏠 保母貼文已發（FB）</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">📸 保母貼文已發（IG）</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">🧵 保母貼文已發（脆）</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">#️⃣ Hashtag 已加入</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">📞 CTA 已加入貼文</div></div>
    </div>
    <div class="card">
      <div class="ch"><div class="ci cib">🌙</div><div><div class="ctitle">晚上任務（20:30前）</div></div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">🐱 中途貼文已發（FB）</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">📸 中途貼文已發（IG）</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">🧵 中途貼文已發（脆）</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">💬 已回覆今日所有留言</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">💌 已回覆私訊詢問</div></div>
    </div>
    <div class="card">
      <div class="ch"><div class="ci cim">🌿</div><div><div class="ctitle">互動任務（每天）</div></div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">👍 在相關貼文留言互動 × 5</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">🤝 跟其他寵物帳號互動</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">📊 查看今日貼文數據</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">📸 拍攝明天的素材照</div></div>
    </div>
    <div class="card">
      <div class="ch"><div class="ci cil">⭐</div><div><div class="ctitle">週任務（每週）</div></div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">📹 製作 1 支 Reels / 限動</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">📢 在 3 個社團分享貼文</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">📊 分析本週數據表現</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">🗓️ 規劃下週貼文主題</div></div>
      <div class="crow" onclick="togC(this)"><div class="cbox"></div><div class="clabel">💜 感謝每一個詢問的人</div></div>
    </div>
  </div>
  <div class="flex gap8 mt12">
    <button class="btn bmint" onclick="resetCL()">🔄 重置清單</button>
  </div>
</div>

<!-- ══════ PAGE: STRATEGY ══════ -->
<div id="pg-strategy" class="page">
  <div class="hero"><div class="hero-icon">🌈</div><div><div class="hero-title">平台策略指南</div><div class="hero-desc">三平台各司其職，相輔相成達成20單！</div></div></div>
  <div class="pstrat psfb"><div class="pst">📘 Facebook — 主力接單戰場</div><ul class="psul"><li>加入「寵物版」「媽媽版」「社區版」社團定期分享服務</li><li>長文分享培養信任感，展現服務細節與照護知識</li><li>每篇保母貼文都要有明確 CTA（私訊預約 / 點連結）</li><li>鼓勵舊客戶分享、標記，增加自然觸及</li><li>開啟 Messenger 快速回覆，縮短詢問到成單時間</li><li>有限度投放廣告（預算500–1000元，鎖定5km內寵物主人）</li></ul></div>
  <div class="pstrat psig"><div class="pst">📸 Instagram — 品牌形象打造</div><ul class="psul"><li>精美毛孩照片為核心，保持視覺一致性（暖色調）</li><li>每週至少 1 支 Reels（服務日常vlog、貓咪萌片）衝免費觸及</li><li>限時動態每天更新，投票互動增加黏著度</li><li>IG 限動加入「點擊私訊」貼紙，降低詢問門檻</li><li>善用 Highlights 保存服務介紹、客戶見證、認養資訊</li></ul></div>
  <div class="pstrat psth"><div class="pst">🧵 Threads（脆）— 社群黏著增溫</div><ul class="psul"><li>輕鬆日常語氣，像朋友在說話，不要太商業</li><li>分享保母真實心情：「今天照顧的貓咪太黏人了」</li><li>熱點話題搶先回應，提升帳號曝光</li><li>貓咪幽默語錄、互動問答，增加轉發和收藏</li></ul></div>
  <div class="tip tp"><span class="tipicon">🚀</span><div><strong>衝單公式：</strong>每月60篇貼文 × 平均觸及500人 = 3萬次曝光 → 0.1%詢問率 = 30個詢問 → 70%轉換 = 21單 🎉</div></div>
</div>

<!-- ══════ PAGE: FORMULA ══════ -->
<div id="pg-formula" class="page">
  <div class="hero"><div class="hero-icon">🧪</div><div><div class="hero-title">貼文公式</div><div class="hero-desc">每一篇接單保母貼文都跟著這6步走！</div></div></div>
  <div class="card">
    <div class="ch"><div class="ci cip">🏠</div><div><div class="ctitle">保母接單 6 步公式</div></div></div>
    <div class="fstep"><div class="fnum" style="background:var(--pink2)">1</div><div><div class="ftitle">🎯 痛點開頭（前2行決定生死）</div><div class="fdesc">「要出門了，主子一個人在家，你是不是超擔心？」<br>前兩行要讓人停下手指，抓住痛點製造共鳴</div></div></div>
    <div class="fstep"><div class="fnum" style="background:var(--blue2)">2</div><div><div class="ftitle">💡 解決方案（你的服務是答案）</div><div class="fdesc">「其實你不用帶走牠！讓貓咪待在熟悉的環境，我來陪伴」<br>自然帶入服務，不要太商業，要像朋友建議</div></div></div>
    <div class="fstep"><div class="fnum" style="background:var(--mint2)">3</div><div><div class="ftitle">🤝 建立信任（讓人放心交給你）</div><div class="fdesc">分享服務細節、貓咪照片、資歷說明、照護清單<br>「每次拜訪都會傳回報照片，讓你隨時放心」</div></div></div>
    <div class="fstep"><div class="fnum" style="background:var(--lemon2)">4</div><div><div class="ftitle">⭐ 社會證明（客戶說的比你更有力）</div><div class="fdesc">引用客戶回饋、合照<br>「上個月幫20個家庭照顧毛孩，零事故100%好評」</div></div></div>
    <div class="fstep"><div class="fnum" style="background:var(--lav2)">5</div><div><div class="ftitle">⏰ 稀缺感（讓人立即行動）</div><div class="fdesc">「本月還剩3個名額」「連假前2週需要提前預約」<br>製造適度緊迫感，促進立即詢問</div></div></div>
    <div class="fstep"><div class="fnum" style="background:var(--peach2)">6</div><div><div class="ftitle">📞 明確 CTA</div><div class="fdesc">「私訊我『預約』兩個字，我馬上回覆！」<br>越具體越好，不要說「有興趣可以聯絡」</div></div></div>
  </div>
</div>

</main>
</div>

<!-- TICKER -->
<div class="ticker-bar">
  <div class="ticker-in">
    <span class="titem">🐱 貓窩社群小編系統</span><span class="titem">🎯 每月20單保母接單目標</span><span class="titem">📸 早上8:00保母貼文</span><span class="titem">🌙 晚上20:30中途貓咪貼文</span><span class="titem">🏠 到府寵物保母 #貓窩</span><span class="titem">🐾 領養代替購買</span><span class="titem">✨ FB · IG · Threads 三平台同步</span><span class="titem">💌 每篇都要有CTA！</span><span class="titem">🌸 今天也要發出漂亮的貼文</span>
    <span class="titem">🐱 貓窩社群小編系統</span><span class="titem">🎯 每月20單保母接單目標</span><span class="titem">📸 早上8:00保母貼文</span><span class="titem">🌙 晚上20:30中途貓咪貼文</span><span class="titem">🏠 到府寵物保母 #貓窩</span><span class="titem">🐾 領養代替購買</span><span class="titem">✨ FB · IG · Threads 三平台同步</span><span class="titem">💌 每篇都要有CTA！</span><span class="titem">🌸 今天也要發出漂亮的貼文</span>
  </div>
</div>

<script>
// ════ BUBBLES ════
const bc=['#FFB5C8','#A8D8EA','#B5EAD7','#FFEAA7','#C3B1E1','#FFCBA4'];
const bw=document.getElementById('bubbles');
for(let i=0;i<14;i++){const b=document.createElement('div');b.className='bubble';const s=30+Math.random()*80;b.style.cssText=`width:${s}px;height:${s}px;left:${Math.random()*100}%;background:${bc[i%6]};animation-duration:${12+Math.random()*18}s;animation-delay:${Math.random()*15}s`;bw.appendChild(b)}

// ════ DATA ════
const POSTS = {
  nanny: {
    fb: [
      {title:'出遊前焦慮解方',body:`各位貓奴朋友們，有沒有這種感覺？

訂好機票，選好飯店，行李都打包好了——
但就是沒辦法開心出門，因為心裡一直掛念著家裡的主子。😿

「牠會不會餓？」
「牠會不會一直叫？」
「萬一生病了怎麼辦？」

這些焦慮，我完全懂！

其實，貓咪最討厭環境改變，強迫牠去寵物旅館反而壓力更大。
最好的方式，就是讓牠留在熟悉的家，由專業保母來陪伴。

我是貓窩保母，每次拜訪都會：
✅ 準時餵食、換水
✅ 清理貓砂
✅ 陪玩互動至少20分鐘
✅ 每次都拍照回報給你安心

本月保母名額有限，出遊前請提早預約！
💌 私訊我「預約」兩個字，我立刻回覆你 🐱

#到府寵物保母 #貓咪保母 #出遊安心 #貓窩`},
      {title:'保母 vs 寵物旅館',body:`帶貓去寵物旅館，真的對牠好嗎？🤔

身為照顧過上百隻貓咪的保母，我想跟大家說實話——

貓咪和狗狗不一樣，牠們是非常戀家的動物。
陌生環境 + 陌生氣味 + 陌生聲音，對貓咪來說壓力超大！

很多送去旅館的貓咪回家後：
😿 好幾天躲起來不理人
😿 食慾不振、精神差
😿 腸胃敏感甚至嘔吐

到府保母的優勢：
🏠 貓咪待在熟悉的家，零壓力
📸 每次拜訪即時照片回報
❤️ 一對一專屬照顧，不用搶注意力
💰 通常比好的旅館更划算！

主子說謝謝你不帶牠去旅館喵～

本月還有幾個名額，私訊詢問 👇
#到府寵物保母 #貓咪照顧 #貓窩 #寵物保母推薦`},
      {title:'服務透明說明',body:`第一次找到府保母，不知道要問什麼？

讓我幫你整理清楚！📋

【貓窩到府保母服務內容】
🕐 每次拜訪時間：約40–60分鐘
🍽️ 餵食新鮮食物/罐頭/零食
💧 補充飲水（飲水機清洗）
🪣 清理貓砂盆
🎾 互動玩耍、梳毛
📸 每次拍照回報給飼主
🚨 緊急狀況立即通知

【常見問題 Q&A】
Q：保母會不會翻我家東西？
A：絕對不會！我只進行貓咪照護範圍的事情。

Q：需要給備用鑰匙嗎？
A：可以鑰匙交接或是密碼鎖，都ok！

Q：可以照顧幾隻貓？
A：1–4隻都沒問題 🐱

有其他問題歡迎私訊我！
本月名額倒數，別忘了提早預約 💌
#到府寵物保母 #貓窩 #寵物照護 #貓咪保母`},
      {title:'客戶回饋分享',body:`收到客戶傳來的訊息，好感動🥺

「上次出差5天，本來超擔心家裡的橘子，
結果每天都收到照片，橘子看起來超開心，
回家發現牠好像比我出門前還更胖了哈哈哈
謝謝你讓我出差完全沒有後顧之憂！」

這就是我當保母最開心的事了💛

每一位把毛孩交給我的主人，
我都把牠們當自己的孩子在照顧。

橘子，下次還歡迎你喔！🐱

想讓自己的出遊也沒有後顧之憂嗎？
💌 私訊預約，本月名額有限！

#到府寵物保母 #貓窩 #客戶回饋 #貓奴日常`},
      {title:'高齡貓照護',body:`家裡有老貓嗎？這篇很重要 👇

高齡貓咪（10歲以上）需要更細心的照護：

🩺 藥物需求：很多老貓需要每天吃藥
🍽️ 飲食特殊：可能需要處方糧或特定食材
💧 多喝水：老貓腎臟容易出問題，喝水很重要
🚶 活動力下降：需要更多溫柔的陪伴與按摩
🌡️ 保暖需求：老貓怕冷，需要舒適的環境

我有豐富的老貓照護經驗，
可以協助餵藥、特殊飲食、日常觀察等。

如果你有高齡貓咪需要特殊照護，
歡迎私訊我詳細討論需求 💌

讓老主子在家舒服度過每一天 🐱💛
#到府寵物保母 #高齡貓照護 #貓窩 #貓奴日常`},
      {title:'連假限量預約',body:`⚠️ 重要通知：連假保母名額快要滿了！

距離下個連假還有____天
目前剩餘名額：___個

每到連假，詢問量就會暴增，
每次都有主人在最後一刻才來詢問，結果名額已滿 😢

為了你和毛孩都能放假放心，
請至少提前____週預約！

【預約流程】
1️⃣ 私訊「預約+假期日期+貓咪數量」
2️⃣ 我回覆確認名額與費用
3️⃣ 約好時間先到府認識貓咪
4️⃣ 假期安心出遊！

不要讓主子等你最後才預約喔～
💌 立刻私訊預約，先到先得！

#到府寵物保母 #貓窩 #連假寵物 #寵物保母推薦`}
    ],
    ig: [
      {title:'出遊前焦慮（IG）',body:`出遊前最難的一步就是⋯⋯
踏出家門 🚪

因為有個毛茸茸的傢伙
用他的大眼睛看著你 🥺

別擔心！交給貓窩保母
我來陪你的主子度過每一天 🏠

✅ 準時餵食餵水
✅ 清理貓砂
✅ 每天照片回報
✅ 滿滿的陪伴與玩耍

本月名額有限 🌸
📩 私訊我「預約」馬上回覆

#到府寵物保母 #貓咪保母 #貓窩 #毛孩守護者 #貓奴日常 #寵物照護 #出遊安心 #貓咪在家最安心 #到府服務 #寵物保母推薦 #貓咪照顧 #連假寵物 #毛孩媽媽 #貓咪代理家長 #台北寵物保母`},
      {title:'保母日常（IG）',body:`今天的服務日記 🐾

早上8點準時到府
橘子已經在門口等我了 😂

今天特別乖，吃完飯還讓我梳毛
梳了一大把毛毛 🐱✨

主人說「牠平常很怕生的欸！」
哈哈我們已經是好朋友了

每一次拜訪都讓我充滿能量 🌸
這就是當保母最開心的事

💌 想讓你的主子也被這樣照顧嗎？
私訊我預約吧！

#到府寵物保母 #貓窩 #貓咪日常 #橘貓 #毛孩守護者 #寵物保母推薦 #貓奴日常 #貓咪照顧 #到府服務 #寵物照護 #貓咪保母 #貓咪在家最安心 #毛孩媽媽 #愛貓 #台北寵物保母`},
      {title:'服務特色（IG）',body:`你知道到府保母跟寵物旅館
差在哪裡嗎？🤔

答案是——壓力！

🏠 在家 = 零陌生環境壓力
🐱 熟悉氣味 = 貓咪安心吃飯睡覺
📸 即時照片 = 主人安心出遊

讓貓咪留在熟悉的家
才是對牠最好的選擇 ✨

本月保母名額有限
💌 私訊「預約」立刻回覆你！

#到府寵物保母 #貓窩 #貓咪保母 #毛孩守護者 #寵物照護 #貓咪在家最安心 #貓奴日常 #到府服務 #寵物保母推薦 #出遊安心 #貓咪照顧 #連假寵物 #台北寵物保母 #毛孩媽媽 #貓咪代理家長`}
    ],
    th: [
      {title:'出遊前焦慮（脆）',body:`要出門了但一直看著貓咪捨不得走

這種感覺只有貓奴懂吧 😂

解方：找一個好保母讓牠在家

我這個月還有名額
要出遊的趕快私訊我🐾

#到府寵物保母 #貓窩`},
      {title:'保母日常（脆）',body:`今天照顧的貓咪
吃完飯就跑來坐我腿上

然後在我腿上睡著了
我根本不敢動 哈哈哈

保母的日常就是這樣
被貓霸佔了也超開心的 🐱

想讓你的貓咪也被這樣寵嗎？找我！ #貓窩`},
      {title:'限量預約（脆）',body:`連假保母名額快滿了喔！

每次都有人最後一刻才來問
結果撲空超可惜的

想出遊又不想主子受委屈的
現在趕快私訊預約 💌

先到先得！ #貓窩 #到府寵物保母`}
    ]
  },
  foster: {
    fb: [
      {title:'本週明星貓',body:`🌟 本週明星貓咪登場！

大家好～我是【貓咪名字】
目前住在貓窩中途之家，在這裡等待一個永遠的家 🏠

【我的基本資料】
🐱 品種：米克斯（混血可愛款）
📅 年齡：約＿歲
⚖️ 體重：約＿公斤
💉 健康：已施打疫苗、已結紮、已驅蟲

【我的個性】
（請填入貓咪個性描述）

我在中途家庭生活得很好，
已經學會用貓砂盆，也不怕人抱～

如果你覺得和我有緣，
歡迎私訊貓窩詢問認養！
讓我們一起找到屬於我的家 💛

認養前會進行訪談，確保大家都幸福 🤝

#貓咪認養 #領養代替購買 #中途之家 #待認養貓咪 #貓窩`},
      {title:'貓咪蛻變故事',body:`有些故事，讓我相信世界是美好的 🌈

【名字】的故事

（請填入貓咪的救援/中途故事）

從當時的模樣，到現在的牠——
真的判若兩貓。

看著牠現在在家裡打滾撒嬌，
我才覺得那些奔波、心疼、熬夜照顧
全部都值得了。

現在牠準備好了，
準備好去尋找一個永遠愛牠的家。

如果你也被這樣的眼神打動，
歡迎私訊詢問認養🥺

轉發讓更多人看到牠好嗎？感謝你 🙏

#領養代替購買 #貓咪認養 #中途之家 #浪浪需要家 #貓窩`},
      {title:'領養代替購買',body:`如果你正在考慮養貓，
我想在你做決定前說幾句話。

台灣每年有數萬隻流浪貓在等待一個家。
牠們不是因為不好，
而是因為命運，來到了街頭、收容所、或中途之家。

領養一隻中途貓咪，你得到的是：
🐱 一個已經健檢、結紮、驅蟲的健康貓咪
❤️ 一隻知道自己被拯救、格外懂得感恩的夥伴
🌈 改變一條生命的成就感

我們目前有幾隻個性超好的貓咪等待認養，
牠們已經在中途家庭生活，了解基本生活習慣。

想認識牠們嗎？私訊我🐾

#領養代替購買 #貓咪認養 #中途之家 #貓窩 #待認養貓咪`},
      {title:'認養成功慶祝',body:`🎉 好消息！【貓咪名字】找到家了！

感謝新家庭的選擇，也謝謝每一位分享、關心牠的人 💛

老實說，每次送出一隻貓咪，
心裡都有點不捨，
但更多的是滿滿的幸福感。

看著牠走進新家，新主人眼神裡的愛，
我就知道牠找到對的地方了。

貓窩還有幾隻可愛的毛孩等待認養，
如果你也想給一個孩子一個家，
歡迎私訊我們 🐾

轉發讓更多毛孩被看見，謝謝你！🙏

#領養代替購買 #貓咪認養 #中途之家 #貓窩 #認養成功`},
      {title:'黑貓迷思破解',body:`黑貓，真的會帶來不好的事嗎？

身為中途媽媽，我要說——
這是最大的誤解！🖤

認識幾個關於黑貓的事實：

❤️ 黑色素讓黑貓的毛色特別柔亮，摸起來超舒服
😻 研究顯示黑貓個性普遍穩定、親人
🧬 黑色素基因甚至讓牠們對某些疾病有更強抵抗力
🐱 黑貓的眼睛，在光線下閃閃發光，美極了

但是——
黑貓的認養率，
是所有顏色貓咪裡最低的 😢

我們現在有幾隻超可愛的黑貓等待認養
真的超級黏人、超愛撒嬌

給牠們一個機會，好嗎？
私訊我了解認養資訊 🖤

#黑貓 #領養代替購買 #貓咪認養 #貓窩 #中途之家`}
    ],
    ig: [
      {title:'明星貓（IG）',body:`✨ 本週的主角是⋯⋯

【貓咪名字】！🐱

（請填入貓咪簡短介紹）

牠喜歡⋯⋯
牠不喜歡⋯⋯
牠最愛的事是⋯⋯

如果覺得和牠有緣 💛
私訊我們詢問認養吧！

#貓咪認養 #領養代替購買 #中途之家 #貓窩 #待認養貓咪 #可愛貓咪 #貓咪日常 #愛貓人士 #浪浪需要家 #中途媽媽 #每隻都值得愛 #台灣中途 #貓咪送養 #毛孩送養 #救援貓咪`},
      {title:'中途日常（IG）',body:`中途媽媽的日常 🌸

今天的【貓咪名字】特別調皮
把玩具全部叼到被窩裡藏起來 😂

搗蛋歸搗蛋
但這樣充滿生命力的眼神
讓我覺得一切都值得了 🐾

牠現在正在等待一個永遠的家
喜歡牠的歡迎私訊我們 💌

#貓窩 #中途之家 #領養代替購買 #貓咪認養 #貓咪日常 #可愛貓咪 #愛貓人士 #待認養貓咪 #中途媽媽 #浪浪需要家 #毛孩送養 #救援貓咪 #每隻都值得愛 #台灣中途 #貓咪的家`},
      {title:'黑貓（IG）',body:`黑色，是最美的顏色 🖤

眼睛一睜開
琥珀色的眼珠在黑夜裡閃閃發光

牠叫【名字】
目前在貓窩中途等待認養

個性超級黏人
就是喜歡趴在人身上睡覺那種 😂

認養率最低的黑貓
其實是最值得被愛的那個

有緣的你，私訊我們 💌🖤

#黑貓 #貓咪認養 #領養代替購買 #貓窩 #中途之家 #待認養貓咪 #可愛貓咪 #愛貓人士 #中途媽媽 #浪浪需要家 #台灣中途 #貓咪送養 #每隻都值得愛 #毛孩送養 #貓咪的家`}
    ],
    th: [
      {title:'明星貓（脆）',body:`本週中途的【名字】
真的是天使轉世

每次我進門牠就衝過來踩我腳
然後開始喵喵叫要抱抱

這種生物為什麼那麼可愛啊 🥺

牠現在在等一個家
有想認養的私訊我 #貓窩`},
      {title:'認養心情（脆）',body:`今天【名字】被認養走了 🎉

送走的時候捨不得哭
但看到新主人抱著牠眼裡發光

就知道這是最好的結局了

謝謝每一個分享幫忙讓更多人看到牠的人 💛

貓窩還有幾個孩子等待，歡迎來認識 #領養代替購買`},
      {title:'中途日常（脆）',body:`中途媽媽的真實日記：

早上6點被踩臉叫起床餵食
收拾完貓砂去上班
下班衝回家陪牠玩
洗澡前先被搶睡

然後看著牠睡著的臉
覺得這一切都超值得的

這就是養貓 哈哈 #貓窩 #中途之家`}
    ]
  }
};

const NANNY_TAGS = ['#到府寵物保母','#貓咪保母','#貓窩','#寵物照護','#毛孩守護者','#出遊安心託付','#台北寵物保母','#貓奴日常','#到府服務','#寵物保母推薦','#貓咪在家最安心','#貓咪照顧','#連假寵物','#寵物代理家長','#毛孩媽媽'];
const FOSTER_TAGS = ['#貓咪認養','#領養代替購買','#中途之家','#待認養貓咪','#浪浪需要家','#貓咪送養','#毛孩送養','#救援貓咪','#中途媽媽','#可愛貓咪','#貓咪日常','#愛貓人士','#每隻都值得愛','#台灣中途'];

const NANNY_IDEAS = [
  {em:'✈️',t:'出遊前焦慮大解密',d:'主人出門前的擔心，告訴他們答案'},
  {em:'📸',t:'服務實況日誌',d:'用真實照片記錄一天的照顧過程'},
  {em:'🆚',t:'保母 vs 旅館比較',d:'用故事說服主人選擇到府服務'},
  {em:'👴',t:'高齡貓照護專題',d:'針對有老貓的主人，打造專業形象'},
  {em:'😿',t:'分離焦慮解方',d:'熱門搜尋話題，自然帶入服務'},
  {em:'🔥',t:'限量名額緊迫貼',d:'製造稀缺感，刺激立即詢問'},
  {em:'💬',t:'客戶見證分享',d:'社會證明最有說服力'},
  {em:'🌡️',t:'換季照護知識',d:'帶有用資訊，展現專業知識'},
  {em:'📋',t:'服務流程透明化',d:'消除新客戶疑慮，降低詢問門檻'},
  {em:'🐈‍⬛',t:'多貓家庭專門',d:'瞄準多貓主人這個利基市場'},
  {em:'🗓️',t:'保母一日日誌',d:'貼近真實生活感，增加親切度'},
  {em:'💜',t:'保母的初心故事',d:'品牌故事最能拉近距離建立信任'}
];
const FOSTER_IDEAS = [
  {em:'⭐',t:'週一明星貓登場',d:'固定欄目讓粉絲每週期待'},
  {em:'🌈',t:'貓咪蛻變故事',d:'最高互動的情感共鳴內容'},
  {em:'💬',t:'認養前必看貼',d:'詳細介紹貓咪個性，匹配適合主人'},
  {em:'🖤',t:'黑貓迷思破解',d:'黑貓認養率最低，用知識打破偏見'},
  {em:'👵',t:'老貓認養推廣',d:'感人內容，讓人想認養資深主子'},
  {em:'🫣',t:'膽小貓咪的美好',d:'幫害羞貓咪找到有耐心的主人'},
  {em:'📋',t:'認養準備清單',d:'有用資訊提高收藏分享率'},
  {em:'🏠',t:'領養代替購買',d:'理念分享，吸引認同價值觀的粉絲'},
  {em:'📸',t:'中途日常萌照',d:'最高互動，讓粉絲每週期待'},
  {em:'🎉',t:'認養成功慶祝帖',d:'最溫暖的內容，激勵更多人分享'}
];

// ════ STATE ════
let curType='nanny', curPlat='fb';
let selTags=new Set(), curIdeaData={};

// ════ INIT ════
window.onload = function(){
  genBubbles();
  renderPosts();
  renderIdeas();
  renderTags();
  genOrderDots();
};

function genBubbles(){
  // already done above
}

// ════ NAV ════
function nav(el,page){
  document.querySelectorAll('.nitem').forEach(n=>n.classList.remove('active'));
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  el.classList.add('active');
  document.getElementById('pg-'+page).classList.add('active');
}

// ════ TYPE / PLAT ════
function selType(t){
  curType=t;
  document.getElementById('tc-nanny').className='tcard nanny'+(t==='nanny'?' sel':'');
  document.getElementById('tc-foster').className='tcard foster'+(t==='foster'?' sel':'');
  renderPosts();
}
function selPlat(p){
  curPlat=p;
  ['fb','ig','th'].forEach(x=>{
    document.getElementById('pb-'+x).className='pbtn'+(x===p?' active '+x:'');
  });
  renderPosts();
}

// ════ RENDER POSTS ════
function renderPosts(){
  const list=document.getElementById('postList');
  const data=POSTS[curType][curPlat]||[];
  if(!data.length){list.innerHTML='<div class="tip tb2"><span class="tipicon">💡</span><div>目前此分類貼文整理中，請切換其他平台！</div></div>';return;}
  list.innerHTML=data.map((p,i)=>`
    <div class="card" style="border-left:4px solid ${curType==='nanny'?'var(--pink2)':'var(--blue2)'}">
      <div class="ch"><div class="ci ${curType==='nanny'?'cip':'cib'}">${curType==='nanny'?'🏠':'🐱'}</div><div><div class="ctitle">${p.title}</div><div class="csub">${curPlat.toUpperCase()} · ${p.body.length}字</div></div><button class="btn bpink bxs" style="margin-left:auto" onclick="usePost(${i})">使用這篇 →</button></div>
      <div style="font-size:12px;color:var(--text2);font-weight:600;line-height:1.7;white-space:pre-wrap;max-height:80px;overflow:hidden;mask-image:linear-gradient(180deg,#000 60%,transparent)">${p.body}</div>
    </div>`).join('');
}

function usePost(i){
  const p=POSTS[curType][curPlat][i];
  const ea=document.getElementById('editArea');
  ea.style.display='block';
  document.getElementById('editTabs').innerHTML=`<div class="tabi active">${curPlat.toUpperCase()} 版本</div>`;
  const ta=document.getElementById('editText');
  ta.value=p.body;
  updateCount('editText','editCount');
  ea.scrollIntoView({behavior:'smooth',block:'start'});
}
function updateCount(tid,cid){
  const t=document.getElementById(tid);
  const c=document.getElementById(cid);
  t.addEventListener('input',()=>c.textContent=t.value.length+' 字');
  c.textContent=t.value.length+' 字';
}
function copyEdit(){
  const t=document.getElementById('editText').value;
  navigator.clipboard.writeText(t).then(()=>showToast('✅ 貼文已複製！'));
}
function copyWithTags(){
  const t=document.getElementById('editText').value;
  const tags=[...(curType==='nanny'?NANNY_TAGS:FOSTER_TAGS)].slice(0,curPlat==='fb'?5:curPlat==='th'?2:15).join(' ');
  navigator.clipboard.writeText(t+'\n\n'+tags).then(()=>showToast('✅ 貼文＋Hashtag 已複製！'));
}
function clearEdit(){
  document.getElementById('editText').value='';
  document.getElementById('editCount').textContent='0 字';
  document.getElementById('editArea').style.display='none';
}

// ════ IDEAS ════
function renderIdeas(){
  document.getElementById('nannyIdeas').innerHTML=NANNY_IDEAS.map((d,i)=>`
    <div class="icard" onclick="useIdea('nanny',${i})">
      <div class="ibadge ibn">保母</div>
      <div class="iem">${d.em}</div>
      <div class="it">${d.t}</div>
      <div class="id">${d.d}</div>
    </div>`).join('');
  document.getElementById('fosterIdeas').innerHTML=FOSTER_IDEAS.map((d,i)=>`
    <div class="icard" onclick="useIdea('foster',${i})">
      <div class="ibadge ibf">中途</div>
      <div class="iem">${d.em}</div>
      <div class="it">${d.t}</div>
      <div class="id">${d.d}</div>
    </div>`).join('');
}
function useIdea(type,i){
  const idea=type==='nanny'?NANNY_IDEAS[i]:FOSTER_IDEAS[i];
  const posts=POSTS[type];
  const platforms=['fb','ig','th'];
  curIdeaData={};
  // Find matching posts or generate template
  platforms.forEach(p=>{
    const arr=posts[p]||[];
    const match=arr.find(x=>x.title.includes(idea.t.slice(0,4)))||arr[0];
    curIdeaData[p]=match?match.body:`【${p.toUpperCase()}版】\n\n請根據「${idea.t}」話題，參考以下重點撰寫：\n\n${idea.d}\n\n（請修改為你自己的內容）\n\n#貓窩 ${type==='nanny'?'#到府寵物保母':'#貓咪認養'}`;
  });
  const out=document.getElementById('ideaOut');
  out.style.display='block';
  document.getElementById('ideaTabs').innerHTML=platforms.map((p,idx)=>`
    <div class="tabi${idx===0?' active':''}" onclick="switchIdeaTab('${p}',this)">${p.toUpperCase()}</div>`).join('');
  const ta=document.getElementById('ideaText');
  ta.value=curIdeaData['fb'];
  updateCount('ideaText','ideaCount');
  out.scrollIntoView({behavior:'smooth',block:'start'});
}
function switchIdeaTab(p,el){
  document.querySelectorAll('#ideaTabs .tabi').forEach(t=>t.classList.remove('active'));
  el.classList.add('active');
  document.getElementById('ideaText').value=curIdeaData[p]||'';
  document.getElementById('ideaCount').textContent=(curIdeaData[p]||'').length+' 字';
}
function copyIdea(){
  navigator.clipboard.writeText(document.getElementById('ideaText').value).then(()=>showToast('✅ 已複製！'));
}
function copyIdeaWithTags(){
  const t=document.getElementById('ideaText').value;
  const tags=NANNY_TAGS.slice(0,8).join(' ');
  navigator.clipboard.writeText(t+'\n\n'+tags).then(()=>showToast('✅ 貼文＋Hashtag 已複製！'));
}

// ════ HASHTAGS ════
function renderTags(){
  const nc=document.getElementById('nannyTags');
  const fc=document.getElementById('fosterTags');
  nc.innerHTML=NANNY_TAGS.map(t=>`<div class="tchip${selTags.has(t)?' sel':''}" onclick="togTag(this,'${t}')">${t}</div>`).join('');
  fc.innerHTML=FOSTER_TAGS.map(t=>`<div class="tchip foster${selTags.has(t)?' sel':''}" onclick="togTag(this,'${t}',true)">${t}</div>`).join('');
}
function togTag(el,tag,foster=false){
  if(el.classList.contains('sel')){el.classList.remove('sel');selTags.delete(tag);}
  else{el.classList.add('sel');selTags.add(tag);}
  updateTagOut();
}
function updateTagOut(){
  const el=document.getElementById('tagOut');
  if(!selTags.size){el.textContent='點擊上方標籤來組合...';return;}
  el.textContent=[...selTags].join(' ');
}
function copyAllTags(){
  if(!selTags.size)return;
  navigator.clipboard.writeText([...selTags].join(' ')).then(()=>showToast('✅ 標籤已複製！'));
}
function copyIGTags(){
  const tags=[...selTags].slice(0,15).join(' ');
  navigator.clipboard.writeText(tags).then(()=>showToast('✅ IG標籤（15個）已複製！'));
}
function clearAllTags(){
  selTags.clear();
  renderTags();
  document.getElementById('tagOut').textContent='點擊上方標籤來組合...';
}

// ════ STATS ════
function updateStats(){
  const o=+document.getElementById('inO').value||0;
  const p=+document.getElementById('inP').value||0;
  const inq=+document.getElementById('inI').value||0;
  document.getElementById('onum').textContent=o;
  document.getElementById('pnum').textContent=p;
  document.getElementById('inum').textContent=inq;
  document.getElementById('opct').textContent=`${o} / 20 單`;
  document.getElementById('ppct').textContent=`${p} / 60 篇`;
  const cv=inq>0?Math.round((o/inq)*100):0;
  document.getElementById('conv').textContent=cv+'%';
  document.getElementById('obar').style.width=Math.min((o/20)*100,100)+'%';
  document.getElementById('pbar').style.width=Math.min((p/60)*100,100)+'%';
  document.getElementById('cbar').style.width=Math.min(cv,100)+'%';
  document.getElementById('ostatus').textContent=o>=20?'🎉 已達標！恭喜！':o>=10?'💪 過半了，加油！':`⏳ 還差 ${20-o} 單`;
  document.querySelectorAll('.odot').forEach((d,i)=>d.classList.toggle('done',i<o));
}
function genOrderDots(){
  const el=document.getElementById('odots');
  for(let i=1;i<=20;i++){const d=document.createElement('div');d.className='odot';d.textContent=i;d.onclick=()=>d.classList.toggle('done');el.appendChild(d);}
}

// ════ CHECKLIST ════
function togC(el){
  el.classList.toggle('done');
  el.querySelector('.cbox').textContent=el.classList.contains('done')?'✓':'';
}
function resetCL(){
  document.querySelectorAll('.crow').forEach(r=>{r.classList.remove('done');r.querySelector('.cbox').textContent='';});
  showToast('🔄 清單已重置！');
}

// ════ TOAST ════
function showToast(msg){
  const t=document.getElementById('toast');
  t.textContent=msg||'✅ 已複製！';
  t.classList.add('show');
  setTimeout(()=>t.classList.remove('show'),2200);
}
</script>
</body>
</html>

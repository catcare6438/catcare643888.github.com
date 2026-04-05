<!DOCTYPE html>
<html lang="zh-TW">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>🐾 貓窩社群小編 ✨</title>
<link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800;900&family=Noto+Sans+TC:wght@400;500;700;900&display=swap" rel="stylesheet">
<style>
:root {
  --pink:    #FFB5C8;
  --pink2:   #FF8FAB;
  --pink-bg: #FFF0F4;
  --blue:    #A8D8EA;
  --blue2:   #7EC8E3;
  --blue-bg: #EEF8FC;
  --mint:    #B5EAD7;
  --mint2:   #7DDBB0;
  --lemon:   #FFEAA7;
  --lemon2:  #FFD93D;
  --lavender:#C3B1E1;
  --lav2:    #A084CA;
  --peach:   #FFCBA4;
  --peach2:  #FFB07C;
  --white:   #FFFFFF;
  --cream:   #FFFDF9;
  --text:    #5D4E75;
  --text2:   #8B7BA8;
  --text3:   #B3A5C8;
  --border:  #EDD9F0;
  --shadow:  rgba(180,140,220,0.15);
  --shadow2: rgba(255,182,200,0.25);
}

* { box-sizing: border-box; margin: 0; padding: 0; }

html { scroll-behavior: smooth; }

body {
  background: var(--cream);
  color: var(--text);
  font-family: 'Nunito', 'Noto Sans TC', sans-serif;
  min-height: 100vh;
  overflow-x: hidden;
  cursor: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24'%3E%3Ctext y='20' font-size='18'%3E🐾%3C/text%3E%3C/svg%3E") 4 4, auto;
}

/* Dreamy background */
body::before {
  content: '';
  position: fixed;
  inset: 0;
  background:
    radial-gradient(ellipse 80% 60% at 10% 0%, rgba(255,181,200,0.18) 0%, transparent 60%),
    radial-gradient(ellipse 60% 50% at 90% 0%, rgba(168,216,234,0.18) 0%, transparent 60%),
    radial-gradient(ellipse 50% 40% at 50% 100%, rgba(181,234,215,0.15) 0%, transparent 60%),
    var(--cream);
  pointer-events: none;
  z-index: 0;
}

/* Floating bubbles deco */
.bubbles {
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 0;
  overflow: hidden;
}
.bubble {
  position: absolute;
  border-radius: 50%;
  opacity: 0.25;
  animation: floatBubble linear infinite;
}
@keyframes floatBubble {
  0% { transform: translateY(110vh) scale(0.5); opacity: 0; }
  10% { opacity: 0.25; }
  90% { opacity: 0.25; }
  100% { transform: translateY(-10vh) scale(1.2); opacity: 0; }
}

/* ────── HEADER ────── */
header {
  position: sticky; top: 0; z-index: 200;
  background: rgba(255,255,255,0.85);
  backdrop-filter: blur(16px);
  border-bottom: 2px dashed var(--border);
  padding: 0 28px;
  height: 68px;
  display: flex; align-items: center; justify-content: space-between;
}

.logo {
  display: flex; align-items: center; gap: 12px;
}
.logo-blob {
  width: 44px; height: 44px;
  background: linear-gradient(135deg, var(--pink), var(--blue));
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
  display: flex; align-items: center; justify-content: center;
  font-size: 22px;
  box-shadow: 0 4px 12px var(--shadow2);
  animation: blobPulse 3s ease-in-out infinite;
}
@keyframes blobPulse {
  0%,100% { border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%; }
  50% { border-radius: 60% 40% 60% 40% / 40% 60% 40% 60%; }
}
.logo-name {
  font-size: 20px; font-weight: 900;
  background: linear-gradient(135deg, var(--pink2), var(--lav2));
  -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  letter-spacing: 0.03em;
}
.logo-en {
  font-size: 10px; color: var(--text3); font-weight: 700; letter-spacing: 0.12em;
}

.header-pills { display: flex; gap: 8px; align-items: center; }

.pill {
  padding: 6px 14px; border-radius: 20px;
  font-size: 12px; font-weight: 800;
  border: none; cursor: pointer;
  transition: all 0.2s; white-space: nowrap;
}
.pill-pink { background: var(--pink); color: white; }
.pill-blue { background: var(--blue2); color: white; }
.pill-pink:hover, .pill-blue:hover { transform: translateY(-2px); box-shadow: 0 4px 12px var(--shadow2); }

/* ────── LAYOUT ────── */
.layout {
  display: grid;
  grid-template-columns: 250px 1fr;
  min-height: calc(100vh - 68px);
  position: relative; z-index: 1;
}

/* ────── SIDEBAR ────── */
.sidebar {
  background: rgba(255,255,255,0.7);
  backdrop-filter: blur(12px);
  border-right: 2px dashed var(--border);
  padding: 24px 16px;
  display: flex; flex-direction: column; gap: 4px;
  position: sticky; top: 68px; height: calc(100vh - 68px);
  overflow-y: auto;
}

.sidebar-cat-deco {
  text-align: center; padding: 12px 0 20px;
  border-bottom: 2px dashed var(--border);
  margin-bottom: 16px;
}
.sidebar-cat-deco .cat-svg { font-size: 48px; animation: catSway 4s ease-in-out infinite; display: inline-block; }
@keyframes catSway {
  0%,100% { transform: rotate(-5deg); }
  50% { transform: rotate(5deg); }
}
.sidebar-cat-deco p { font-size: 11px; color: var(--text3); font-weight: 700; margin-top: 4px; }

.nav-section-title {
  font-size: 10px; font-weight: 800; letter-spacing: 0.12em;
  color: var(--text3); padding: 12px 10px 4px;
  text-transform: uppercase;
}

.nav-item {
  display: flex; align-items: center; gap: 10px;
  padding: 10px 12px; border-radius: 14px;
  cursor: pointer; font-size: 13px; font-weight: 700;
  color: var(--text2); transition: all 0.2s;
  border: 2px solid transparent;
  position: relative;
}
.nav-item:hover { background: var(--pink-bg); color: var(--pink2); }
.nav-item.active { background: linear-gradient(135deg, var(--pink-bg), var(--blue-bg)); border-color: var(--pink); color: var(--pink2); }
.nav-item .nav-emoji { font-size: 18px; }
.nav-badge {
  position: absolute; right: 10px; top: 50%; transform: translateY(-50%);
  background: var(--pink2); color: white;
  font-size: 9px; font-weight: 900; padding: 2px 6px; border-radius: 10px;
}

/* ────── CONTENT ────── */
.content {
  padding: 28px 32px 80px;
  overflow-y: auto;
}

.page { display: none; animation: pageIn 0.3s ease; }
.page.active { display: block; }
@keyframes pageIn {
  from { opacity: 0; transform: translateY(12px); }
  to { opacity: 1; transform: translateY(0); }
}

/* ────── PAGE HEADER ────── */
.page-hero {
  display: flex; align-items: flex-start; gap: 20px;
  margin-bottom: 28px; padding: 24px 28px;
  background: white; border-radius: 24px;
  border: 2px solid var(--border);
  box-shadow: 0 6px 24px var(--shadow);
  position: relative; overflow: hidden;
}
.page-hero::after {
  content: '';
  position: absolute; right: -20px; top: -20px;
  width: 120px; height: 120px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--pink), var(--lemon));
  opacity: 0.12;
}
.page-hero-icon {
  font-size: 52px; line-height: 1;
  filter: drop-shadow(0 4px 8px rgba(255,100,100,0.2));
  flex-shrink: 0;
}
.page-hero-title { font-size: 26px; font-weight: 900; color: var(--text); margin-bottom: 4px; }
.page-hero-desc { font-size: 13px; color: var(--text2); line-height: 1.7; font-weight: 600; }

/* ────── CARDS ────── */
.card {
  background: white; border-radius: 20px;
  border: 2px solid var(--border);
  padding: 22px 24px; margin-bottom: 18px;
  box-shadow: 0 4px 16px var(--shadow);
  transition: box-shadow 0.2s;
}
.card:hover { box-shadow: 0 8px 28px var(--shadow2); }

.card-head {
  display: flex; align-items: center; gap: 10px;
  margin-bottom: 18px;
}
.card-icon {
  width: 36px; height: 36px; border-radius: 12px;
  display: flex; align-items: center; justify-content: center;
  font-size: 18px; flex-shrink: 0;
}
.ci-pink { background: var(--pink-bg); }
.ci-blue { background: var(--blue-bg); }
.ci-mint { background: rgba(181,234,215,0.25); }
.ci-lemon { background: rgba(255,234,167,0.3); }
.ci-lav { background: rgba(195,177,225,0.2); }

.card-title { font-size: 14px; font-weight: 900; color: var(--text); }
.card-subtitle { font-size: 11px; color: var(--text3); font-weight: 600; }

/* ────── GRID ────── */
.g2 { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
.g3 { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 14px; }
.g4 { display: grid; grid-template-columns: repeat(4,1fr); gap: 12px; }

/* ────── BUTTONS ────── */
.btn {
  display: inline-flex; align-items: center; gap: 7px;
  padding: 10px 20px; border-radius: 50px;
  font-size: 13px; font-weight: 800; font-family: inherit;
  cursor: pointer; border: none; transition: all 0.2s;
  letter-spacing: 0.02em;
}
.btn:active { transform: scale(0.96); }
.btn-pink {
  background: linear-gradient(135deg, var(--pink2), #ff6b9d);
  color: white; box-shadow: 0 4px 14px rgba(255,100,150,0.35);
}
.btn-pink:hover { transform: translateY(-2px); box-shadow: 0 6px 20px rgba(255,100,150,0.45); }
.btn-pink:disabled { opacity: 0.55; pointer-events: none; }
.btn-blue {
  background: linear-gradient(135deg, var(--blue2), #5bb8d4);
  color: white; box-shadow: 0 4px 14px rgba(100,180,220,0.35);
}
.btn-blue:hover { transform: translateY(-2px); }
.btn-mint {
  background: linear-gradient(135deg, var(--mint2), #5dc99a);
  color: white; box-shadow: 0 4px 14px rgba(100,200,160,0.35);
}
.btn-mint:hover { transform: translateY(-2px); }
.btn-ghost {
  background: white; color: var(--text2);
  border: 2px solid var(--border); box-shadow: none;
}
.btn-ghost:hover { border-color: var(--pink); color: var(--pink2); }
.btn-lemon {
  background: linear-gradient(135deg, var(--lemon2), #ffa500);
  color: white; box-shadow: 0 4px 14px rgba(255,200,50,0.35);
}
.btn-sm { padding: 7px 14px; font-size: 12px; }
.btn-xs { padding: 5px 10px; font-size: 11px; }

/* ────── FORM CONTROLS ────── */
.form-group { margin-bottom: 16px; }
label {
  display: block; font-size: 12px; font-weight: 800;
  color: var(--text2); margin-bottom: 6px; letter-spacing: 0.05em;
}
.label-icon { margin-right: 4px; }

input[type=text], input[type=number], textarea, select {
  width: 100%;
  background: var(--pink-bg);
  border: 2px solid var(--border);
  border-radius: 14px;
  padding: 10px 14px;
  color: var(--text);
  font-family: inherit; font-size: 13px; font-weight: 600;
  outline: none; transition: all 0.2s;
  -webkit-appearance: none;
}
input:focus, textarea:focus, select:focus {
  border-color: var(--pink); background: white;
  box-shadow: 0 0 0 4px rgba(255,143,171,0.12);
}
textarea { resize: vertical; line-height: 1.7; }
select { cursor: pointer; }

.input-row { display: flex; gap: 10px; align-items: flex-end; }

/* ────── TYPE SELECTOR ────── */
.type-cards { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; margin-bottom: 20px; }

.type-card {
  border: 3px solid var(--border);
  border-radius: 20px; padding: 18px;
  cursor: pointer; transition: all 0.25s;
  text-align: center; background: white;
  position: relative; overflow: hidden;
}
.type-card::before {
  content: '';
  position: absolute; inset: 0;
  opacity: 0; transition: opacity 0.25s;
}
.type-card.nanny::before { background: linear-gradient(135deg, rgba(255,181,200,0.15), rgba(255,206,164,0.15)); }
.type-card.foster::before { background: linear-gradient(135deg, rgba(168,216,234,0.15), rgba(181,234,215,0.15)); }
.type-card.selected, .type-card:hover { transform: translateY(-3px); box-shadow: 0 8px 24px var(--shadow2); }
.type-card.selected::before { opacity: 1; }
.type-card.nanny.selected { border-color: var(--pink2); }
.type-card.foster.selected { border-color: var(--blue2); }
.type-card-emoji { font-size: 36px; margin-bottom: 10px; display: block; }
.type-card-title { font-size: 14px; font-weight: 900; color: var(--text); margin-bottom: 4px; }
.type-card-desc { font-size: 11px; color: var(--text2); font-weight: 600; line-height: 1.5; }
.type-card-badge {
  position: absolute; top: 10px; right: 10px;
  background: var(--pink); color: white;
  font-size: 9px; font-weight: 900; padding: 3px 7px; border-radius: 10px;
}

/* ────── PLATFORM PILLS ────── */
.platform-row { display: flex; gap: 8px; flex-wrap: wrap; margin-bottom: 18px; }
.plat-btn {
  padding: 8px 16px; border-radius: 50px;
  font-size: 12px; font-weight: 800; font-family: inherit;
  cursor: pointer; border: 2px solid var(--border);
  background: white; color: var(--text3);
  transition: all 0.2s; display: flex; align-items: center; gap: 6px;
}
.plat-btn:hover { border-color: var(--pink); color: var(--pink2); }
.plat-btn.active.fb { background: #1877f2; border-color: #1877f2; color: white; }
.plat-btn.active.ig { background: linear-gradient(135deg,#f09433,#e6683c,#dc2743,#cc2366,#bc1888); border-color: #dc2743; color: white; }
.plat-btn.active.th { background: #111; border-color: #111; color: white; }
.plat-btn.active.all { background: linear-gradient(135deg, var(--pink2), var(--blue2)); border-color: var(--pink2); color: white; }

/* ────── OUTPUT ────── */
.output-wrap {
  border: 3px dashed var(--border); border-radius: 20px;
  padding: 22px; min-height: 140px;
  background: linear-gradient(135deg, var(--pink-bg), var(--blue-bg));
  font-size: 14px; line-height: 1.9; font-weight: 600;
  white-space: pre-wrap; word-break: break-word;
  position: relative; transition: all 0.3s;
}
.output-wrap.loading {
  display: flex; align-items: center; justify-content: center;
  flex-direction: column; gap: 12px;
  color: var(--text3); font-size: 13px;
}
.output-actions {
  display: flex; gap: 8px; margin-top: 12px; flex-wrap: wrap;
}

/* ────── TABS ────── */
.tab-row {
  display: flex; gap: 0; margin-bottom: 16px;
  background: var(--pink-bg); border-radius: 16px; padding: 4px;
  border: 2px solid var(--border);
}
.tab-item {
  flex: 1; text-align: center;
  padding: 8px 12px; border-radius: 12px;
  font-size: 12px; font-weight: 800; cursor: pointer;
  color: var(--text3); transition: all 0.2s;
}
.tab-item.active {
  background: white; color: var(--pink2);
  box-shadow: 0 2px 8px var(--shadow);
}

/* ────── TOPICS ────── */
.topic-item {
  display: flex; align-items: center; gap: 12px;
  padding: 12px 14px; border-radius: 14px;
  border: 2px solid var(--border); margin-bottom: 8px;
  cursor: pointer; background: white; transition: all 0.2s;
}
.topic-item:hover, .topic-item.selected {
  border-color: var(--pink); background: var(--pink-bg);
  transform: translateX(4px);
}
.topic-item.foster:hover, .topic-item.foster.selected {
  border-color: var(--blue2); background: var(--blue-bg);
}
.topic-dot { width: 10px; height: 10px; border-radius: 50%; flex-shrink: 0; }
.td-pink { background: var(--pink2); }
.td-blue { background: var(--blue2); }
.topic-text { font-size: 13px; font-weight: 700; flex: 1; color: var(--text); }
.topic-badge {
  font-size: 10px; font-weight: 800; padding: 3px 9px; border-radius: 10px;
}
.tb-hot { background: rgba(255,143,171,0.2); color: var(--pink2); }
.tb-trend { background: rgba(126,200,163,0.2); color: var(--mint2); }
.tb-new { background: rgba(168,216,234,0.25); color: var(--blue2); }
.tb-season { background: rgba(255,234,167,0.4); color: #c47f00; }

/* ────── STATS ────── */
.stat-blob {
  background: white; border-radius: 20px;
  border: 2px solid var(--border);
  padding: 20px; text-align: center;
  box-shadow: 0 4px 16px var(--shadow);
  position: relative; overflow: hidden;
  transition: transform 0.2s;
}
.stat-blob:hover { transform: translateY(-3px); }
.stat-blob::before {
  content: '';
  position: absolute; inset: -1px;
  border-radius: 20px; opacity: 0.12;
  z-index: 0;
}
.stat-blob.pink::before { background: linear-gradient(135deg, var(--pink), var(--lemon)); }
.stat-blob.blue::before { background: linear-gradient(135deg, var(--blue), var(--mint)); }
.stat-blob.mint::before { background: linear-gradient(135deg, var(--mint), var(--lemon)); }
.stat-blob.lav::before { background: linear-gradient(135deg, var(--lavender), var(--blue)); }
.stat-blob > * { position: relative; z-index: 1; }
.stat-emoji { font-size: 28px; margin-bottom: 8px; display: block; }
.stat-num { font-size: 36px; font-weight: 900; line-height: 1; margin-bottom: 4px; }
.stat-num.pink { color: var(--pink2); }
.stat-num.blue { color: var(--blue2); }
.stat-num.mint { color: var(--mint2); }
.stat-num.lav { color: var(--lav2); }
.stat-label { font-size: 12px; font-weight: 800; color: var(--text2); }
.stat-sub { font-size: 11px; color: var(--text3); margin-top: 3px; font-weight: 600; }

/* ────── PROGRESS ────── */
.progress-wrap { margin: 8px 0; }
.progress-header { display: flex; justify-content: space-between; font-size: 12px; font-weight: 800; color: var(--text2); margin-bottom: 6px; }
.progress-bar { height: 10px; background: var(--pink-bg); border-radius: 10px; overflow: hidden; border: 1px solid var(--border); }
.progress-fill { height: 100%; border-radius: 10px; transition: width 0.8s cubic-bezier(.17,.67,.35,1.1); }
.pf-pink { background: linear-gradient(90deg, var(--pink), var(--pink2)); }
.pf-blue { background: linear-gradient(90deg, var(--blue), var(--blue2)); }
.pf-mint { background: linear-gradient(90deg, var(--mint), var(--mint2)); }

/* ────── WEEK PLANNER ────── */
.week-grid { display: grid; grid-template-columns: repeat(7,1fr); gap: 6px; margin-top: 14px; }
.day-col { display: flex; flex-direction: column; gap: 6px; }
.day-head { text-align: center; font-size: 11px; font-weight: 900; color: var(--text3); padding: 8px 4px; background: var(--pink-bg); border-radius: 10px; }
.day-head.today { background: linear-gradient(135deg, var(--pink), var(--blue)); color: white; }
.day-post {
  background: white; border: 2px solid var(--border); border-radius: 12px;
  padding: 8px 7px; font-size: 10px; font-weight: 700;
  cursor: pointer; transition: all 0.2s;
  line-height: 1.4;
}
.day-post:hover { transform: scale(1.04); box-shadow: 0 4px 10px var(--shadow2); }
.day-post.nanny { border-left: 4px solid var(--pink2); }
.day-post.foster { border-left: 4px solid var(--blue2); }
.dp-time { font-size: 10px; font-weight: 900; margin-bottom: 3px; }
.dp-time.nanny { color: var(--pink2); }
.dp-time.foster { color: var(--blue2); }
.dp-text { color: var(--text2); font-size: 10px; }

/* ────── HASHTAG CHIPS ────── */
.tag-cloud { display: flex; flex-wrap: wrap; gap: 7px; }
.tag-chip {
  padding: 5px 12px; border-radius: 50px;
  font-size: 12px; font-weight: 800; font-family: inherit;
  cursor: pointer; border: 2px solid var(--border);
  background: white; color: var(--text2);
  transition: all 0.18s;
}
.tag-chip:hover { border-color: var(--pink); color: var(--pink2); }
.tag-chip.selected { background: var(--pink); border-color: var(--pink); color: white; box-shadow: 0 3px 10px var(--shadow2); }
.tag-chip.foster.selected { background: var(--blue2); border-color: var(--blue2); }

/* ────── ALERT BOXES ────── */
.tip-box {
  border-radius: 16px; padding: 14px 18px;
  font-size: 13px; font-weight: 700; line-height: 1.7;
  margin-bottom: 14px; display: flex; gap: 12px; align-items: flex-start;
}
.tip-box .tip-icon { font-size: 22px; flex-shrink: 0; margin-top: 1px; }
.tip-pink { background: rgba(255,181,200,0.2); border: 2px solid rgba(255,143,171,0.35); color: var(--text); }
.tip-blue { background: rgba(168,216,234,0.2); border: 2px solid rgba(126,200,227,0.35); color: var(--text); }
.tip-mint { background: rgba(181,234,215,0.25); border: 2px solid rgba(125,219,176,0.4); color: var(--text); }
.tip-lemon { background: rgba(255,234,167,0.3); border: 2px solid rgba(255,217,61,0.35); color: var(--text); }

/* ────── TIME SLOTS ────── */
.time-slot {
  display: flex; align-items: center; gap: 16px;
  padding: 16px 18px; border-radius: 16px;
  border: 2px solid var(--border); margin-bottom: 10px;
  background: white; transition: all 0.2s;
}
.time-slot:hover { border-color: var(--pink); box-shadow: 0 4px 16px var(--shadow2); }
.ts-time { font-size: 26px; font-weight: 900; color: var(--pink2); min-width: 75px; line-height: 1; }
.ts-info { flex: 1; }
.ts-title { font-size: 13px; font-weight: 800; color: var(--text); margin-bottom: 4px; }
.ts-desc { font-size: 11px; color: var(--text3); font-weight: 600; line-height: 1.5; }
.ts-plats { display: flex; gap: 5px; }
.ts-plat {
  width: 26px; height: 26px; border-radius: 8px;
  display: flex; align-items: center; justify-content: center;
  font-size: 11px; font-weight: 900; color: white;
}
.tsp-fb { background: #1877f2; }
.tsp-ig { background: linear-gradient(135deg,#f09433,#dc2743); }
.tsp-th { background: #333; }

/* ────── CTA FORMULA ────── */
.formula-step {
  display: flex; align-items: flex-start;

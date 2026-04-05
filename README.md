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
select { cursor: poin
/* 接續你原本中斷的 select 樣式 */
select {
    cursor: pointer;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 24 24' fill='none' stroke='%238B7BA8' stroke-width='3' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m6 9 6 6 6-6'/%3E%3C/svg%3E");
    background-repeat: no-repeat;
    background-position: right 12px center;
    padding-right: 36px;
}

/* 數據卡片樣式 */
.stat-box {
    background: white;
    padding: 16px;
    border-radius: 18px;
    border: 2px solid var(--border);
    text-align: center;
    transition: transform 0.2s;
}
.stat-box:hover { transform: translateY(-5px); }
.stat-val { font-size: 22px; font-weight: 900; color: var(--pink2); }
.stat-label { font-size: 11px; color: var(--text3); font-weight: 700; margin-top: 4px; }

/* 貼文預覽區 */
.preview-container {
    background: var(--blue-bg);
    border-radius: 20px;
    border: 2px dashed var(--blue2);
    padding: 20px;
    min-height: 200px;
    font-size: 14px;
    line-height: 1.6;
    color: var(--text);
    white-space: pre-wrap;
}

/* 自定義捲軸 */
::-webkit-scrollbar { width: 8px; }
::-webkit-scrollbar-track { background: transparent; }
::-webkit-scrollbar-thumb { background: var(--border); border-radius: 10px; }
::-webkit-scrollbar-thumb:hover { background: var(--pink); }

/* 響應式微調 */
@media (max-width: 850px) {
    .layout { grid-template-columns: 1fr; }
    .sidebar { display: none; }
}
</style>
</head>
<body>

<div class="bubbles" id="bubble-container"></div>

<header>
    <div class="logo">
        <div class="logo-blob">🐾</div>
        <div>
            <div class="logo-name">貓窩 NEKO HUB</div>
            <div class="logo-en">COMMUNITY MANAGER</div>
        </div>
    </div>
    <div class="header-pills">
        <button class="pill pill-pink">喵喵模式 ON</button>
        <button class="pill pill-blue">管理員：小花</button>
    </div>
</header>

<div class="layout">
    <aside class="sidebar">
        <div class="sidebar-cat-deco">
            <span class="cat-svg">🐱</span>
            <p>今日貓氣值：100%</p>
        </div>
        
        <div class="nav-section-title">主要選單</div>
        <div class="nav-item active" onclick="showPage('dashboard', this)">
            <span class="nav-emoji">🏠</span> 總覽面板
        </div>
        <div class="nav-item" onclick="showPage('composer', this)">
            <span class="nav-emoji">✍️</span> 貼文靈感
            <span class="nav-badge">NEW</span>
        </div>
        <div class="nav-item">
            <span class="nav-emoji">📈</span> 數據分析
        </div>
        
        <div class="nav-section-title" style="margin-top:20px;">工具箱</div>
        <div class="nav-item">
            <span class="nav-emoji">🖼️</span> 圖片生成
        </div>
        <div class="nav-item">
            <span class="nav-emoji">⚙️</span> 系統設定
        </div>
    </aside>

    <main class="content">
        <section id="dashboard" class="page active">
            <div class="page-hero">
                <div class="page-hero-icon">🌤️</div>
                <div>
                    <h2 class="page-hero-title">早安，社群小編！</h2>
                    <p class="page-hero-desc">今天又是充滿肉球香氣的一天。目前有 3 則預約貼文待發佈，粉絲互動率比昨日增長了 12% 喔！</p>
                </div>
            </div>

            <div class="g4">
                <div class="stat-box"><div class="stat-val">1,284</div><div class="stat-label">追蹤人數</div></div>
                <div class="stat-box"><div class="stat-val">85%</div><div class="stat-label">平均互動</div></div>
                <div class="stat-box"><div class="stat-val">12</div><div class="stat-label">本月貼文</div></div>
                <div class="stat-box"><div class="stat-val">5</div><div class="stat-label">待辦任務</div></div>
            </div>
        </section>

        <section id="composer" class="page">
            <div class="page-hero">
                <div class="page-hero-icon">✨</div>
                <div>
                    <h2 class="page-hero-title">文案靈感發射器</h2>
                    <p class="page-hero-desc">輸入關鍵字，讓貓窩 AI 幫你寫出最吸睛的社群內容。</p>
                </div>
            </div>

            <div class="g2">
                <div class="card">
                    <div class="card-head">
                        <div class="card-icon ci-pink">📝</div>
                        <div>
                            <div class="card-title">編輯內容</div>
                            <div class="card-subtitle">Editor</div>
                        </div>
                    </div>
                    <div class="form-group">
                        <label><span class="label-icon">🏷️</span>主題標籤</label>
                        <input type="text" id="topic-input" placeholder="例如：肉泥特價、主子日常...">
                    </div>
                    <div class="form-group">
                        <label><span class="label-icon">🎭</span>語氣選擇</label>
                        <select id="tone-select">
                            <option value="cute">軟萌喵喵語 (ΦωΦ)</option>
                            <option value="cool">傲嬌主子風 (￣^￣)</option>
                            <option value="pro">專業貓奴報告</option>
                        </select>
                    </div>
                    <button class="btn btn-pink" style="width: 100%; justify-content: center;" onclick="generateText()">
                        生成文案 ✨
                    </button>
                </div>

                <div class="card">
                    <div class="card-head">
                        <div class="card-icon ci-blue">👁️</div>
                        <div>
                            <div class="card-title">內容預覽</div>
                            <div class="card-subtitle">Preview</div>
                        </div>
                    </div>
                    <div class="preview-container" id="preview-box">
                        文案會在這裡出現喵...
                    </div>
                </div>
            </div>
        </section>
    </main>
</div>

<script>
// 1. 生成動態背景泡泡
function createBubbles() {
    const container = document.getElementById('bubble-container');
    const colors = ['#FFB5C8', '#A8D8EA', '#B5EAD7', '#FFEAA7'];
    
    for (let i = 0; i < 15; i++) {
        const bubble = document.createElement('div');
        bubble.className = 'bubble';
        
        const size = Math.random() * 60 + 20 + 'px';
        bubble.style.width = size;
        bubble.style.height = size;
        bubble.style.left = Math.random() * 100 + 'vw';
        bubble.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
        bubble.style.animationDuration = Math.random() * 10 + 5 + 's';
        bubble.style.animationDelay = Math.random() * 5 + 's';
        
        container.appendChild(bubble);
    }
}

// 2. 頁面切換邏輯
function showPage(pageId, element) {
    // 隱藏所有頁面
    document.querySelectorAll('.page').forEach(page => page.classList.remove('active'));
    // 顯示目標頁面
    document.getElementById(pageId).classList.add('active');
    
    // 更新側邊欄樣式
    document.querySelectorAll('.nav-item').forEach(item => item.classList.remove('active'));
    element.classList.add('active');
}

// 3. 模擬文案生成
function generateText() {
    const topic = document.getElementById('topic-input').value || '好吃的罐罐';
    const tone = document.getElementById('tone-select').value;
    const preview = document.getElementById('preview-box');
    
    preview.innerText = "正在呼喚靈感貓神...🐾";
    
    setTimeout(() => {
        let content = "";
        if(tone === 'cute') {
            content = `喵嗚～各位人類注意！\n今天的【${topic}】超級誘人喵～🐾\n快點過來看看，不然朕要生氣囉！(っ●ω●)っ`;
        } else if(tone === 'cool') {
            content = `哼，聽說你們在找【${topic}】？\n朕剛好心情好，就給你們這群奴才瞧瞧。\n還不快按讚分享？(✧≖‿ゝ≖)`;
        } else {
            content = `【社群公告：關於${topic}的深度解析】\n經過專業肉球鑑定，本次內容互動率預計提升 200%。\n建議發佈時間：奴才餵飯前一小時。`;
        }
        preview.innerText = content;
    }, 800);
}

// 初始化
window.onload = createBubbles;
</script>

</body>
</html>

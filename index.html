<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>毛毛執事排班 App</title>
    <style>
        /* 直接內建 CSS，防止讀取失敗 */
        body { background-color: #fff9f2; font-family: sans-serif; color: #5d4037; padding: 20px; display: flex; flex-direction: column; align-items: center; }
        .card { background: white; border: 3px solid #ffcfdf; border-radius: 20px; padding: 20px; width: 100%; max-width: 350px; box-shadow: 5px 5px 0px #ffcfdf; margin-bottom: 20px; }
        .btn { background: #ff8fab; color: white; border: none; padding: 10px 20px; border-radius: 50px; cursor: pointer; display: block; margin: 10px auto; font-weight: bold; }
        .day-grid { display: grid; grid-template-columns: repeat(7, 1fr); gap: 5px; background: white; padding: 10px; border-radius: 15px; border: 1px solid #ffcfdf; width: 100%; max-width: 350px; }
        .day { aspect-ratio: 1; display: flex; flex-direction: column; align-items: center; justify-content: center; font-size: 12px; border-radius: 5px; cursor: pointer; }
        .today { background: #ff8fab !important; color: white !important; }
        .icons { font-size: 10px; }
    </style>
</head>
<body>

    <div class="card">
        <h2 id="date-title" style="text-align:center; color:#ff8fab;">載入中...</h2>
        <button class="btn" onclick="loadData()">🔄 點我同步班表</button>
        <div id="my-info" style="background:#fdf2f5; padding:10px; border-radius:10px;">
            <b>我的班表：</b><span id="me">讀取中...</span>
        </div>
        <div style="margin-top:10px;">
            <b>今日其他人：</b><ul id="others" style="font-size:14px; padding-left:20px;"></ul>
        </div>
    </div>

    <div class="day-grid" id="grid"></div>

    <script>
        // 🚨 請把下面這一行換成你剛剛複製的 CSV 連結 🚨
        const myCsv = "https://docs.google.com/spreadsheets/d/e/2PACX-1vTEm.../pub?output=csv"; 
        
        async function loadData() {
            document.getElementById('date-title').innerText = "同步中...";
            try {
                const res = await fetch(myCsv + "&t=" + Date.now());
                const csv = await res.text();
                const lines = csv.split('\n').map(row => row.split(','));
                
                let data = {};
                lines.slice(1).forEach(cols => {
                    const d = cols[0]?.trim();
                    if(d) {
                        if(!data[d]) data[d] = [];
                        data[d].push({ name: cols[1]?.trim(), start: cols[2], end: cols[3] });
                    }
                });

                render(data);
            } catch (e) {
                alert("抓不到資料，請檢查 CSV 連結是否正確發布！");
            }
        }

        function render(data) {
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('date-title').innerText = today;
            
            // 顯示今日
            const list = data[today] || [];
            const me = list.find(s => s.name === "球球" || s.name === "你");
            document.getElementById('me').innerText = me ? `${me.start}-${me.end}` : "休假 🎉";
            document.getElementById('others').innerHTML = list.filter(s => s.name!=="球球" && s.name!=="你").map(s => `<li>${s.name}: ${s.start}-${s.end}</li>`).join('') || "無";

            // 生成日曆
            const grid = document.getElementById('grid');
            grid.innerHTML = "";
            for(let i=1; i<=31; i++) {
                const dayStr = `2026-03-${String(i).padStart(2, '0')}`; // 這裡先固定3月測試
                const dayData = data[dayStr] || [];
                const hasMe = dayData.some(s => s.name==="球球" || s.name==="你");
                const hasAny = dayData.length > 0;

                const el = document.createElement('div');
                el.className = 'day' + (dayStr === today ? ' today' : '');
                
                let icon = "";
                if(hasMe) icon += "🐱";
                if(hasAny) icon += "🔸";
                if(!hasAny) icon += "🎉";
                
                el.innerHTML = `<span>${i}</span><div class="icons">${icon}</div>`;
                grid.appendChild(el);
            }
        }
        window.onload = loadData;
    </script>
</body>
</html>

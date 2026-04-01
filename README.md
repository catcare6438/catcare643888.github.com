<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>球球班表</title>
    <style>
        /* --- 可愛插畫風格 CSS --- */
        body {
            background-color: #fff9f2;
            font-family: "PingFang TC", "Microsoft JhengHei", sans-serif;
            color: #5d4037;
            margin: 0;
            padding: 15px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .today-card {
            background: #ffffff;
            border: 3px solid #ffcfdf;
            border-radius: 20px;
            padding: 20px;
            width: 90%;
            max-width: 400px;
            box-shadow: 5px 5px 0px #ffcfdf;
            margin-bottom: 20px;
            position: relative;
        }

        .today-card::before {
            content: "📌";
            position: absolute;
            top: -15px;
            left: 45%;
            font-size: 24px;
        }

        h2 { color: #ff8fab; text-align: center; margin-top: 10px; }

        .sync-button {
            background: #ff8fab;
            color: white;
            border: none;
            padding: 8px 20px;
            border-radius: 50px;
            font-weight: bold;
            cursor: pointer;
            box-shadow: 0 4px 0 #fb6f92;
            display: block;
            margin: 10px auto;
        }

        .sync-button:active { transform: translateY(4px); box-shadow: none; }

        .shift-group {
            background: #fdf2f5;
            padding: 12px;
            border-radius: 15px;
            margin-bottom: 10px;
            border-left: 5px solid #ffc2d1;
        }

        ul { list-style: none; padding: 0; margin: 0; }
        li { padding: 5px 0; border-bottom: 1px dashed #eee; font-size: 14px; }

        /* 日曆區塊 */
        #calendar-container {
            background: white;
            border-radius: 20px;
            padding: 15px;
            width: 90%;
            max-width: 400px;
            border: 2px solid #ffcfdf;
        }

        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 5px;
        }

        .day {
            aspect-ratio: 1/1.2;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border-radius: 10px;
            font-size: 14px;
            cursor: pointer;
            position: relative;
        }

        .today { background-color: #ff8fab !important; color: white !important; font-weight: bold; }

        .icon-wrap { font-size: 12px; margin-top: 2px; }

        /* 彈窗樣式 */
        .modal {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.5);
            z-index: 100;
        }
        .modal-content {
            background: white;
            margin: 20% auto;
            padding: 20px;
            width: 80%;
            border-radius: 20px;
            border: 3px solid #ffcfdf;
        }
    </style>
</head>
<body>

    <div class="today-card">
        <h2 id="display-today-date">讀取中...</h2>
        <button class="sync-button" onclick="fetchSchedule()">🔄 立即同步</button>
        <p id="sync-status" style="text-align:center; font-size:12px; color:gray;">等待同步...</p>
        
        <div class="shift-group">
            <strong>我的班表：</strong>
            <span id="my-shift-time">--:--</span>
        </div>

        <div class="shift-group">
            <strong>其他人上班：</strong>
            <ul id="others-list"></ul>
        </div>
    </div>

    <div id="calendar-container">
        <div class="calendar-grid" id="calendar-grid">
            </div>
    </div>

    <div id="schedule-modal" class="modal" onclick="this.style.display='none'">
        <div class="modal-content" onclick="event.stopPropagation()">
            <h3 id="modal-date" style="color:#ff8fab"></h3>
            <div id="modal-list"></div>
            <button class="sync-button" onclick="document.getElementById('schedule-modal').style.display='none'">關閉</button>
        </div>
    </div>

    <script>
        // --- 核心邏輯 ---
        const CSV_URL = '你的Google試算表CSV連結'; // <--- 請換成你的 CSV 連結
        let scheduleData = {};
        const myName = "球球"; // <--- 檢查你的名字在 CSV 裡怎麼寫

        async function fetchSchedule() {
            const status = document.getElementById('sync-status');
            status.innerText = "同步中...";
            try {
                const response = await fetch(`${CSV_URL}&t=${new Date().getTime()}`);
                const text = await response.text();
                const rows = text.split('\n').slice(1);
                
                scheduleData = {};
                rows.forEach(row => {
                    const [date, name, start, end, note] = row.split(',').map(s => s?.trim());
                    if (date) {
                        if (!scheduleData[date]) scheduleData[date] = [];
                        scheduleData[date].push({ name, start, end, note });
                    }
                });

                document.getElementById('sync-status').innerText = "最後同步: " + new Date().toLocaleTimeString();
                renderAll();
            } catch (e) {
                status.innerText = "同步失敗，請檢查網路";
            }
        }

        function renderAll() {
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('display-today-date').innerText = today;

            // 渲染 Today 區塊
            const todayList = scheduleData[today] || [];
            const myShift = todayList.find(s => s.name === myName);
            document.getElementById('my-shift-time').innerText = myShift ? `${myShift.start} - ${myShift.end}` : "今日休假 🎉";

            const others = todayList.filter(s => s.name !== myName);
            document.getElementById('others-list').innerHTML = others.map(s => `<li><b>${s.name}</b>: ${s.start}-${s.end}</li>`).join('') || "<li>暫無行程</li>";

            // 渲染日曆
            const grid = document.getElementById('calendar-grid');
            grid.innerHTML = "";
            const now = new Date();
            const daysInMonth = new Date(now.getFullYear(), now.getMonth() + 1, 0).getDate();

            for (let i = 1; i <= daysInMonth; i++) {
                const dateStr = `${now.getFullYear()}-${String(now.getMonth() + 1).padStart(2, '0')}-${String(i).padStart(2, '0')}`;
                const dayEl = document.createElement('div');
                dayEl.className = 'day' + (dateStr === today ? ' today' : '');
                
                const data = scheduleData[dateStr] || [];
                const hasMyShift = data.some(s => s.name === myName);
                const hasAny = data.length > 0;

                let icons = "";
                if (hasMyShift) icons += "🐱";
                if (hasAny) icons += "🔸";
                if (!hasAny) icons += "🎉";

                dayEl.innerHTML = `<span>${i}</span><div class="icon-wrap">${icons}</div>`;
                dayEl.onclick = () => showModal(dateStr, data);
                grid.appendChild(dayEl);
            }
        }

        function showModal(date, data) {
            const modal = document.getElementById('schedule-modal');
            document.getElementById('modal-date').innerText = date;
            document.getElementById('modal-list').innerHTML = data.map(s => `<p><b>${s.name}</b>: ${s.start}-${s.end} ${s.note || ''}</p>`).join('') || "全體放假";
            modal.style.display = 'block';
        }

        window.onload = fetchSchedule;
    </script>
</body>
</html>

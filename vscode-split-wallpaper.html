<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VSCode代码+时钟动态壁纸</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #1e1e1e;
            color: #d4d4d4;
            font-family: 'Consolas', 'Monaco', 'Lucida Console', monospace;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0;
            overflow: hidden;
            user-select: none;
            transition: background-color 0.5s, color 0.5s;
        }

        /* 浅色主题样式 */
        body.light-theme {
            background-color: #ffffff;
            color: #1e1e1e;
        }

        body.light-theme .code-block {
            background-color: #ffffff;
            border-left: 3px solid #0078d4;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
        }

        body.light-theme .json-key {
            color: #0000ff;
        }

        body.light-theme .json-value-number {
            color: #098658;
        }

        body.light-theme .json-value-string {
            color: #a31515;
        }

        body.light-theme .json-bracket,
        body.light-theme .json-colon,
        body.light-theme .json-comma {
            color: #1e1e1e;
        }

        body.light-theme .cursor {
            background-color: #1e1e1e;
        }

        body.light-theme .line-number {
            color: #6e7681;
        }

        body.light-theme .analog-clock {
            border: 3px solid #d1d5da;
            background-color: #ffffff;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
        }

        body.light-theme .clock-center {
            background-color: #0078d4;
        }

        body.light-theme .hour-hand,
        body.light-theme .minute-hand {
            background-color: #1e1e1e;
        }

        body.light-theme .second-hand {
            background-color: #d73a49;
        }

        body.light-theme .marker {
            background-color: #6e7681;
        }

        /* 左侧代码区域 */
        .code-container {
            margin-right: 100px;
            font-size: 24px;
            line-height: 1.6;
        }

        .code-block {
            background-color: #1e1e1e;
            padding: 20px;
            border-left: 3px solid #007acc;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
        }

        .line-number {
            color: #858585;
            margin-right: 20px;
            user-select: none;
        }

        .json-key {
            color: #9cdcfe;
            font-weight: normal;
        }

        .json-value-number {
            color: #b5cea8;
        }

        .json-value-string {
            color: #ce9178;
        }

        .json-bracket {
            color: #d4d4d4;
        }

        .json-colon {
            color: #d4d4d4;
        }

        .json-comma {
            color: #d4d4d4;
        }

        .cursor {
            display: inline-block;
            width: 2px;
            height: 1.2em;
            background-color: #d4d4d4;
            animation: blink 1s infinite;
            vertical-align: text-bottom;
            margin-left: 2px;
        }

        /* 右侧圆形时钟 */
        .clock-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .analog-clock {
            width: 200px;
            height: 200px;
            border: 3px solid #3e3e42;
            border-radius: 50%;
            position: relative;
            background-color: #1e1e1e;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
        }

        .clock-center {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 12px;
            height: 12px;
            background-color: #569cd6;
            border-radius: 50%;
            transform: translate(-50%, -50%);
            z-index: 10;
        }

        .hour-hand, .minute-hand, .second-hand {
            position: absolute;
            top: 50%;
            left: 50%;
            transform-origin: 0% 50%;
            background-color: #d4d4d4;
            border-radius: 2px;
        }

        .hour-hand {
            width: 60px;
            height: 4px;
            transform: translate(0%, -50%) rotate(0deg);
        }

        .minute-hand {
            width: 80px;
            height: 2px;
            transform: translate(0%, -50%) rotate(0deg);
        }

        .second-hand {
            width: 90px;
            height: 1px;
            background-color: #ff6b6b;
            transform: translate(0%, -50%) rotate(0deg);
        }

        .clock-markers {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        .marker {
            position: absolute;
            width: 2px;
            height: 10px;
            background-color: #858585;
            top: 5px;
            left: 50%;
            transform-origin: center 95px;
        }

        .marker:nth-child(1) { transform: translateX(-50%) rotate(0deg); }
        .marker:nth-child(2) { transform: translateX(-50%) rotate(30deg); }
        .marker:nth-child(3) { transform: translateX(-50%) rotate(60deg); }
        .marker:nth-child(4) { transform: translateX(-50%) rotate(90deg); }
        .marker:nth-child(5) { transform: translateX(-50%) rotate(120deg); }
        .marker:nth-child(6) { transform: translateX(-50%) rotate(150deg); }
        .marker:nth-child(7) { transform: translateX(-50%) rotate(180deg); }
        .marker:nth-child(8) { transform: translateX(-50%) rotate(210deg); }
        .marker:nth-child(9) { transform: translateX(-50%) rotate(240deg); }
        .marker:nth-child(10) { transform: translateX(-50%) rotate(270deg); }
        .marker:nth-child(11) { transform: translateX(-50%) rotate(300deg); }
        .marker:nth-child(12) { transform: translateX(-50%) rotate(330deg); }

        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0; }
        }

        /* 主题切换开关 */
        .theme-switch {
            position: absolute;
            top: 28px;
            right: 28px;
            display: flex;
            align-items: center;
            gap: 14px;
        }

        .theme-switch input[type="checkbox"] {
            appearance: none;
            width: 60px;
            height: 30px;
            background: #569cd6;
            border-radius: 15px;
            position: relative;
            cursor: pointer;
            transition: background 0.3s;
        }

        .theme-switch input[type="checkbox"]::before {
            content: '🌙';
            position: absolute;
            width: 26px;
            height: 26px;
            background: #1e1e1e;
            border-radius: 50%;
            top: 2px;
            left: 2px;
            transition: transform 0.3s, content 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 14px;
        }

        .theme-switch input[type="checkbox"]:checked::before {
            content: '☀️';
            transform: translateX(30px);
            background: #f0f0f0;
        }

        .theme-switch input[type="checkbox"]:checked {
            background: #ffa500;
        }

        /* 响应式设计 */
        @media (max-width: 768px) {
            body {
                flex-direction: column;
                padding-left: 0;
                justify-content: center;
            }
            .code-container {
                margin-right: 0;
                margin-bottom: 40px;
            }
        }
    </style>
</head>
<body>
    <!-- 左侧代码区域 -->
    <div class="code-container">
        <div class="code-block">
            <div>
                <span class="json-key">const</span> <span class="json-key">currentTime</span> <span class="json-colon">=</span> <span class="json-bracket">{</span>
            </div>
            <div>
                    <span class="json-key">year</span><span class="json-colon">:</span> <span class="json-value-number" id="year">2025</span><span class="json-comma">,</span>
            </div>
            <div>
                    <span class="json-key">month</span><span class="json-colon">:</span> <span class="json-value-number" id="month">07</span><span class="json-comma">,</span>
            </div>
            <div>
                    <span class="json-key">day</span><span class="json-colon">:</span> <span class="json-value-number" id="day">22</span><span class="json-comma">,</span>
            </div>
            <div>
                    <span class="json-key">dayOfWeek</span><span class="json-colon">:</span> <span class="json-value-string" id="weekday">"Tuesday"</span><span class="json-comma">,</span>
            </div>
            <div>
                    <span class="json-key">hour</span><span class="json-colon">:</span> <span class="json-value-number" id="hours">16</span><span class="json-comma">,</span>
            </div>
            <div>
                    <span class="json-key">minute</span><span class="json-colon">:</span> <span class="json-value-number" id="minutes">25</span><span class="json-comma">,</span>
            </div>
            <div>
                    <span class="json-key">second</span><span class="json-colon">:</span> <span class="json-value-number" id="seconds">35</span><span class="json-comma">,</span>
            </div>
            <div>
                    <span class="json-key">dayProgress</span><span class="json-colon">:</span> <span class="json-value-number" id="dayProgress">68.44%</span>
            </div>
            <div>
                <span class="json-bracket">};</span><span class="cursor"></span>
            </div>
        </div>
    </div>

    <!-- 右侧圆形时钟 -->
    <div class="clock-container">
        <div class="analog-clock">
            <div class="clock-markers">
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
                <div class="marker"></div>
            </div>
            <div class="hour-hand" id="hourHand"></div>
            <div class="minute-hand" id="minuteHand"></div>
            <div class="second-hand" id="secondHand"></div>
            <div class="clock-center"></div>
        </div>
    </div>

    <!-- 主题切换开关 -->
    <div class="theme-switch">
        <input type="checkbox" id="theme-toggle" onclick="toggleTheme()">
    </div>

    <script>
        function updateCodeClock() {
            const now = new Date();
            
            // 获取时间
            const hours = String(now.getHours()).padStart(2, '0');
            const minutes = String(now.getMinutes()).padStart(2, '0');
            const seconds = String(now.getSeconds()).padStart(2, '0');
            
            // 获取日期
            const year = now.getFullYear();
            const month = String(now.getMonth() + 1).padStart(2, '0');
            const day = String(now.getDate()).padStart(2, '0');
            
            // 获取星期
            const weekdays = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
            const weekday = weekdays[now.getDay()];
            
            // 计算一天的进度百分比
            const totalSecondsInDay = 24 * 60 * 60;
            const currentSecondsInDay = now.getHours() * 3600 + now.getMinutes() * 60 + now.getSeconds();
            const dayProgress = ((currentSecondsInDay / totalSecondsInDay) * 100).toFixed(2);
            
            // 更新JSON显示
            document.getElementById('hours').textContent = hours;
            document.getElementById('minutes').textContent = minutes;
            document.getElementById('seconds').textContent = seconds;
            document.getElementById('year').textContent = year;
            document.getElementById('month').textContent = month;
            document.getElementById('day').textContent = day;
            document.getElementById('weekday').textContent = `"${weekday}"`;
            document.getElementById('dayProgress').textContent = `${dayProgress}%`;
            
            // 更新圆形时钟
            const hourDeg = (now.getHours() % 12) * 30 + now.getMinutes() * 0.5;
            const minuteDeg = now.getMinutes() * 6;
            const secondDeg = now.getSeconds() * 6;
            
            document.getElementById('hourHand').style.transform = 
                `translate(0%, -50%) rotate(${hourDeg - 90}deg)`;
            document.getElementById('minuteHand').style.transform = 
                `translate(0%, -50%) rotate(${minuteDeg - 90}deg)`;
            document.getElementById('secondHand').style.transform = 
                `translate(0%, -50%) rotate(${secondDeg - 90}deg)`;
        }

        // 初始化
        updateCodeClock();
        
        // 每秒更新一次
        setInterval(updateCodeClock, 1000);

        // 防止右键菜单
        document.addEventListener('contextmenu', function(e) {
            e.preventDefault();
        });

        // 主题切换功能
        function toggleTheme() {
            const body = document.body;
            body.classList.toggle('light-theme');
        }

        // 防止F12开发者工具
        document.addEventListener('keydown', function(e) {
            if (e.key === 'F12' || (e.ctrlKey && e.shiftKey && e.key === 'I')) {
                e.preventDefault();
            }
        });
    </script>
</body>
</html>

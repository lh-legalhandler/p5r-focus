<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <title>P5R风格专注 · AI智能NPC · 学习助手</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            user-select: none;
        }

        body {
            background: radial-gradient(circle at 20% 30%, #0a0a0a, #000000);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Segoe UI', 'Poppins', system-ui, sans-serif;
            padding: 20px;
        }

        .game-container {
            width: 1400px;
            max-width: 98vw;
            background: #1a1a1c;
            border: 2px solid #e33b3b;
            box-shadow: 0 0 0 4px #000, 0 0 0 8px #e33b3b, 0 20px 40px rgba(0,0,0,0.6);
            position: relative;
            overflow: hidden;
        }

        .game-container::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 120px;
            height: 120px;
            background: linear-gradient(135deg, #e33b3b 0%, #e33b3b 50%, transparent 50%);
            z-index: 1;
            pointer-events: none;
        }

        .game-container::after {
            content: "";
            position: absolute;
            bottom: 0;
            right: 0;
            width: 120px;
            height: 120px;
            background: linear-gradient(225deg, #e33b3b 0%, #e33b3b 50%, transparent 50%);
            z-index: 1;
            pointer-events: none;
        }

        .main-dashboard {
            display: flex;
            flex-wrap: wrap;
            min-height: 650px;
            background: rgba(10, 10, 12, 0.9);
        }

        /* 左侧场景栏 */
        .scene-bar {
            width: 110px;
            background: #0f0f11;
            border-right: 2px solid #e33b3b;
            padding: 24px 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 28px;
        }

        .scene-item {
            text-align: center;
            cursor: pointer;
            transition: transform 0.1s ease;
            filter: grayscale(0.4);
            opacity: 0.7;
        }
        .scene-item.active {
            filter: grayscale(0);
            opacity: 1;
            transform: scale(1.05);
            text-shadow: 0 0 4px #e33b3b;
        }
        .scene-icon {
            font-size: 44px;
            display: block;
            background: #1e1e22;
            padding: 10px;
            border-radius: 20px;
            border: 1px solid #e33b3b50;
            margin-bottom: 8px;
        }
        .scene-name {
            font-size: 12px;
            font-weight: bold;
            color: #f0e6d0;
            letter-spacing: 1px;
            background: #00000080;
            padding: 2px 8px;
            border-radius: 20px;
        }
        .scene-item.active .scene-name {
            background: #e33b3b;
            color: white;
            box-shadow: 0 0 6px red;
        }

        /* 中央区域：NPC + 计时 + AI对话 */
        .character-area {
            flex: 3;
            min-width: 300px;
            background: linear-gradient(145deg, #131316, #0b0b0e);
            padding: 20px;
            display: flex;
            flex-direction: column;
            border-right: 1px solid #e33b3b80;
        }

        .npc-card {
            background: #000000aa;
            border-radius: 48px 48px 24px 24px;
            padding: 16px;
            text-align: center;
            border: 1px solid #e33b3b;
            box-shadow: 0 8px 0 #4a0e0e;
            margin-bottom: 16px;
        }

        .npc-name {
            font-size: 28px;
            font-weight: 800;
            color: #ffd966;
            text-shadow: 2px 2px 0 #b52e2e;
        }
        .npc-quote {
            color: #e0e0e0;
            font-style: italic;
            font-size: 14px;
            margin-top: 8px;
            padding: 8px;
            background: #1e1e1eaa;
            border-radius: 40px;
            min-height: 70px;
        }
        .npc-avatar {
            font-size: 100px;
            filter: drop-shadow(6px 8px 0 #3a0f0f);
            margin: 8px 0;
        }

        /* 计时器 */
        .timer-panel {
            background: #040404cc;
            border-radius: 40px;
            padding: 16px;
            margin-bottom: 16px;
            text-align: center;
            backdrop-filter: blur(8px);
            border: 1px solid #e33b3b;
        }
        .timer-display {
            font-family: 'Courier New', monospace;
            font-size: 52px;
            font-weight: 800;
            background: #000;
            padding: 8px 16px;
            display: inline-block;
            border-radius: 60px;
            color: #ff3a3a;
            letter-spacing: 4px;
            margin-bottom: 12px;
        }
        .timer-btn {
            background: #e33b3b;
            border: none;
            color: white;
            font-weight: bold;
            font-size: 24px;
            padding: 6px 28px;
            border-radius: 60px;
            cursor: pointer;
            margin: 0 6px;
            box-shadow: 0 4px 0 #691515;
            transition: 0.05s linear;
        }
        .timer-btn:active {
            transform: translateY(2px);
            box-shadow: 0 2px 0 #691515;
        }

        /* AI对话区域 */
        .chat-section {
            background: #0a0a0ccc;
            border-radius: 28px;
            border: 1px solid #e33b3b80;
            padding: 12px;
            margin-top: 8px;
        }
        .chat-messages {
            background: #010101aa;
            border-radius: 20px;
            height: 160px;
            overflow-y: auto;
            padding: 10px;
            font-size: 13px;
            display: flex;
            flex-direction: column;
            gap: 8px;
        }
        .message {
            padding: 6px 12px;
            border-radius: 20px;
            max-width: 85%;
            word-wrap: break-word;
        }
        .user-msg {
            background: #e33b3b;
            color: white;
            align-self: flex-end;
            text-align: right;
        }
        .npc-msg {
            background: #2c2c34;
            color: #ffebc2;
            align-self: flex-start;
            border-left: 3px solid #e33b3b;
        }
        .chat-input-area {
            display: flex;
            margin-top: 12px;
            gap: 8px;
        }
        .chat-input {
            flex: 1;
            background: #1e1e24;
            border: 1px solid #e33b3b;
            color: white;
            padding: 10px;
            border-radius: 40px;
            font-family: inherit;
            outline: none;
        }
        .send-btn {
            background: #e33b3b;
            border: none;
            color: white;
            padding: 0 20px;
            border-radius: 40px;
            font-weight: bold;
            cursor: pointer;
        }
        .ai-badge {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 8px;
            font-size: 12px;
            color: #ffb347;
        }
        .mode-switch {
            background: #2a2a30;
            border: none;
            color: #ccc;
            padding: 4px 12px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 11px;
        }
        .mode-switch.active {
            background: #e33b3b;
            color: white;
        }

        /* 右侧面板 */
        .info-panel {
            width: 260px;
            background: #0c0c0f;
            padding: 20px 12px;
            border-left: 2px solid #e33b3b;
            display: flex;
            flex-direction: column;
            gap: 20px;
        }
        .stat-card {
            background: #000000aa;
            border-radius: 24px;
            padding: 12px;
            text-align: center;
            border-bottom: 3px solid #e33b3b;
        }
        .stat-label {
            font-size: 18px;
            font-weight: bold;
            color: #e0b853;
        }
        .stat-value {
            font-size: 48px;
            font-weight: 800;
            color: #f0f0f0;
        }
        .map-mini {
            background: #0a0a0c;
            border-radius: 24px;
            padding: 12px;
            border: 1px solid #e33b3b80;
        }
        .map-mini h4 {
            color: #e33b3b;
            font-size: 14px;
            margin-bottom: 10px;
            text-align: center;
        }
        .map-station {
            display: flex;
            justify-content: space-between;
            margin: 8px 0;
            font-size: 12px;
            background: #1b1b20;
            padding: 5px 10px;
            border-radius: 40px;
        }
        .station-dot {
            width: 12px;
            height: 12px;
            background: gray;
            border-radius: 12px;
        }
        .station-dot.lit { background: #e33b3b; box-shadow: 0 0 6px red; }
        button.small {
            background: none;
            border: 1px solid gray;
            color: gray;
            border-radius: 20px;
            padding: 4px;
            margin-top: 8px;
            width: 100%;
            cursor: pointer;
        }

        footer {
            text-align: center;
            font-size: 10px;
            color: #555;
            padding: 6px;
            background: #000000aa;
        }
    </style>
</head>
<body>
<div class="game-container">
    <div class="main-dashboard">
        <div class="scene-bar">
            <div class="scene-item active" data-scene="library" id="scene-lib">
                <span class="scene-icon">📚</span>
                <span class="scene-name">图书馆</span>
            </div>
            <div class="scene-item" data-scene="cafe" id="scene-cafe">
                <span class="scene-icon">☕</span>
                <span class="scene-name">卢布朗</span>
            </div>
        </div>

        <div class="character-area">
            <div class="npc-card">
                <div class="npc-name" id="npcName">MONA</div>
                <div class="npc-avatar" id="npcAvatar">🐱🎒</div>
                <div class="npc-quote" id="npcQuote">「吾辈是AI版MONA！和我聊天就能巩固知识喵～」</div>
            </div>

            <div class="timer-panel">
                <div class="timer-display" id="timerDisplay">25:00</div>
                <div>
                    <button class="timer-btn" id="startTimerBtn">🔴 自习</button>
                    <button class="timer-btn" id="resetTimerBtn">🔄 重置</button>
                </div>
                <div class="timer-status" id="timerStatus" style="font-size:12px; margin-top:5px;">⚡ 专注25分钟，结束后知识+1</div>
            </div>

            <!-- AI 对话模块 -->
            <div class="chat-section">
                <div class="ai-badge">
                    <span>🤖 AI 智能对话 (实时学习助手)</span>
                    <div>
                        <button id="mockModeBtn" class="mode-switch active">🎭 模拟AI</button>
                        <button id="realAIModeBtn" class="mode-switch">🌐 真AI (需API)</button>
                    </div>
                </div>
                <div class="chat-messages" id="chatMessages">
                    <div class="message npc-msg">🐱 MONA: 「欢迎来到学习空间！你可以问我知识点、最近学了什么，或者让我抽查你喵～」</div>
                </div>
                <div class="chat-input-area">
                    <input type="text" id="chatInput" class="chat-input" placeholder="提问/总结/让NPC抽查..." autocomplete="off">
                    <button id="sendMsgBtn" class="send-btn">🗣️ 对话</button>
                </div>
                <div style="font-size: 10px; color:#aaa; margin-top: 6px; text-align:center;">✨ 支持: 知识点答疑 / 学习总结 / 随机抽查 / 背单词互动</div>
            </div>
        </div>

        <div class="info-panel">
            <div class="stat-card">
                <div class="stat-label">📖 知识能力</div>
                <div class="stat-value" id="knowledgeValue">0</div>
                <button id="debugAddBtn" style="background:#3a2a2a; border:none; color:white; border-radius:20px; padding:5px; margin-top:5px; cursor:pointer;">➕ 测试+知识</button>
            </div>
            <div class="map-mini">
                <h4>🗺️ 知识路线 · 数学分析</h4>
                <div id="stationList"></div>
                <button id="resetMapDemo" class="small">重置地图(演示)</button>
            </div>
        </div>
    </div>
    <footer>✨ AI对话支持学习总结、抽查、知识点掉落 | 真AI模式需配置OpenAI/DeepSeek API</footer>
</div>

<script>
    // ---------- 游戏状态 ----------
    let knowledge = 0;
    let currentScene = "library"; 
    let timerInterval = null;
    let timeSeconds = 25 * 60;
    let isTiming = false;

    // ---------- AI 模式: mock / real ----------
    let aiMode = "mock";   // "mock" 或 "real"
    // 真实API配置 (需用户自行填入)
    let API_KEY = "";      // 建议在localStorage设定或弹窗输入，这里为了体验提供设置入口
    let API_URL = "https://api.openai.com/v1/chat/completions";  // 可替换为DeepSeek等

    // NPC角色设定 (供AI使用)
    const npcPersonality = {
        library: "你是女神异闻录5中的MONA，一只神秘又自傲的猫咪，喜欢用「吾辈」自称，语气活泼带喵喵口癖，擅长鼓励学生学习，可以抽查数学、英语等知识点，帮助学生总结学习内容。保持热情、中二又可爱的风格。",
        cafe: "你是佐仓双叶，天才黑客少女，性格有点宅但很聪明，说话有时会用网络用语，亲切又有点俏皮。你擅长用类比和图表帮助用户理解知识，也可以抽查学习效果并给出复习建议。"
    };

    // 模拟AI的智能回复库 (具备掉落知识点、抽查等功能)
    function mockAIResponse(userMessage, scene, currentKnowledge) {
        const msg = userMessage.toLowerCase();
        // 抽查逻辑
        if (msg.includes("抽查") || msg.includes("考我") || msg.includes("提问")) {
            const questions = [
                { q: "「数列极限的ε-δ定义中，ε代表什么？」", a: "任意小的正数" },
                { q: "「函数连续的三要素是什么？」", a: "有定义、极限存在、极限值等于函数值" },
                { q: "「导数定义的极限表达式是什么？」", a: "lim(Δx→0) (f(x+Δx)-f(x))/Δx" },
                { q: "「罗尔定理的条件是什么？」", a: "闭区间连续，开区间可导，端点值相等" }
            ];
            const rand = questions[Math.floor(Math.random() * questions.length)];
            return `📚 抽查时间！${rand.q} (回答后我可以给你解析)`;
        }
        // 学习总结/反思
        if (msg.includes("总结") || msg.includes("反思") || msg.includes("我今天学了")) {
            return `🌟 太棒了！及时总结是学习的关键。能把今天学到的核心概念用自己的话复述一遍吗？我会帮你强化记忆！${scene === 'library' ? '喵~' : ' 加油!'}`;
        }
        // 知识点掉落 (碎片化巩固)
        if (msg.includes("知识点") || msg.includes("掉落") || msg.includes("讲一下")) {
            const tips = [
                "无穷级数收敛的必要条件是通项趋于0喵！",
                "夹逼准则：两边夹，中间得极限。",
                "微分中值定理联系函数与导数，是证明题的利器。",
                "泰勒展开可以用多项式逼近复杂函数。"
            ];
            return `✨ 知识点掉落: ${tips[Math.floor(Math.random() * tips.length)]} 需要更详细解析吗？`;
        }
        // 背单词交互
        if (msg.includes("单词") || msg.includes("背单词")) {
            const words = [["rigorous", "严谨的"], ["theorem", "定理"], ["convergence", "收敛"], ["derivative", "导数"]];
            const w = words[Math.floor(Math.random() * words.length)];
            return `📖 单词卡: ${w[0]} —— ${w[1]}。 下次我会继续掉落新词喵!`;
        }
        // 默认智能回复 + 结合知识值
        if (currentKnowledge > 5) {
            return `看起来你知识值已经${currentKnowledge}了！相当不错喵～ 要继续挑战难题吗？还是让我抽查你最近学的章节？`;
        }
        return `「${userMessage}」关于学习，吾辈建议你从基础概念入手～ 要不要试试「抽查」或者让我给你掉落一个知识点？`;
    }

    // 真实AI调用 (OpenAI风格，可替换)
    async function callRealAI(userMessage, scene, knowledgeLevel) {
        if (!API_KEY) {
            return "⚠️ 未配置API Key！请点击右上角设置API密钥，或使用模拟AI模式。\n(临时方案：点击「模拟AI」按钮即可免费使用内置智能对话)";
        }
        const systemPrompt = `${npcPersonality[scene]} 当前学生的学习能力值(知识点数)为 ${knowledgeLevel}，你应结合此数值给予适当难度和鼓励。对话要简短有趣，可以包含掉落知识点、抽查或对用户总结的反馈。`;
        try {
            const response = await fetch(API_URL, {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json',
                    'Authorization': `Bearer ${API_KEY}`
                },
                body: JSON.stringify({
                    model: "gpt-3.5-turbo",
                    messages: [
                        { role: "system", content: systemPrompt },
                        { role: "user", content: userMessage }
                    ],
                    temperature: 0.8,
                    max_tokens: 300
                })
            });
            const data = await response.json();
            if (data.choices && data.choices[0] && data.choices[0].message) {
                return data.choices[0].message.content;
            } else {
                return "AI 返回错误，请检查API配置。切换到模拟模式试试~";
            }
        } catch (err) {
            return `网络错误: ${err.message}。建议用模拟AI模式。`;
        }
    }

    // 获取NPC名字/表情前缀
    function getNPCNameAndIcon() {
        if (currentScene === "library") return { name: "MONA", icon: "🐱" };
        return { name: "双叶", icon: "🍔" };
    }

    // 核心对话调用
    async function sendMessageToNPC(userText) {
        if (!userText.trim()) return;
        const { name, icon } = getNPCNameAndIcon();
        // 显示用户消息
        addMessageToChat("user", `👤 你: ${userText}`);
        
        // 让AI思考中临时占位
        const loadingId = addLoadingMessage();
        
        let reply = "";
        try {
            if (aiMode === "mock") {
                // 模拟AI支持上下文增强
                reply = mockAIResponse(userText, currentScene, knowledge);
            } else {
                reply = await callRealAI(userText, currentScene, knowledge);
            }
        } catch(e) {
            reply = "AI遇到问题啦，请刷新或切换到模拟模式。";
        }
        // 移除loading
        removeLoadingMessage(loadingId);
        const finalMsg = `${icon} ${name}: ${reply}`;
        addMessageToChat("npc", finalMsg);
        // 同时更新NPC头顶气泡显示最新一句亮点
        document.getElementById("npcQuote").innerText = reply.slice(0, 80);
        // 趣味彩蛋：如果对话涉及学习完成, 不额外加减知识，但可以给个隐藏鼓励
        if (reply.includes("知识点掉落") && Math.random() > 0.7) {
            setTimeout(() => {
                addMessageToChat("npc", `✨ 因为专注互动，你的知识值悄悄提升了1点! ✨`);
                addKnowledge(1);
            }, 800);
        }
    }

    let msgContainer = document.getElementById("chatMessages");
    function addMessageToChat(type, content) {
        const div = document.createElement("div");
        div.className = `message ${type === "user" ? "user-msg" : "npc-msg"}`;
        div.innerText = content;
        msgContainer.appendChild(div);
        div.scrollIntoView({ behavior: "smooth", block: "nearest" });
    }
    function addLoadingMessage() {
        const id = "loading-" + Date.now();
        const div = document.createElement("div");
        div.id = id;
        div.className = "message npc-msg";
        div.innerText = "✍️ NPC 正在思考...";
        msgContainer.appendChild(div);
        div.scrollIntoView({ behavior: "smooth", block: "nearest" });
        return id;
    }
    function removeLoadingMessage(id) {
        const el = document.getElementById(id);
        if (el) el.remove();
    }

    // 知识+地图系统
    const stations = [
        { name: "🐉 数列极限", lit: false, need: 2 },
        { name: "📈 函数连续", lit: false, need: 4 },
        { name: "🧮 导数定义", lit: false, need: 6 },
        { name: "🎯 微分中值", lit: false, need: 8 },
        { name: "🏆 级数收敛", lit: false, need: 10 }
    ];
    function updateKnowledgeUI() {
        document.getElementById("knowledgeValue").innerText = knowledge;
        let changed = false;
        stations.forEach(s => {
            const should = knowledge >= s.need;
            if (s.lit !== should) { s.lit = should; changed = true; }
        });
        if (changed) renderMap();
        saveGame();
    }
    function addKnowledge(amount) {
        knowledge += amount;
        updateKnowledgeUI();
        if (amount > 0 && currentScene === "library") 
            document.getElementById("npcQuote").innerText = `知识+${amount}！继续学习喵!`;
        else if(amount > 0)
            document.getElementById("npcQuote").innerText = `知识+${amount}！好厉害！`;
        setTimeout(() => updateNPCByScene(), 2000);
    }
    function renderMap() {
        const container = document.getElementById("stationList");
        if (!container) return;
        container.innerHTML = "";
        stations.forEach(s => {
            const div = document.createElement("div");
            div.className = "map-station";
            div.innerHTML = `<span>${s.name}</span><div class="station-dot ${s.lit ? 'lit' : ''}"></div>`;
            container.appendChild(div);
        });
    }
    function updateNPCByScene() {
        const data = (currentScene === "library") ? 
            { name: "MONA", avatar: "🐱🎒", quote: "「吾辈与你同在喵！聊学习或抽查都行～」" } : 
            { name: "佐仓双叶", avatar: "🍔🖥️", quote: "「卢布朗信号稳定，随时可以帮你总结知识哦！」" };
        document.getElementById("npcName").innerText = data.name;
        document.getElementById("npcAvatar").innerText = data.avatar;
        document.getElementById("npcQuote").innerText = data.quote;
    }
    function setScene(scene) {
        currentScene = scene;
        document.getElementById("scene-lib").classList.toggle("active", scene === "library");
        document.getElementById("scene-cafe").classList.toggle("active", scene === "cafe");
        updateNPCByScene();
        saveGame();
    }
    // 计时器
    function startTimer() {
        if (isTiming) return;
        isTiming = true;
        timerInterval = setInterval(() => {
            if (timeSeconds <= 1) {
                clearInterval(timerInterval);
                isTiming = false;
                timeSeconds = 25 * 60;
                updateTimerDisplay();
                addKnowledge(1);
                document.getElementById("timerStatus").innerText = "✅ 专注完成！知识+1，辛苦了！";
                setTimeout(() => document.getElementById("timerStatus").innerText = "⚡ 专注25分钟，结束后知识+1", 3000);
            } else {
                timeSeconds--;
                updateTimerDisplay();
            }
        }, 1000);
    }
    function resetTimer() {
        if (timerInterval) clearInterval(timerInterval);
        isTiming = false;
        timeSeconds = 25 * 60;
        updateTimerDisplay();
        document.getElementById("timerStatus").innerText = "⚡ 计时已重置";
    }
    function updateTimerDisplay() {
        let mins = Math.floor(timeSeconds / 60);
        let secs = timeSeconds % 60;
        document.getElementById("timerDisplay").innerText = `${mins.toString().padStart(2,'0')}:${secs.toString().padStart(2,'0')}`;
    }
    function saveGame() { localStorage.setItem("p5r_save", JSON.stringify({ knowledge, currentScene })); }
    function loadGame() {
        let d = localStorage.getItem("p5r_save");
        if (d) { let obj = JSON.parse(d); knowledge = obj.knowledge || 0; currentScene = obj.currentScene || "library"; setScene(currentScene); updateKnowledgeUI(); }
        else updateKnowledgeUI();
    }

    // 模式切换与API设置(简易弹窗)
    document.getElementById("mockModeBtn").addEventListener("click", () => {
        aiMode = "mock";
        document.getElementById("mockModeBtn").classList.add("active");
        document.getElementById("realAIModeBtn").classList.remove("active");
        addMessageToChat("npc", "🎭 已切换到模拟AI模式，可以免费使用全部智能对话功能！");
    });
    document.getElementById("realAIModeBtn").addEventListener("click", () => {
        if (!API_KEY) {
            let key = prompt("请输入OpenAI API Key (或DeepSeek兼容密钥，需有余额)", "");
            if (key && key.length > 10) { API_KEY = key; 
                addMessageToChat("npc", "🌐 真实AI模式已启用！你可以畅快对话了。"); }
            else { alert("未输入有效Key, 保持模拟模式"); return; }
        }
        aiMode = "real";
        document.getElementById("realAIModeBtn").classList.add("active");
        document.getElementById("mockModeBtn").classList.remove("active");
        addMessageToChat("npc", "🌐 已切换至真实AI模式！ (若未配置API将提示错误)");
    });
    
    // 事件绑定
    document.getElementById("sendMsgBtn").addEventListener("click", () => {
        let input = document.getElementById("chatInput");
        if (input.value.trim()) sendMessageToNPC(input.value);
        input.value = "";
    });
    document.getElementById("chatInput").addEventListener("keypress", (e) => { if(e.key === "Enter") document.getElementById("sendMsgBtn").click(); });
    document.getElementById("startTimerBtn").addEventListener("click", startTimer);
    document.getElementById("resetTimerBtn").addEventListener("click", resetTimer);
    document.getElementById("debugAddBtn").addEventListener("click", () => addKnowledge(1));
    document.getElementById("resetMapDemo").addEventListener("click", () => { stations.forEach(s => s.lit=false); renderMap(); addMessageToChat("npc", "🗺️ 地图已重置，但知识值还在，继续学习点亮吧！"); });
    document.getElementById("scene-lib").addEventListener("click", () => setScene("library"));
    document.getElementById("scene-cafe").addEventListener("click", () => setScene("cafe"));
    
    loadGame();
    updateTimerDisplay();
    renderMap();
</script>
</body>
</html>

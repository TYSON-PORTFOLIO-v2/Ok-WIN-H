<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OKWin Hack - Advanced Prediction System</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;600;700&family=Poppins:wght@300;400;500;600&display=swap');
        
        :root {
            --primary: #3a1b6e;
            --primary-light: #5d2d9e;
            --secondary: #00a8e8;
            --big-color: #ff9f1c;
            --small-color: #4cc9f0;
            --danger: #ff3860;
            --warning: #ffb703;
            --success: #2ecc71;
            --dark: #121212;
            --darker: #0a0a0a;
            --light: #e0e0e0;
            --lighter: #ffffff;
            --gold: #ffd700;
            --silver: #c0c0c0;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #0c061f 0%, #1a0a38 100%);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            color: var(--lighter);
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
            -webkit-font-smoothing: antialiased;
            position: relative;
        }
        
        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><rect width="100" height="100" fill="none"/><path d="M0,50 L100,50 M50,0 L50,100" stroke="rgba(93, 45, 158, 0.1)" stroke-width="1"/></svg>');
            opacity: 0.3;
            z-index: -1;
        }

        /* Main Container */
        .container {
            width: 100%;
            max-width: 500px;
            background: rgba(18, 18, 18, 0.95);
            border-radius: 20px;
            padding: 25px;
            margin-bottom: 20px;
            border: 1px solid var(--primary-light);
            position: relative;
            overflow: hidden;
            box-shadow: 0 0 30px rgba(93, 45, 158, 0.3);
            z-index: 10;
        }
        
        .container::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 80% 20%, rgba(93, 45, 158, 0.1) 0%, transparent 40%);
            pointer-events: none;
        }

        /* Winner Container */
        .winner-container {
            text-align: center;
            padding: 15px;
            background: linear-gradient(90deg, rgba(93, 45, 158, 0.1), rgba(0, 168, 232, 0.1));
            border-radius: 12px;
            margin-bottom: 18px;
            border: 1px solid var(--primary-light);
            position: relative;
            overflow: hidden;
            box-shadow: 0 0 10px rgba(93, 45, 158, 0.2);
        }

        .winner-container::after {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, 
                transparent, 
                rgba(93, 45, 158, 0.2), 
                transparent);
            transition: left 0.8s ease-out;
        }

        .winner-container:hover::after {
            left: 100%;
        }

        .winner-text {
            font-size: 15px;
            font-weight: 500;
            color: var(--lighter);
            letter-spacing: 0.5px;
            background: linear-gradient(90deg, var(--light), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 10px rgba(0, 168, 232, 0.2);
        }

        /* Online Users */
        .online-users {
            text-align: center;
            padding: 12px;
            background: rgba(0, 168, 232, 0.1);
            border-radius: 12px;
            margin-bottom: 25px;
            font-size: 14px;
            color: var(--secondary);
            border: 1px solid var(--secondary);
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease-out;
            position: relative;
        }

        .online-users:hover {
            box-shadow: 0 0 15px rgba(0, 168, 232, 0.3);
            transform: translateY(-2px);
        }

        .online-users i {
            margin-right: 8px;
            font-size: 12px;
        }

        /* Game Header */
        .game-header {
            display: flex;
            align-items: center;
            margin-bottom: 25px;
            padding-bottom: 18px;
            border-bottom: 1px solid rgba(93, 45, 158, 0.3);
            position: relative;
        }
        
        .premium-badge {
            position: absolute;
            top: -10px;
            right: -10px;
            background: linear-gradient(45deg, var(--gold), var(--warning));
            color: #000;
            padding: 5px 10px;
            border-radius: 15px;
            font-size: 10px;
            font-weight: 700;
            transform: rotate(15deg);
            box-shadow: 0 3px 10px rgba(255, 183, 3, 0.5);
            z-index: 20;
        }

        .game-logo {
            width: 70px;
            height: 70px;
            border-radius: 18px;
            margin-right: 18px;
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            border: 2px solid var(--primary-light);
            box-shadow: 0 0 20px rgba(93, 45, 158, 0.4);
            position: relative;
        }
        
        .game-logo::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at center, rgba(255,255,255,0.2) 0%, transparent 70%);
        }

        .game-logo img {
            width: 80%;
            height: 80%;
            object-fit: contain;
            filter: drop-shadow(0 0 5px rgba(255,255,255,0.3));
        }

        .game-info {
            flex: 1;
        }

        .game-name {
            font-family: 'Orbitron', sans-serif;
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 5px;
            color: var(--lighter);
            letter-spacing: 1px;
            background: linear-gradient(90deg, var(--light), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(0, 168, 232, 0.3);
        }

        .game-about {
            font-style: italic;
            font-size: 12px;
            opacity: 0.7;
            color: var(--light);
            letter-spacing: 0.3px;
        }
        
        /* Features */
        .features-container {
            display: flex;
            justify-content: space-between;
            margin-bottom: 25px;
            background: rgba(18, 18, 18, 0.7);
            border-radius: 12px;
            padding: 15px;
            border: 1px solid rgba(93, 45, 158, 0.3);
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
        }
        
        .feature-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            flex: 1;
            padding: 5px;
        }
        
        .feature-icon {
            font-size: 18px;
            margin-bottom: 8px;
            color: var(--secondary);
        }
        
        .feature-text {
            font-size: 12px;
            color: var(--light);
        }
        
        .feature-item:nth-child(1) .feature-icon {
            color: var(--gold);
        }
        
        .feature-item:nth-child(2) .feature-icon {
            color: var(--success);
        }
        
        .feature-item:nth-child(3) .feature-icon {
            color: var(--warning);
        }

        /* Game Type Selector */
        .game-type-container {
            display: flex;
            justify-content: space-between;
            margin-bottom: 25px;
            background: rgba(93, 45, 158, 0.1);
            border-radius: 12px;
            padding: 10px;
            border: 1px solid var(--primary-light);
        }

        .game-type {
            flex: 1;
            padding: 12px 8px;
            text-align: center;
            font-family: 'Orbitron', sans-serif;
            font-size: 12px;
            font-weight: 600;
            color: var(--light);
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.2s ease-out;
            margin: 0 5px;
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(93, 45, 158, 0.3);
        }

        .game-type.selected {
            background: var(--primary);
            color: white;
            border-color: var(--primary-light);
            box-shadow: 0 0 10px rgba(93, 45, 158, 0.4);
        }

        .game-type:not(.selected):hover {
            background: rgba(93, 45, 158, 0.2);
        }

        /* Prediction Container */
        .prediction-container {
            background: rgba(18, 18, 18, 0.7);
            padding: 20px;
            border-radius: 15px;
            margin-bottom: 20px;
            border: 1px solid var(--primary-light);
            box-shadow: 0 0 15px rgba(93, 45, 158, 0.1);
            position: relative;
        }
        
        .prediction-container::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            border-radius: 0 0 15px 15px;
        }

        .server-status {
            display: flex;
            align-items: center;
            margin-bottom: 18px;
            font-size: 14px;
            color: var(--light);
            justify-content: space-between;
        }
        
        .server-status-left {
            display: flex;
            align-items: center;
        }
        
        .ping-indicator {
            background: rgba(0, 0, 0, 0.3);
            padding: 4px 10px;
            border-radius: 15px;
            font-size: 12px;
            color: var(--light);
            border: 1px solid var(--primary-light);
            display: flex;
            align-items: center;
        }
        
        .ping-indicator i {
            margin-right: 5px;
            font-size: 10px;
        }
        
        .ping-value {
            font-weight: 600;
            margin-left: 3px;
            color: var(--success);
        }

        .status-dot {
            width: 8px;
            height: 8px;
            background: var(--secondary);
            border-radius: 50%;
            margin-right: 12px;
            box-shadow: 0 0 10px var(--secondary);
            animation: pulse 2s infinite ease-out;
        }

        @keyframes pulse {
            0%, 100% { opacity: 0.7; transform: scale(0.95); }
            50% { opacity: 1; transform: scale(1); }
        }

        /* Input Group */
        .input-group {
            margin-bottom: 20px;
            position: relative;
        }

        .input-group label {
            display: block;
            margin-bottom: 8px;
            font-size: 13px;
            color: var(--light);
            letter-spacing: 0.3px;
            display: flex;
            align-items: center;
        }
        
        .input-group label i {
            margin-right: 8px;
            color: var(--secondary);
            font-size: 14px;
        }

        .input-group input {
            width: 100%;
            padding: 14px 18px;
            background: rgba(0, 0, 0, 0.3);
            border: 1px solid var(--primary-light);
            border-radius: 10px;
            color: white;
            font-size: 14px;
            outline: none;
            transition: all 0.2s ease-out;
            letter-spacing: 0.5px;
        }

        .input-group input:focus {
            border-color: var(--secondary);
            background: rgba(0, 0, 0, 0.4);
            box-shadow: 0 0 10px rgba(0, 168, 232, 0.2);
        }

        .error-message {
            position: absolute;
            bottom: -20px;
            left: 0;
            color: var(--danger);
            font-size: 11px;
            opacity: 0;
            transition: opacity 0.2s ease-out;
        }

        .shake {
            animation: shake 0.4s ease-out both;
        }

        @keyframes shake {
            0%, 100% { transform: translateX(0); }
            20%, 60% { transform: translateX(-5px); }
            40%, 80% { transform: translateX(5px); }
        }

        /* Flip Card */
        .flip-card {
            width: 80px;
            height: 100px;
            margin: 25px auto;
            perspective: 1000px;
        }

        .flip-card-inner {
            position: relative;
            width: 100%;
            height: 100%;
            transition: transform 0.4s ease-out;
            transform-style: preserve-3d;
            border-radius: 12px;
        }

        .flip-card.flipped .flip-card-inner {
            transform: rotateY(180deg);
        }

        .flip-card-front, .flip-card-back {
            position: absolute;
            width: 100%;
            height: 100%;
            backface-visibility: hidden;
            border-radius: 12px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border: 2px solid rgba(255, 255, 255, 0.15);
        }

        .flip-card-front {
            background: rgba(30, 30, 40, 0.9);
            box-shadow: 0 0 20px rgba(93, 45, 158, 0.3);
        }
        
        .flip-card-front::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at center, rgba(255,255,255,0.1) 0%, transparent 70%);
        }

        .flip-card-back {
            background: var(--small-color);
            transform: rotateY(180deg);
            font-family: 'Orbitron', sans-serif;
            font-size: 16px;
            font-weight: 800;
            color: white;
            box-shadow: 0 0 25px var(--small-color);
        }

        .flip-card-back.big {
            background: var(--big-color);
            box-shadow: 0 0 25px var(--big-color);
        }

        .flip-card-back.small {
            background: var(--small-color);
            box-shadow: 0 0 25px var(--small-color);
        }

        .flip-card-icon {
            font-size: 24px;
            margin-bottom: 8px;
            color: rgba(255, 255, 255, 0.6);
        }

        .flip-card-text {
            font-size: 8px;
            color: var(--light);
            text-align: center;
            max-width: 80%;
        }
        
        /* Earn Limit */
        .earn-limit {
            text-align: center;
            padding: 12px;
            background: rgba(255, 215, 0, 0.1);
            border-radius: 12px;
            margin: 20px 0;
            font-size: 14px;
            color: var(--gold);
            border: 1px solid var(--gold);
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
        }
        
        .earn-limit i {
            margin-right: 10px;
            font-size: 16px;
        }

        /* Buttons */
        .btn {
            width: 100%;
            padding: 16px;
            border: none;
            border-radius: 10px;
            font-size: 15px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.2s ease-out;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            letter-spacing: 0.5px;
            position: relative;
            overflow: hidden;
        }

        .btn::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(
                to bottom right,
                rgba(255,255,255,0) 0%,
                rgba(255,255,255,0) 45%,
                rgba(255,255,255,0.1) 48%,
                rgba(255,255,255,0.1) 52%,
                rgba(255,255,255,0) 55%,
                rgba(255,255,255,0) 100%
            );
            transform: rotate(30deg);
            transition: all 0.5s ease-out;
        }

        .btn:hover::after {
            left: 100%;
            top: 100%;
        }

        .btn-primary {
            background: linear-gradient(45deg, var(--primary), var(--primary-light));
            color: white;
            box-shadow: 0 0 15px rgba(93, 45, 158, 0.4);
        }

        .btn-primary:hover {
            box-shadow: 0 0 20px rgba(93, 45, 158, 0.6);
            transform: translateY(-2px);
        }

        .btn-warning {
            background: linear-gradient(45deg, var(--warning), #ff9500);
            color: #000;
            box-shadow: 0 0 15px rgba(255, 183, 3, 0.4);
        }

        .btn-warning:hover {
            box-shadow: 0 0 20px rgba(255, 183, 3, 0.6);
            transform: translateY(-2px);
        }

        .btn-danger {
            background: linear-gradient(45deg, var(--danger), #ff1a4a);
            color: white;
            box-shadow: 0 0 15px rgba(255, 56, 96, 0.4);
        }

        .btn-danger:hover {
            box-shadow: 0 0 20px rgba(255, 56, 96, 0.6);
            transform: translateY(-2px);
        }

        /* Warning Text */
        .warning-text {
            font-size: 12px;
            text-align: center;
            margin: 20px 0;
            color: var(--warning);
            font-style: italic;
            letter-spacing: 0.3px;
            line-height: 1.5;
            padding: 12px;
            background: rgba(255, 183, 3, 0.08);
            border-radius: 8px;
            border-left: 3px solid var(--warning);
        }

        .btn-icon {
            margin-right: 10px;
            font-size: 14px;
        }
        
        /* Footer */
        .footer {
            text-align: center;
            font-size: 11px;
            color: rgba(255, 255, 255, 0.5);
            margin-top: 10px;
            padding: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="winner-container">
            <div class="winner-text" id="winnerText">User {random_620-999}****{random_000-999} Win ₹{random_500-15000}</div>
        </div>
        
        <div class="online-users">
            <i class="fas fa-users"></i>
            <span id="onlineUsers">Online Users: {random_500-7000}</span>
        </div>
        
        <div class="game-header">
            <div class="game-logo">
                <img src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMDAiIGhlaWdodD0iMTAwIiB2aWV3Qm94PSIwIDAgMTAwIDEwMCI+PHJlY3Qgd2lkdGg9IjEwMCIgaGVpZ2h0PSIxMDAiIGZpbGw9IiMzYjFjNzQiLz48cGF0aCBkPSJNNTAgMTVMMjAgNDBoNjB6IiBmaWxsPSIjZmZmIi8+PHBhdGggZD0iTTUwIDg1TDIwIDYwaDYweiIgZmlsbD0iI2ZmZiIvPjwvc3ZnPg==" alt="OKWin Logo">
            </div>
            <div class="game-info">
                <div class="premium-badge">PRO VERSION</div>
                <div class="game-name">OKWin Hack</div>
                <div class="game-about">Next-generation prediction system, earn money easily. 🚀</div>
            </div>
        </div>
        
        <div class="features-container">
            <div class="feature-item">
                <div class="feature-icon">👑</div>
                <div class="feature-text">Private Server</div>
            </div>
            <div class="feature-item">
                <div class="feature-icon">☄️</div>
                <div class="feature-text">More Accurate</div>
            </div>
            <div class="feature-item">
                <div class="feature-icon">💯</div>
                <div class="feature-text">Safe & Secure</div>
            </div>
        </div>
        
        <div class="game-type-container">
            <div class="game-type" data-type="30s">WINGO 30s</div>
            <div class="game-type selected" data-type="1m">WINGO 1m</div>
            <div class="game-type" data-type="3m">WINGO 3m</div>
        </div>
        
        <div class="prediction-container">
            <div class="server-status">
                <div class="server-status-left">
                    <div class="status-dot"></div>
                    <div>Server: Active</div>
                </div>
                <div class="ping-indicator">
                    <i class="fas fa-bolt"></i> Ping: <span class="ping-value" id="pingValue">18ms</span>
                </div>
            </div>
            
            <div class="input-group">
                <label for="periodNumber"><i class="fas fa-key"></i> ENTER PERIOD NO:</label>
                <input type="text" id="periodNumber" placeholder="Enter period number...">
                <div class="error-message" id="errorMessage">Please enter a period number</div>
            </div>
            
            <div class="flip-card" id="flipCard">
                <div class="flip-card-inner">
                    <div class="flip-card-front">
                        <i class="fas fa-dice flip-card-icon"></i>
                        <div class="flip-card-text">Click Start to predict</div>
                    </div>
                    <div class="flip-card-back" id="resultCard">
                        --
                    </div>
                </div>
            </div>
            
            <button class="btn btn-primary" id="startBtn">
                <i class="fas fa-play btn-icon"></i> START PREDICTION
            </button>
            
            <div class="warning-text">
                Make a new OKWin account by clicking on below "Register" button, otherwise hack will not work properly.
            </div>
            
            <button class="btn btn-warning" id="registerBtn">
                <i class="fas fa-user-plus btn-icon"></i> REGISTER NOW !
            </button>
            
            <button class="btn btn-danger" id="telegramBtn">
                <i class="fab fa-telegram btn-icon"></i> JOIN TELEGRAM
            </button>
        </div>
        
        <div class="earn-limit">
            <i class="fas fa-money-bill-wave"></i>
            <span>Earn Limit: 1,00,000₹</span>
        </div>
    </div>
    
    <div class="footer">
        OKWin Hack &copy; 2023 | Advanced Prediction System
    </div>
    
    <script>
        // Optimized winner text update
        let lastWinnerUpdate = 0;
        function updateWinner(timestamp) {
            if (!lastWinnerUpdate || timestamp - lastWinnerUpdate >= 2500) {
                lastWinnerUpdate = timestamp;
                const randomId1 = Math.floor(Math.random() * 380) + 620;
                const randomId2 = Math.floor(Math.random() * 1000).toString().padStart(3, '0');
                const randomAmount = Math.floor(Math.random() * 14500) + 500;
                document.getElementById('winnerText').textContent = 
                    `User ${randomId1}****${randomId2} Win ₹${randomAmount.toLocaleString()}`;
            }
            requestAnimationFrame(updateWinner);
        }

        // Optimized online users update
        let lastUsersUpdate = 0;
        function updateOnlineUsers(timestamp) {
            if (!lastUsersUpdate || timestamp - lastUsersUpdate >= 3000) {
                lastUsersUpdate = timestamp;
                const randomUsers = Math.floor(Math.random() * 6500) + 500;
                document.getElementById('onlineUsers').textContent = `Online Users: ${randomUsers.toLocaleString()}`;
            }
            requestAnimationFrame(updateOnlineUsers);
        }
        
        // Real-time ping simulation
        function updatePing() {
            const pingValue = document.getElementById('pingValue');
            const basePing = 5 + Math.random() * 15;
            const ping = Math.floor(basePing);
            pingValue.textContent = `${ping}ms`;
            
            // Change color based on ping
            if (ping < 15) {
                pingValue.style.color = '#2ecc71';
            } else if (ping < 25) {
                pingValue.style.color = '#f39c12';
            } else {
                pingValue.style.color = '#e74c3c';
            }
        }

        // Initialize
        document.addEventListener('DOMContentLoaded', () => {
            // Start animation frame loops
            requestAnimationFrame(updateWinner);
            requestAnimationFrame(updateOnlineUsers);
            
            // Update ping every second
            setInterval(updatePing, 1000);
            updatePing();

            // Game type selection
            const gameTypes = document.querySelectorAll('.game-type');
            gameTypes.forEach(type => {
                type.addEventListener('click', function() {
                    gameTypes.forEach(t => t.classList.remove('selected'));
                    this.classList.add('selected');
                });
            });
            
            // Handle start button click
            document.getElementById('startBtn').addEventListener('click', function() {
                const periodNumber = document.getElementById('periodNumber').value.trim();
                const flipCard = document.getElementById('flipCard');
                const resultCard = document.getElementById('resultCard');
                const errorMessage = document.getElementById('errorMessage');
                const inputField = document.getElementById('periodNumber');
                const startBtn = this;
                
                if (!periodNumber) {
                    errorMessage.style.opacity = '1';
                    inputField.classList.add('shake');
                    setTimeout(() => {
                        inputField.classList.remove('shake');
                    }, 400);
                    return;
                }
                
                errorMessage.style.opacity = '0';
                startBtn.disabled = true;
                startBtn.innerHTML = '<i class="fas fa-cog fa-spin btn-icon"></i> PROCESSING...';
                
                if (flipCard.classList.contains('flipped')) {
                    flipCard.classList.remove('flipped');
                }
                
                setTimeout(() => {
                    const isBig = Math.random() > 0.5;
                    resultCard.textContent = isBig ? 'BIG' : 'SMALL';
                    resultCard.className = 'flip-card-back ' + (isBig ? 'big' : 'small');
                    
                    setTimeout(() => {
                        flipCard.classList.add('flipped');
                        startBtn.disabled = false;
                        startBtn.innerHTML = '<i class="fas fa-play btn-icon"></i> START PREDICTION';
                    }, 800);
                    
                }, flipCard.classList.contains('flipped') ? 400 : 0);
            });
            
            // Other event listeners
            document.getElementById('registerBtn').addEventListener('click', () => {
                window.open('https://www.okwin.game//#/register?invitationCode=565455654920', '_blank');
            });
            
            document.getElementById('telegramBtn').addEventListener('click', () => {
                window.open('https://t.me/TYSON_OK_WIN_HACK', '_blank');
            });
            
            document.getElementById('periodNumber').addEventListener('input', function() {
                const flipCard = document.getElementById('flipCard');
                if (flipCard.classList.contains('flipped')) {
                    flipCard.classList.remove('flipped');
                }
                document.getElementById('errorMessage').style.opacity = '0';
            });

            // Add hover effect to winner container
            const winnerContainer = document.querySelector('.winner-container');
            winnerContainer.addEventListener('mouseenter', () => {
                winnerContainer.querySelector('::after').style.left = '100%';
            });
        });
    </script>
</body>
</html>

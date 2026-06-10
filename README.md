
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Sumi's Magical Birthday Funhouse! 🎀✨ | From Subho</title>
    <link href="https://fonts.googleapis.com/css2?family=Special+Elite&family=Playfair+Display:ital,wght@0,400;0,600;1,400&family=Kalam:wght@300;400;700&family=Caveat:wght@400;700&family=Fredoka+One&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        
        body {
            min-height: 100vh;
            background: linear-gradient(135deg, #fdf0e0 0%, #ffe6d5 50%, #fef0e5 100%);
            background-attachment: fixed;
            font-family: 'Kalam', cursive;
            color: #4a2a1a;
            padding: 1rem;
            position: relative;
            cursor: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="24" height="27" viewBox="0 0 24 27"><circle cx="12" cy="12" r="10" fill="%23ffb347" stroke="%23ff8c00" stroke-width="1.5"/><text x="12" y="17" font-size="14" text-anchor="middle" fill="white">⭐</text></svg>') 12 12, auto;
        }
        
        /* Floating sparkles background */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 200 200"><text x="10" y="30" font-size="20">✨</text><text x="150" y="80" font-size="25">🌟</text><text x="40" y="170" font-size="18">⭐</text><text x="170" y="150" font-size="22">💫</text><text x="80" y="40" font-size="16">✨</text></svg>');
            background-repeat: repeat;
            opacity: 0.1;
            pointer-events: none;
            z-index: 0;
        }
        
        .main-wrapper {
            max-width: 1400px;
            margin: 0 auto;
            background: rgba(255, 251, 245, 0.92);
            border-radius: 45px 45px 70px 70px;
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.15), inset 0 1px 2px rgba(255,255,200,0.8);
            padding: 1.8rem;
            backdrop-filter: blur(3px);
            border: 2px solid #ffdbb5;
            position: relative;
            z-index: 1;
        }
        
        /* Bouncy header */
        .hero {
            text-align: center;
            animation: bounceIn 0.8s ease;
        }
        
        @keyframes bounceIn {
            0% { transform: scale(0.8); opacity: 0; }
            80% { transform: scale(1.05); }
            100% { transform: scale(1); opacity: 1; }
        }
        
        .cursive-big {
            font-family: 'Fredoka One', cursive;
            font-size: 4rem;
            background: linear-gradient(135deg, #e8855a, #f5b87a, #e8a06e);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            text-shadow: 3px 3px 10px rgba(0,0,0,0.1);
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-8px); }
        }
        
        .typewriter-date {
            font-family: 'Special Elite', monospace;
            background: linear-gradient(135deg, #ffe0b5, #ffd4a0);
            display: inline-block;
            padding: 0.5rem 2rem;
            border-radius: 60px;
            margin-top: 12px;
            font-size: 1rem;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
        }
        
        .doodle-row {
            display: flex;
            justify-content: center;
            gap: 18px;
            flex-wrap: wrap;
            margin: 20px 0;
            font-size: 2rem;
        }
        
        .doodle-row span {
            animation: wiggle 2s ease-in-out infinite;
            display: inline-block;
        }
        
        @keyframes wiggle {
            0%, 100% { transform: rotate(0deg); }
            25% { transform: rotate(8deg); }
            75% { transform: rotate(-8deg); }
        }
        
        /* Friendship banner */
        .friendship-banner {
            background: linear-gradient(135deg, #fff5e8, #ffefdd);
            border-radius: 70px;
            padding: 1rem;
            text-align: center;
            margin-bottom: 2rem;
            border: 2px solid #ffd9ae;
            box-shadow: 0 8px 20px rgba(0,0,0,0.05);
        }
        
        /* Games Grid */
        .games-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 1.8rem;
            margin: 2rem 0;
        }
        
        .game-card {
            background: #fffef8;
            border-radius: 40px 20px 40px 20px;
            padding: 1.3rem;
            box-shadow: 0 12px 25px rgba(0, 0, 0, 0.1);
            transition: all 0.3s;
            border: 1px solid #ffebcd;
            position: relative;
            overflow: hidden;
        }
        
        .game-card:hover {
            transform: translateY(-8px) scale(1.01);
            box-shadow: 0 20px 35px rgba(0, 0, 0, 0.15);
        }
        
        .game-card::before {
            content: '✨';
            position: absolute;
            top: -10px;
            right: -10px;
            font-size: 2rem;
            opacity: 0.3;
            transform: rotate(15deg);
        }
        
        .game-title {
            font-family: 'Fredoka One', cursive;
            font-size: 1.6rem;
            text-align: center;
            border-bottom: 2px dotted #ffcc99;
            padding-bottom: 8px;
            margin-bottom: 1rem;
            color: #c97a4a;
        }
        
        /* Balloon Game */
        .balloon-area {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 12px;
            min-height: 130px;
            margin: 10px 0;
        }
        .balloon {
            font-size: 2.8rem;
            cursor: pointer;
            transition: 0.08s linear;
            filter: drop-shadow(2px 4px 6px rgba(0,0,0,0.1));
        }
        .balloon:active { transform: scale(0.85); }
        .balloon-score { text-align: center; font-weight: bold; margin-top: 8px; }
        
        /* Memory Game */
        .memory-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 8px;
            margin: 10px 0;
        }
        .memory-card {
            background: linear-gradient(135deg, #ffd89b, #f5b87a);
            aspect-ratio: 1/1;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            cursor: pointer;
            transition: 0.2s;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .memory-card.flipped { background: #fff0dd; transform: scale(0.95); }
        .memory-card:hover { transform: scale(1.03); }
        
        /* Firefly Game */
        .firefly-area {
            background: linear-gradient(135deg, #2d1b3a, #1a0f25);
            border-radius: 30px;
            min-height: 150px;
            position: relative;
            cursor: crosshair;
            overflow: hidden;
            margin: 10px 0;
        }
        .firefly {
            position: absolute;
            font-size: 1.8rem;
            cursor: pointer;
            transition: 0.05s linear;
            animation: glow 1s infinite alternate;
        }
        @keyframes glow {
            from { text-shadow: 0 0 2px yellow; }
            to { text-shadow: 0 0 12px #ffdd77; }
        }
        .firefly-score { text-align: center; margin-top: 8px; font-weight: bold; color: #ffcc66; }
        
        /* Cake Decorator */
        .cake-decor {
            text-align: center;
        }
        .cake-base {
            font-size: 5rem;
            display: inline-block;
            margin: 10px;
        }
        .deco-buttons {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
            margin: 10px 0;
        }
        .deco-btn {
            background: #f5e0c8;
            border: none;
            font-size: 1.5rem;
            padding: 5px 12px;
            border-radius: 50px;
            cursor: pointer;
            transition: 0.1s;
        }
        .deco-btn:active { transform: scale(0.9); }
        
        /* Magic 8 Ball */
        .magic-ball {
            background: #2a2a3a;
            width: 100px;
            height: 100px;
            border-radius: 50%;
            margin: 10px auto;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            transition: 0.1s;
            box-shadow: 0 8px 15px rgba(0,0,0,0.2);
        }
        .magic-ball:active { transform: scale(0.95); }
        .magic-answer { text-align: center; margin-top: 10px; font-size: 0.9rem; }
        
        /* Buttons */
        .cute-btn {
            background: linear-gradient(135deg, #e8a87c, #d47a4a);
            border: none;
            color: white;
            padding: 6px 16px;
            border-radius: 40px;
            cursor: pointer;
            font-family: monospace;
            margin-top: 8px;
            font-weight: bold;
            transition: 0.2s;
        }
        .cute-btn:hover { transform: scale(1.05); background: linear-gradient(135deg, #f5b88a, #e88955); }
        
        /* Photo Gallery */
        .polaroid-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
            gap: 20px;
            margin: 1.5rem 0;
        }
        .polaroid {
            background: #fffcf3;
            padding: 12px 12px 18px;
            border-radius: 20px;
            box-shadow: 8px 12px 20px rgba(0,0,0,0.1);
            transform: rotate(var(--rot, 0deg));
            transition: all 0.3s;
            cursor: pointer;
            text-align: center;
        }
        .polaroid:hover { transform: rotate(0deg) scale(1.02); }
        .polaroid img {
            width: 100%;
            aspect-ratio: 1/1;
            object-fit: cover;
            border-radius: 15px;
        }
        .compliment-badge {
            background: #ffe8d4;
            border-radius: 30px;
            padding: 4px 8px;
            font-size: 0.7rem;
            margin-top: 8px;
        }
        
        /* Floating animation */
        .floating-emoji {
            position: fixed;
            pointer-events: none;
            z-index: 10000;
            font-size: 1.8rem;
            animation: floatUp 2.5s ease-out forwards;
        }
        @keyframes floatUp {
            0% { transform: translateY(0) scale(0.5); opacity: 1; }
            100% { transform: translateY(-500px) scale(1.2); opacity: 0; }
        }
        
        footer { text-align: center; margin-top: 2rem; font-size: 0.8rem; padding-top: 1rem; border-top: 2px dashed #ffd9ae; }
        
        @media (max-width: 650px) {
            .cursive-big { font-size: 2.5rem; }
            .games-grid { gap: 1rem; }
        }
    </style>
</head>
<body>

<div class="main-wrapper">
    <div class="hero">
        <div class="doodle-row">🎈✨🍰🌸🎀🧸🍒📸💖</div>
        <div class="cursive-big">🎉 Happy Birthday, Sumi! 🎉</div>
        <div class="typewriter-date"><i class="fas fa-calendar-alt"></i> 14th June — Bestie's Magical Day! <i class="fas fa-star"></i></div>
        <div class="doodle-row">💛🙌🍭🐱🎁🎨🦋🍰🎀✨</div>
    </div>

    <div class="friendship-banner">
        <i class="fas fa-handshake fa-2x" style="color:#e8a87c;"></i>
        <p style="font-size: 1.2rem; margin-top: 8px;">To my amazing bestie Sumi — you're the sparkle in every day! 💛</p>
        <p>— Subho ✨</p>
    </div>

    <!-- GAMES SECTION -->
    <div class="games-grid">
        
        <!-- Game 1: Pop the Balloons -->
        <div class="game-card">
            <div class="game-title"><i class="fas fa-balloon"></i> Pop the Balloons!</div>
            <div class="balloon-area" id="balloonArea"></div>
            <div class="balloon-score" id="balloonScore">🎈 Popped: 0</div>
            <button class="cute-btn" id="refreshBalloonsBtn"><i class="fas fa-redo-alt"></i> New Balloons</button>
        </div>
        
        <!-- Game 2: Memory Match -->
        <div class="game-card">
            <div class="game-title"><i class="fas fa-puzzle-piece"></i> Memory Match 🧩</div>
            <div class="memory-grid" id="memoryGrid"></div>
            <div id="memoryStatus" style="text-align:center; font-size:0.8rem;">match the pairs!</div>
        </div>
        
        <!-- Game 3: Catch the Fireflies -->
        <div class="game-card">
            <div class="game-title"><i class="fas fa-bug"></i> Catch the Fireflies! 🦋</div>
            <div class="firefly-area" id="fireflyArea" style="height: 160px;"></div>
            <div class="firefly-score" id="fireflyScore">✨ Caught: 0</div>
            <button class="cute-btn" id="newFirefliesBtn"><i class="fas fa-sync-alt"></i> New Fireflies</button>
        </div>
        
        <!-- Game 4: Cake Decorator -->
        <div class="game-card">
            <div class="game-title"><i class="fas fa-birthday-cake"></i> Decorate the Cake! 🎂</div>
            <div class="cake-decor">
                <div class="cake-base" id="cakeDisplay">🎂</div>
                <div class="deco-buttons">
                    <button class="deco-btn" data-deco="🧁">🧁</button>
                    <button class="deco-btn" data-deco="🍒">🍒</button>
                    <button class="deco-btn" data-deco="✨">✨</button>
                    <button class="deco-btn" data-deco="🌸">🌸</button>
                    <button class="deco-btn" data-deco="🕯️">🕯️</button>
                    <button class="deco-btn" data-deco="🎀">🎀</button>
                </div>
                <button class="cute-btn" id="resetCakeBtn">Reset Cake</button>
            </div>
        </div>
        
        <!-- Game 5: Magic 8-Ball -->
        <div class="game-card">
            <div class="game-title"><i class="fas fa-magic"></i> Magic 8-Ball 🔮</div>
            <div class="magic-ball" id="magicBall">
                <span style="color: white; font-size: 1.5rem;">🎱</span>
            </div>
            <div class="magic-answer" id="magicAnswer">ask me anything!</div>
            <input type="text" id="magicQuestion" placeholder="ask a yes/no question..." style="width:100%; padding:6px; border-radius:50px; border:1px solid #ffcc99; margin-top:8px;">
        </div>
        
        <!-- Game 6: Fortune Cookie + Pet Cat combined -->
        <div class="game-card">
            <div class="game-title"><i class="fas fa-cookie-bite"></i> Fortune & Kitty 🍪🐱</div>
            <div id="fortuneMsg" style="background:#fff0e0; border-radius:30px; padding:10px; text-align:center; margin:8px 0;">🌸 click for a fortune!</div>
            <button class="cute-btn" id="fortuneBtn"><i class="fas fa-cookie"></i> Fortune Cookie</button>
            <div style="margin-top: 12px; text-align:center;">
                <span id="petCatEmoji" style="font-size:2.5rem; cursor:pointer;">🐱</span>
                <div id="catMsg" style="font-size:0.7rem;">pet the kitty!</div>
            </div>
        </div>
    </div>

    <!-- PHOTO GALLERY with compliments -->
    <div class="gallery-title" style="text-align:center; font-size:1.8rem; margin:1rem 0;">
        <i class="fas fa-camera-retro"></i> 10 Sweet Moments with Sumi 📸
    </div>
    <div class="polaroid-grid" id="polaroidGrid"></div>
    <p style="text-align: center; font-size: 0.7rem;">✨ click any photo to see a special compliment! ✨</p>

    <footer>
        <i class="fas fa-feather-alt"></i> made with magic & bestie love — for Sumi's special day 🎉
        <br>✨💛🎀🧸🍰🌸🐱🦋✨
    </footer>
</div>

<script>
    // ========== PHOTO GALLERY (10 photos - replace with your images) ==========
    // PUT YOUR PHOTOS IN "images" FOLDER AS photo1.jpg to photo10.jpg
    const photoPaths = [
        "images/photo1.jpg", "images/photo2.jpg", "images/photo3.jpg", "images/photo4.jpg", "images/photo5.jpg",
        "images/photo6.jpg", "images/photo7.jpg", "images/photo8.jpg", "images/photo9.jpg", "images/photo10.jpg"
    ];
    
    const compliments = [
        "🌸 You have the kindest heart! 🌸", "🍰 You're the funniest person ever! 🍰", "🎀 Your energy is pure magic! 🎀",
        "🧸 You're such a loyal friend! 🧸", "✨ Your smile lights up everything! ✨", "🍒 You're so talented and creative! 🍒",
        "📸 Hanging out with you is always a blast! 📸", "🐻‍❄️ You're so strong and brave! 🐻‍❄️",
        "💛 You make the world better just by being you! 💛", "🎉 You're the coolest bestie ever! 🎉"
    ];
    
    const captions = ["🌸 sunny", "🍰 cake time", "🎀 cute", "🧸 cozy", "✨ sparkle", "🍒 fun", "📸 memory", "🐻 adventure", "💛 happy", "🎉 party"];
    
    const polaroidGrid = document.getElementById('polaroidGrid');
    
    for (let i = 0; i < 10; i++) {
        const polaroid = document.createElement('div');
        polaroid.className = 'polaroid';
        const rot = (Math.random() * 6 - 3).toFixed(1);
        polaroid.style.setProperty('--rot', `${rot}deg`);
        
        const img = document.createElement('img');
        img.src = photoPaths[i];
        img.alt = `Sumi ${i+1}`;
        img.onerror = function() { this.src = `data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 200'%3E%3Crect width='200' height='200' fill='%23faeedb'/%3E%3Ctext x='100' y='110' text-anchor='middle' fill='%23b87a4a'%3E📸 Photo ${i+1}%3C/text%3E%3C/svg%3E`; };
        
        const captionDiv = document.createElement('div');
        captionDiv.innerHTML = `<i class="fas fa-heart" style="color:#e8a87c;"></i> ${captions[i]} <i class="fas fa-heart" style="color:#e8a87c;"></i>
                                <div class="compliment-badge" id="compBadge${i}">✨ tap for compliment ✨</div>`;
        
        polaroid.appendChild(img);
        polaroid.appendChild(captionDiv);
        
        const badge = captionDiv.querySelector(`.compliment-badge`);
        polaroid.addEventListener('click', () => {
            badge.innerHTML = `💬 "${compliments[i]}" 💬`;
            badge.style.background = "#ffd9b5";
            createFloatingEmoji('💛');
            setTimeout(() => {
                badge.innerHTML = `✨ tap for compliment ✨`;
                badge.style.background = "#ffe8d4";
            }, 3500);
        });
        polaroidGrid.appendChild(polaroid);
    }
    
    // ========== GAME 1: BALLOON POP ==========
    let balloonsPopped = 0;
    const balloonArea = document.getElementById('balloonArea');
    const balloonScore = document.getElementById('balloonScore');
    
    function createBalloons() {
        balloonArea.innerHTML = '';
        for(let i=0; i<8; i++) {
            const balloon = document.createElement('div');
            balloon.className = 'balloon';
            balloon.innerHTML = ['🎈','🎈','🎈','🎈','🎈','🎈','🎈','🎈','🎈'][Math.floor(Math.random()*9)];
            balloon.addEventListener('click', () => {
                balloonsPopped++;
                balloonScore.innerHTML = `🎈 Popped: ${balloonsPopped}`;
                balloon.style.opacity = '0';
                createFloatingEmoji('💥');
                setTimeout(() => balloon.remove(), 50);
            });
            balloonArea.appendChild(balloon);
        }
    }
    createBalloons();
    document.getElementById('refreshBalloonsBtn').addEventListener('click', createBalloons);
    
    // ========== GAME 2: MEMORY MATCH ==========
    c

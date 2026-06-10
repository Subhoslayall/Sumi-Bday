<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Happy Birthday Sumi! 🎀 | From Subho</title>
    <link href="https://fonts.googleapis.com/css2?family=Special+Elite&family=Playfair+Display:ital,wght@0,400;0,600;1,400&family=Kalam:wght@300;400;700&family=Caveat:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            min-height: 100vh;
            background: #fdf3e3;
            background-image: radial-gradient(circle at 20% 35%, rgba(210, 170, 100, 0.12) 2%, transparent 2.5%);
            font-family: 'Special Elite', 'Courier New', monospace;
            color: #3b2a1f;
            padding: 1.2rem;
        }
        .main-wrapper {
            max-width: 1400px;
            margin: 0 auto;
            background: rgba(254, 248, 235, 0.92);
            border-radius: 32px 32px 60px 60px;
            box-shadow: 0 25px 45px rgba(0, 0, 0, 0.1);
            padding: 1.8rem;
            border: 1px solid #ecdbba;
        }
        .hero { text-align: center; border-bottom: 2px dashed #e2caa0; padding-bottom: 1.2rem; margin-bottom: 1.8rem; }
        .cursive-big { font-family: 'Caveat', cursive; font-size: 4rem; font-weight: 700; background: linear-gradient(135deg, #bc6f3a, #e7a062); background-clip: text; -webkit-background-clip: text; color: transparent; }
        .typewriter-date { font-family: 'Special Elite', monospace; background: #f2e3cf; display: inline-block; padding: 0.3rem 1.5rem; border-radius: 50px; margin-top: 10px; font-size: 0.9rem; }
        .doodle-row { display: flex; justify-content: center; gap: 15px; flex-wrap: wrap; margin: 15px 0 8px; font-size: 1.8rem; }
        .friendship-banner { background: #fef5e8; border-radius: 30px; padding: 0.8rem; text-align: center; margin-bottom: 1.8rem; border-left: 8px solid #9bc48e; }
        .gallery-title { text-align: center; font-family: 'Caveat', cursive; font-size: 2rem; margin: 1.5rem 0 1rem; }
        .polaroid-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(210px, 1fr)); gap: 28px; justify-items: center; margin: 1.5rem 0; }
        .polaroid {
            background: #fffcf3;
            padding: 14px 14px 20px 14px;
            box-shadow: 8px 12px 20px rgba(0, 0, 0, 0.12);
            transform: rotate(var(--rot, 0deg));
            transition: all 0.3s;
            width: 100%;
            max-width: 230px;
            border-radius: 18px 18px 24px 24px;
            border: 1px solid #f2e2c0;
            cursor: pointer;
        }
        .polaroid:hover { transform: rotate(0deg) scale(1.02); box-shadow: 12px 18px 28px rgba(0, 0, 0, 0.15); }
        .polaroid img { width: 100%; aspect-ratio: 1/1; object-fit: cover; border-radius: 14px; filter: sepia(0.1); }
        .polaroid-caption { text-align: center; margin-top: 12px; font-family: 'Kalam', cursive; font-size: 1rem; font-weight: bold; color: #aa6a3c; }
        .compliment-badge { display: inline-block; background: #f5e6d4; border-radius: 40px; padding: 4px 12px; font-size: 0.75rem; margin-top: 6px; font-family: monospace; }
        .activities-row { display: flex; flex-wrap: wrap; gap: 1.2rem; margin: 2rem 0 1rem; justify-content: center; }
        .mini-card { background: #fffbf0; border-radius: 28px; padding: 0.8rem 1.2rem; flex: 1; min-width: 150px; text-align: center; border: 1px solid #f3e2c5; transition: 0.2s; }
        .mini-card:hover { transform: translateY(-3px); }
        .fortune-btn, .compliment-btn { background: #c9865c; border: none; color: white; padding: 6px 16px; border-radius: 30px; cursor: pointer; font-family: monospace; margin-top: 8px; }
        .floating-emoji { position: fixed; pointer-events: none; z-index: 10000; font-size: 1.5rem; animation: floatUp 2.5s ease-out forwards; }
        @keyframes floatUp { 0% { transform: translateY(0) scale(0.4); opacity: 0.9; } 100% { transform: translateY(-400px) scale(1.1); opacity: 0; } }
        footer { text-align: center; margin-top: 2rem; font-size: 0.7rem; border-top: 1px dashed #dec394; padding-top: 1rem; }
        @media (max-width: 650px) { .cursive-big { font-size: 2.8rem; } }
    </style>
</head>
<body>
<div class="main-wrapper">
    <div class="hero">
        <div class="doodle-row">🎈🍒📸🧸🌸🍰🎀🐻‍❄️🍬✨</div>
        <div class="cursive-big">🎉 Happy Birthday, Sumi! 🎉</div>
        <div class="typewriter-date"><i class="fas fa-calendar-alt"></i> 14th June — Bestie Birthday Bash! <i class="fas fa-star"></i></div>
        <div class="doodle-row">📸✨🎀</div>
    </div>

    <div class="friendship-banner">
        <i class="fas fa-handshake"></i> To my amazing friend Sumi — you're the best! Hope your day is filled with laughs, cake, and good vibes. <i class="fas fa-heart" style="color:#9bc48e;"></i> — Subho
    </div>

    <div class="gallery-title"><i class="fas fa-camera-retro"></i> 10 precious moments with Sumi <i class="fas fa-heart" style="color:#e8a87c;"></i></div>
    <div class="polaroid-grid" id="polaroidGrid"></div>
    <p style="text-align: center; font-size: 0.7rem;">✨ click any photo to see a special compliment! ✨</p>

    <div class="activities-row">
        <div class="mini-card"><i class="fas fa-cookie-bite fa-2x"></i><div id="fortuneMsg" style="font-size:0.8rem; margin:8px 0;">🌸 sweet message</div><button class="fortune-btn" id="fortuneBtn">Fortune Cookie</button></div>
        <div class="mini-card"><i class="fas fa-gift fa-2x"></i><div id="giftMsg" style="font-size:0.8rem; margin:8px 0;">🎁 open a gift</div><button class="compliment-btn" id="giftBtn">Open Gift</button></div>
        <div class="mini-card"><i class="fas fa-cat fa-2x"></i><div id="catMsg" style="font-size:0.8rem; margin:8px 0;">🐱 pet the kitty</div><button class="compliment-btn" id="petCatBtn">Pet Cat</button></div>
        <div class="mini-card"><i class="fas fa-smile fa-2x"></i><div id="complimentMsg" style="font-size:0.8rem; margin:8px 0;">💬 nice words</div><button class="compliment-btn" id="randomComplimentBtn">Compliment</button></div>
    </div>

    <footer><i class="fas fa-feather-alt"></i> made with doodles & bestie energy — for Sumi's 14th June 🎉</footer>
</div>

<script>
    // ========== YOUR 10 PHOTOS ==========
    // METHOD: Put your photos in "images" folder named photo1.jpg to photo10.jpg
    // Example: images/photo1.jpg, images/photo2.jpg, etc.
    
    const photoPaths = [
        "images/photo1.jpg",
        "images/photo2.jpg",
        "images/photo3.jpg",
        "images/photo4.jpg",
        "images/photo5.jpg",
        "images/photo6.jpg",
        "images/photo7.jpg",
        "images/photo8.jpg",
        "images/photo9.jpg",
        "images/photo10.jpg"
    ];
    
    // 10 unique compliments (friendly, no romance)
    const uniqueCompliments = [
        "🌸 You have the kindest heart! Always makes everyone feel welcome.",
        "🍰 You're literally the funniest person I know — your memes are iconic!",
        "🎀 Your energy is so positive and uplifting. Thanks for being you!",
        "🧸 You're an amazing friend — so loyal, honest, and real. No cap!",
        "✨ Your smile lights up any room. Keep shining bestie!",
        "🍒 You're so creative and talented! Everything you do is awesome.",
        "📸 You have the best vibes — hanging out with you is always a blast!",
        "🐻‍❄️ You're so strong and brave. I admire you a lot!",
        "💛 You make the world a better place just by being in it. Periodt.",
        "🎉 You're the coolest person to have late night chats with. Bestie forever!"
    ];
    
    const photoCaptions = ["🌸 sunny days", "🍰 cake time", "🎀 cute moment", "🧸 cozy vibes", "✨ sparkle energy", "🍒 fun times", "📸 memory lane", "🐻‍❄️ adventure", "💛 happy heart", "🎉 celebration"];
    
    const polaroidGrid = document.getElementById('polaroidGrid');
    
    for (let i = 0; i < 10; i++) {
        const polaroid = document.createElement('div');
        polaroid.className = 'polaroid';
        const rot = (Math.random() * 6 - 3).toFixed(1);
        polaroid.style.setProperty('--rot', `${rot}deg`);
        
        const img = document.createElement('img');
        img.src = photoPaths[i];
        img.alt = `Sumi's memory ${i+1}`;
        // if image fails to load, show placeholder
        img.onerror = function() {
            this.src = `data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 200'%3E%3Crect width='200' height='200' fill='%23faeedb'/%3E%3Ctext x='100' y='110' text-anchor='middle' fill='%23b87a4a'%3E📸 Photo ${i+1}%3C/text%3E%3C/svg%3E`;
        };
        
        const captionDiv = document.createElement('div');
        captionDiv.className = 'polaroid-caption';
        captionDiv.innerHTML = `<i class="fas fa-heart" style="color:#e6905f;"></i> ${photoCaptions[i]} <i class="fas fa-heart" style="color:#e6905f;"></i>
                                <div class="compliment-badge" id="complimentBadge${i}">✨ tap for compliment ✨</div>`;
        
        polaroid.appendChild(img);
        polaroid.appendChild(captionDiv);
        
        const complimentBadge = captionDiv.querySelector(`.compliment-badge`);
        polaroid.addEventListener('click', (function(index) {
            return function() {
                complimentBadge.innerHTML = `💬 "${uniqueCompliments[index]}" 💬`;
                complimentBadge.style.background = "#e8d5b8";
                createFloatingEmoji('💛');
                setTimeout(() => {
                    complimentBadge.innerHTML = `✨ tap for compliment ✨`;
                    complimentBadge.style.background = "#f5e6d4";
                }, 4000);
            };
        })(i));
        
        polaroidGrid.appendChild(polaroid);
    }
    
    // Fortune Cookie
    const fortunes = ["🌸 Wishing you the happiest birthday ever, bestie!", "🍰 This year will bring you so much joy!", "🎀 You're the coolest friend ever!", "🧸 May your day be filled with good vibes!", "💛 You deserve all the amazing things!", "🍒 No cap, you're literally the best!"];
    document.getElementById('fortuneBtn').addEventListener('click', () => {
        document.getElementById('fortuneMsg').innerHTML = `🍪 "${fortunes[Math.floor(Math.random()*fortunes.length)]}" 🍪`;
        createFloatingEmoji('🍀');
    });
    
    // Gift
    const gifts = ["🎁 Virtual cupcake! 🧁", "📸 A cute photo sticker!", "🌸 Virtual flowers!", "🍰 Digital cake slice!"];
    let giftIdx = 0;
    document.getElementById('giftBtn').addEventListener('click', () => {
        document.getElementById('giftMsg').innerHTML = `🎁 ${gifts[giftIdx++ % gifts.length]} 🎁`;
        createFloatingEmoji('🎁');
    });
    
    // Pet cat
    let petCount = 0;
    document.getElementById('petCatBtn').addEventListener('click', () => {
        petCount++;
        document.getElementById('catMsg').innerHTML = `🐱 Petted ${petCount} time${petCount!==1?'s':''}! Purrs happily! 🐾`;
        createFloatingEmoji('🐱');
    });
    
    // Random compliment
    const extraComps = ["🌸 You're such a kind soul!", "🍰 Your smile makes everyone's day!", "🎀 You're literally the coolest bestie!", "✨ You have amazing vibes!", "🧸 You're so fun to be around!"];
    document.getElementById('randomComplimentBtn').addEventListener('click', () => {
        document.getElementById('complimentMsg').innerHTML = `💬 "${extraComps[Math.floor(Math.random()*extraComps.length)]}" 💬`;
        createFloatingEmoji('💛');
    });
    
    function createFloatingEmoji(emojiType = null) {
        const emojis = ['🌸', '🍒', '🧸', '🎀', '✨', '🍰', '💛', '🎉'];
        const chosen = emojiType || emojis[Math.floor(Math.random()*emojis.length)];
        const div = document.createElement('div');
        div.className = 'floating-emoji';
        div.innerHTML = chosen;
        div.style.left = Math.random() * 90 + 5 + '%';
        div.style.bottom = '-20px';
        document.body.appendChild(div);
        setTimeout(() => div.remove(), 2500);
    }
    
    setInterval(() => { if(Math.random() > 0.7) createFloatingEmoji(); }, 3000);
    window.addEventListener('load', () => { for(let i=0;i<5;i++) setTimeout(()=>createFloatingEmoji('🎉'), i*200); });
</script>
</body>
</html>

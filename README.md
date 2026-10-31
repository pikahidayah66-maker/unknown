
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Monik ♡</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,500&family=Poppins:wght@300;400;500;600&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --pink: #ffb6d5;
    --purple: #bd9bff;
    --white: #fff8ff;
    --dark: #100b25;
}

body {
    min-height: 100vh;
    overflow-x: hidden;
    background:
      radial-gradient(ellipse at top, #44305f 0%, transparent 60%),
      linear-gradient(145deg, #100b25, #24143e, #160d2c);
    color: var(--white);
    font-family: 'Poppins', sans-serif;
}

/* BACKGROUND STARS */

#stars {
    position: fixed;
    inset: 0;
    pointer-events: none;
    z-index: 0;
}

.star {
    position: absolute;
    background: white;
    border-radius: 50%;
    animation: twinkle 2s infinite alternate;
}

@keyframes twinkle {
    from { opacity: .15; transform: scale(.6); }
    to { opacity: 1; transform: scale(1.4); }
}

/* MAIN CONTAINER */

.container {
    position: relative;
    z-index: 2;
    width: 100%;
    max-width: 750px;
    margin: auto;
    padding: 55px 22px;
    text-align: center;
}

/* HEADER */

.top-label {
    color: #e4c5ff;
    font-size: 11px;
    letter-spacing: 6px;
    margin-bottom: 25px;
    animation: fadeIn 2s ease;
}

h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(48px, 12vw, 90px);
    line-height: 1.1;
    background: linear-gradient(
        90deg,
        #fff0f7,
        #ffacd4,
        #c8aaff,
        #fff0f7
    );
    background-size: 200%;
    -webkit-background-clip: text;
    color: transparent;
    animation: shine 5s linear infinite;
    text-shadow: 0 0 35px #d79bff30;
}

@keyframes shine {
    to { background-position: 200%; }
}

.subtitle {
    margin-top: 18px;
    font-size: 13px;
    letter-spacing: 3px;
    color: #d8c6e8;
}

/* DIVIDER */

.divider {
    width: 130px;
    height: 1px;
    margin: 32px auto;
    background: linear-gradient(
      90deg, transparent, #ffb6d5, transparent
    );
}

/* CAKE */

.cake-area {
    margin: 35px auto;
    position: relative;
    width: 220px;
    height: 190px;
}

.cake {
    position: absolute;
    bottom: 15px;
    left: 50%;
    transform: translateX(-50%);
    width: 175px;
    height: 90px;
    background: linear-gradient(135deg,#ffb7d9,#e878b1);
    border-radius: 12px 12px 20px 20px;
    box-shadow: 0 12px 35px #ff8fc655;
}

.cake::before {
    content: "";
    position: absolute;
    top: -22px;
    left: 0;
    width: 100%;
    height: 35px;
    background: #fff0fa;
    border-radius: 50%;
}

.cake::after {
    content: "♡  ♡  ♡";
    position: absolute;
    top: 34px;
    left: 0;
    width: 100%;
    text-align: center;
    color: #fff;
    font-size: 20px;
}

.plate {
    position: absolute;
    bottom: 5px;
    left: 50%;
    transform: translateX(-50%);
    width: 210px;
    height: 15px;
    background: #d9c8ef;
    border-radius: 50%;
    box-shadow: 0 5px 25px #d8b9ff66;
}

.candle {
    position: absolute;
    top: 28px;
    left: 50%;
    transform: translateX(-50%);
    height: 55px;
    width: 9px;
    background: repeating-linear-gradient(
      45deg,
      #fff,
      #fff 5px,
      #e5a4d1 5px,
      #e5a4d1 10px
    );
    z-index: 3;
    border-radius: 4px;
}

.flame {
    position: absolute;
    width: 15px;
    height: 22px;
    top: -22px;
    left: -3px;
    background: #ffdb83;
    border-radius: 50% 50% 40% 40%;
    box-shadow: 0 0 20px #ffcf67, 0 0 45px #ffb5a0;
    animation: flicker .7s infinite alternate;
    transform-origin: bottom;
}

@keyframes flicker {
    from { transform: rotate(-8deg) scale(.9); }
    to { transform: rotate(8deg) scale(1.1); }
}

.cake-hint {
    font-size: 11px;
    color: #dfc5f5;
    margin-top: 8px;
}

/* BUTTONS */

button {
    border: none;
    cursor: pointer;
    font-family: 'Poppins', sans-serif;
    transition: .3s;
}

.main-btn {
    padding: 14px 30px;
    border-radius: 40px;
    color: #291637;
    background: linear-gradient(110deg,#ffc4df,#d6b6ff);
    font-size: 13px;
    font-weight: 600;
    box-shadow: 0 0 25px #e8a8ff55;
    margin: 12px 5px;
}

.main-btn:hover {
    transform: translateY(-4px);
    box-shadow: 0 0 35px #f9b4e5;
}

.secondary-btn {
    padding: 12px 25px;
    border: 1px solid #d6b6ff88;
    border-radius: 30px;
    background: transparent;
    color: white;
    margin: 8px;
}

.secondary-btn:hover {
    background: #ffffff15;
}

/* MESSAGE CARD */

.message-card {
    display: none;
    margin: 35px auto;
    padding: 30px 23px;
    max-width: 540px;
    background: linear-gradient(
      145deg,
      #ffffff12,
      #d9b6ff0a
    );
    border: 1px solid #ffffff25;
    border-radius: 22px;
    backdrop-filter: blur(15px);
    box-shadow: 0 10px 50px #00000030;
    animation: appear 1s ease;
}

.message-card h2 {
    font-family: 'Playfair Display', serif;
    color: #ffc5e0;
    font-size: 30px;
    margin-bottom: 20px;
}

.message-card p {
    font-size: 13px;
    line-height: 2.1;
    color: #f5e9ff;
    text-align: left;
    margin-bottom: 15px;
}

.signature {
    text-align: right !important;
    color: #ffc5e0 !important;
    font-family: 'Playfair Display', serif;
    font-size: 19px !important;
    font-style: italic;
}

/* COUNTDOWN TEXT */

.little-note {
    color: #cbb8dc;
    font-size: 12px;
    line-height: 2;
    margin-top: 30px;
}

/* FLOATING HEARTS */

.floating {
    position: fixed;
    bottom: -30px;
    pointer-events: none;
    z-index: 1;
    animation: floatUp 7s linear forwards;
}

@keyframes floatUp {
    0% {
        transform: translateY(0) rotate(0deg);
        opacity: 0;
    }
    15% { opacity: .8; }
    100% {
        transform: translateY(-110vh) rotate(360deg);
        opacity: 0;
    }
}

/* CONFETTI */

.confetti {
    position: fixed;
    top: -20px;
    z-index: 10;
    pointer-events: none;
    animation: fall 4s linear forwards;
}

@keyframes fall {
    to {
        transform: translateY(110vh) rotate(900deg);
        opacity: 0;
    }
}

/* SURPRISE */

.surprise {
    display: none;
    margin: 30px auto;
    animation: appear 1s ease;
}

.surprise h2 {
    font-family: 'Playfair Display', serif;
    color: #ffc4df;
    font-size: 27px;
    margin-bottom: 15px;
}

.surprise p {
    color: #e9d9f5;
    font-size: 13px;
    line-height: 2;
}

/* ANIMATIONS */

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(15px); }
    to { opacity: 1; transform: translateY(0); }
}

@keyframes appear {
    from {
        opacity: 0;
        transform: translateY(25px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* FOOTER */

footer {
    margin-top: 65px;
    padding-bottom: 25px;
    color: #a995bd;
    font-size: 10px;
    letter-spacing: 2px;
}

/* MOBILE */

@media(max-width:480px) {
    .container { padding-top: 65px; }
    .message-card { padding: 25px 18px; }
    .cake-area { transform: scale(.9); }
}
</style>
</head>

<body>

<div id="stars"></div>

<main class="container">

    <div class="top-label">
        A LITTLE CELEBRATION FOR SOMEONE SPECIAL
    </div>

    <h1>Monik ♡</h1>

    <div class="subtitle">
        TODAY IS ALL ABOUT YOU
    </div>

    <div class="divider"></div>

    <p style="font-size:13px;color:#e6d4f3;">
        A special day for a special person.
        Something beautiful is waiting for you...
    </p>

    <!-- BIRTHDAY CAKE -->

    <div class="cake-area">
        <div class="plate"></div>
        <div class="cake"></div>
        <div class="candle">
            <div class="flame" id="flame"></div>
        </div>
    </div>

    <p class="cake-hint">
        ♡ Make a wish and click the candle ♡
    </p>

    <button class="main-btn" onclick="openLetter()">
        Open Your Birthday Letter ♡
    </button>

    <button class="secondary-btn" onclick="celebrate()">
        ✨ Make It Magical
    </button>

    <!-- LETTER -->

    <section class="message-card" id="letter">

        <h2>Dear Monik, ♡</h2>

        <p>
            Happy Birthday, Monik!
            Selamat bertambah usia untuk salah satu
            manusia yang semoga selalu dikelilingi
            hal-hal baik dalam hidupnya.
        </p>

        <p>
            Di hari spesial ini, aku berharap kamu
            selalu punya alasan untuk tersenyum.
            Semoga semua hal yang sedang kamu
            perjuangkan perlahan menemukan jalannya.
        </p>

        <p>
            Semoga langkahmu selalu dipertemukan
            dengan kesempatan baik, orang-orang
            tulus, kebahagiaan sederhana, dan
            cerita-cerita indah yang belum pernah
            kamu bayangkan sebelumnya.
        </p>

        <p>
            Jangan terlalu keras sama diri sendiri,
            ya. Kamu juga berhak istirahat,
            bahagia, dan menikmati setiap proses
            yang sedang kamu jalani.
        </p>

        <p>
            May your new chapter be filled with
            beautiful surprises, endless laughter,
            unforgettable memories, and dreams
            that slowly turn into reality.
        </p>

        <p>
            Keep being yourself, keep growing,
            and never forget how precious
            your existence is.
        </p>

        <p>
            Once again, happy birthday!
            Semoga tahun ini menjadi salah satu
            bab paling indah dalam hidupmu.
        </p>

        <p class="signature">
            With love, ♡
        </p>

    </section>

    <!-- SURPRISE -->

    <section class="surprise" id="surprise">

        <h2>One More Thing... ✨</h2>

        <p>
            If I could give you one thing today,
            I would give you the ability to see
            yourself through the eyes of people
            who appreciate you.
        </p>

        <p style="margin-top:15px;">
            You deserve all the beautiful things
            this world has to offer.
        </p>

        <h1 style="font-size:40px;margin-top:25px;">
            HAPPY BIRTHDAY!
        </h1>

        <p style="margin-top:15px;">
            Monik, this day is yours. Enjoy every second! ♡
        </p>

    </section>

    <div class="divider"></div>

    <p class="little-note">
        Made with love, stars, and a little bit of magic.
        <br>
        This little website exists just for you, Monik.
    </p>

    <footer>
        ✦ A LITTLE WEBSITE FOR MONIK ✦
        <br><br>
        © 2026 — MADE WITH ♡
    </footer>

</main>

<script>

// CREATE STARS

const stars = document.getElementById("stars");

for(let i = 0; i < 100; i++) {

    let star = document.createElement("div");

    star.className = "star";

    star.style.left = Math.random() * 100 + "%";
    star.style.top = Math.random() * 100 + "%";

    let size = Math.random() * 3 + 1;

    star.style.width = size + "px";
    star.style.height = size + "px";

    star.style.animationDelay =
        Math.random() * 3 + "s";

    stars.appendChild(star);
}


// FLOATING HEARTS

const symbols = ["♡", "✦", "✨", "🌸", "💗"];

function createFloating() {

    let item = document.createElement("div");

    item.className = "floating";

    item.innerHTML =
        symbols[Math.floor(Math.random() * symbols.length)];

    item.style.left = Math.random() * 100 + "vw";

    item.style.fontSize =
        Math.random() * 15 + 12 + "px";

    item.style.animationDuration =
        Math.random() * 4 + 5 + "s";

    document.body.appendChild(item);

    setTimeout(() => {
        item.remove();
    }, 9000);
}

setInterval(createFloating, 700);


// OPEN LETTER

function openLetter() {

    const letter = document.getElementById("letter");

    letter.style.display = "block";

    letter.scrollIntoView({
        behavior: "smooth",
        block: "center"
    });

    celebrate();
}


// BLOW THE CANDLE

let candleBlown = false;

document.querySelector(".cake-area")
.addEventListener("click", function() {

    const flame = document.getElementById("flame");

    if(!candleBlown) {

        flame.style.display = "none";

        candleBlown = true;

        alert("Your wish is on its way, Monik! ♡");

        celebrate();

    } else {

        flame.style.display = "block";

        candleBlown = false;
    }

});


// CONFETTI EFFECT

function celebrate() {

    const colors = [
        "#ffc1df",
        "#c9a5ff",
        "#fff1a8",
        "#ffffff",
        "#a9d9ff"
    ];

    for(let i = 0; i < 100; i++) {

        let confetti = document.createElement("div");

        confetti.className = "confetti";

        confetti.style.left =
            Math.random() * 100 + "vw";

        confetti.style.width =
            Math.random() * 8 + 4 + "px";

        confetti.style.height =
            Math.random() * 12 + 5 + "px";

        confetti.style.background =
            colors[Math.floor(Math.random() * colors.length)];

        confetti.style.borderRadius =
            Math.random() > .5 ? "50%" : "2px";

        confetti.style.animationDuration =
            Math.random() * 3 + 2 + "s";

        document.body.appendChild(confetti);

        setTimeout(() => {
            confetti.remove();
        }, 5500);
    }
}


// SURPRISE BUTTON

function showSurprise() {

    const surprise =
        document.getElementById("surprise");

    surprise.style.display = "block";

    surprise.scrollIntoView({
        behavior: "smooth",
        block: "center"
    });

    celebrate();
}


// CONNECT SURPRISE TO MAIN BUTTON

document.querySelector(".secondary-btn")
.addEventListener("click", showSurprise);


// CONSOLE MESSAGE

console.log(
    "%c HAPPY BIRTHDAY MONIK ♡ ",
    "color:#ffacd4;font-size:25px;font-weight:bold;"
);

console.log(
    "A little magic was created just for you."
);

</script>

</body>
</html>





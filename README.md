# nezhnoglad5012e.github.io
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IDK - скачай игру</title>
    <style>
        * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background: #008cff;
    color: #fff;
    line-height: 1.6;
}

/* навигация по сайту */
header {
    background: rgba(0, 0, 0, 0.9);
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 100;
    padding: 20px 0;
}

nav {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
}

.logo {
    font-size: 24px;
    font-weight: bold;
    color: #008cff;
}

nav ul {
    display: flex;
    list-style: none;
    gap: 30px;
}

nav ul a {
    color: #fff;
    text-decoration: none;
    transition: 0.3s;
}

nav ul a:hover {
    color: #46abfd;
}

/* главная хуйня */
.hero {
    height: 100vh;
    background: linear-gradient(135deg, #0a0a1a, #1a1a2e);
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding-top: 80px;
}

.hero h1 {
    font-size: 64px;
    margin-bottom: 20px;
    color: #008cff;
    text-shadow: 0 0 20px #ffffff(255, 65, 108, 0.5);
    animation: fadeInUp 1s ease;
}

.hero p {
    font-size: 24px;
    margin-bottom: 30px;
    animation: fadeInUp 1s ease 0.2s both;
}

.cta-btn {
    display: inline-block;
    background: linear-gradient(45deg, #008cff, #35a2fc);
    color: white;
    padding: 15px 40px;
    text-decoration: none;
    border-radius: 50px;
    font-weight: bold;
    transition: 0.3s;
    animation: fadeInUp 1s ease 0.4s both;
}

.cta-btn:hover {
    transform: scale(1.1);
    box-shadow: 0 0 30px #008cff;
}

/* секции */
section {
    padding: 80px 20px;
    max-width: 1200px;
    margin: 0 auto;
}

h2 {
    font-size: 36px;
    text-align: center;
    margin-bottom: 40px;
    color: #008cff;
}

/* об игре */
.about-content {
    text-align: center;
    max-width: 800px;
    margin: 0 auto;
    font-size: 18px;
    line-height: 1.8;
}

/* галери */
.gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.gallery-item {
    border-radius: 15px;
    overflow: hidden;
    transition: 0.3s;
}

.gallery-item img {
    width: 100%;
    height: auto;
    transition: 0.3s;
}

.gallery-item:hover {
    transform: scale(1.05);
}

/* требования */
.requirements-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.req-card {
    background: rgba(255, 255, 255, 0.1);
    padding: 30px;
    border-radius: 15px;
    backdrop-filter: blur(10px);
    transition: 0.3s;
}

.req-card:hover {
    transform: translateY(-10px);
    background: rgba(255, 255, 255, 0.2);
}

.req-card h3 {
    margin-bottom: 20px;
    color: #008cff;
}

.req-card ul {
    list-style: none;
}

.req-card li {
    margin: 10px 0;
}

/* скачять */
.download {
    text-align: center;
}

.download-btn {
    background: linear-gradient(45deg, #008cff, #48adfffd);
    color: white;
    border: none;
    padding: 20px 50px;
    font-size: 24px;
    font-weight: bold;
    border-radius: 50px;
    cursor: pointer;
    transition: 0.3s;
    margin: 20px 0;
}

.download-btn:hover {
    transform: scale(1.1);
    box-shadow: 0 0 40px #008cff;
}

.counter {
    font-size: 18px;
    color: #aaa;
}

/* подвал */
footer {
    background: #000;
    text-align: center;
    padding: 20px;
    color: #666;
}

/* АНиМЦийия */
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}


@media (max-width: 768px) {
    .hero h1 {
        font-size: 36px;
    }
    
    .hero p {
        font-size: 18px;
    }
    
    nav ul {
        gap: 15px;
    }
    
    .logo {
        font-size: 18px;
    }
    
    h2 {
        font-size: 28px;
    }
    
    .gallery-grid {
        grid-template-columns: 1fr;
    }
    
    .requirements-grid {
        grid-template-columns: 1fr;
    }
    
    .download-btn {
        font-size: 18px;
        padding: 15px 30px;
    }
}

#particlesCanvas {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    pointer-events: none;
    background: linear-gradient(135deg, #0a0a1a, #1a1a2e);
}

body {
    backdrop-filter: blur(0px);
    transition: backdrop-filter 0.3s;
}


section:hover {
    filter: blur(0.5px);
    transition: 0.3s;
}
.gallery-item img {
    filter: sepia(0.5) grayscale(0.3);
    transition: 0.5s;
}

.gallery-item:hover img {
    filter: sepia(0) grayscale(0);
    transform: scale(1.05);
}
.memory-float {
    position: fixed;
    bottom: 20%;
    right: 5%;
    font-size: 14px;
    color: rgba(255, 255, 255, 0.3);
    font-style: italic;
    animation: fadeInOut 8s infinite;
    pointer-events: none;
    z-index: 10;
}

@keyframes fadeInOut {
    0% { opacity: 0; transform: translateX(20px); }
    20% { opacity: 0.5; transform: translateX(0); }
    80% { opacity: 0.5; transform: translateX(0); }
    100% { opacity: 0; transform: translateX(-20px); }
}
/* Линии разрыва */
body::before {
    content: '';
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: repeating-linear-gradient(
        0deg,
        transparent,
        transparent 2px,
        rgba(255, 255, 255, 0.02) 2px,
        rgba(255, 255, 255, 0.02) 4px
    );
    pointer-events: none;
    z-index: 2;
}

/* Статический шум */
body::after {
    content: '';
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: repeating-linear-gradient(
        90deg,
        transparent,
        transparent 3px,
        rgba(0, 0, 0, 0.1) 3px,
        rgba(0, 0, 0, 0.1) 6px
    );
    pointer-events: none;
    z-index: 2;
    animation: noise 0.3s infinite;
}

@keyframes noise {
    0% { opacity: 0.3; }
    100% { opacity: 0.5; }
}
.req-card, .gallery-item {
    background: rgba(255, 255, 255, 0.05);
    backdrop-filter: blur(5px);
    border: 1px solid rgba(255, 255, 255, 0.1);
    transition: 0.5s;
}

.req-card:hover, .gallery-item:hover {
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
}
h1, h2, p, .cta-btn {
    animation: textShake 3s infinite;
}

@keyframes textShake {
    0%, 100% { transform: translate(0, 0); text-shadow: 0 0 0 rgba(0,0,0,0); }
    95% { transform: translate(0, 0); text-shadow: 0 0 0 rgba(0,0,0,0); }
    96% { transform: translate(-1px, 0); text-shadow: 2px 0 5px rgba(0,0,0,0.3); }
    97% { transform: translate(1px, -1px); text-shadow: -2px 0 5px rgba(0,0,0,0.3); }
    98% { transform: translate(0, 1px); text-shadow: 0 2px 5px rgba(0,0,0,0.3); }
    99% { transform: translate(-1px, 0); text-shadow: 2px 0 5px rgba(0,0,0,0.3); }
}
:root {
    --primary: #8b5a2b;
    --secondary: #5a3a1a;
    --accent: #c97e3a;
    --dark: #1e1a0c;
    --light: #e8ddc5;
    --glow: rgba(139, 90, 43, 0.5);
}
#fallingMemories {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 1;
    overflow: hidden;
}

.falling-item {
    position: absolute;
    font-size: 20px;
    opacity: 0.3;
    animation: fall 8s linear forwards;
    color: rgba(255,255,200,0.5);
}

@keyframes fall {
    0% {
        transform: translateY(-10%) rotate(0deg);
        opacity: 0.3;
    }
    100% {
        transform: translateY(110vh) rotate(360deg);
        opacity: 0;
    }
}
body::before {
content: '';
position: fixed;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: radial-gradient(ellipse at center, transparent 60%, rgba(0,0,0,0.6) 100%);
pointer-events: none;
z-index: 3;
}

body::after {
content: '';
position: fixed;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: repeating-linear-gradient(
45deg,
transparent,
transparent 2px,
rgba(0,0,0,0.1) 2px,
rgba(0,0,0,0.1) 4px


);
pointer-events: none;
z-index: 3;
animation: filmGrain 0.2s infinite;

}

@keyframes filmGrain {
0% { opacity: 0.3s; transform: translate(0, 0); }
100% { opacity: 0.5s; transform: translate(1px, -1px); }

}


/* Кастомный скроллбар */
::-webkit-scrollbar {
    width: 8px;
    background: #1a1a2e;
}

::-webkit-scrollbar-thumb {
    background: linear-gradient(135deg, #8b5a2b, #c97e3a);
    border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
    background: #2d00aa;
}
body {
    overflow-x: hidden;  /* убираем горизонтальный скролл */
    overflow-y: auto;    /* вертикальный оставляем */
}

/* И проверь, нет ли элементов шире экрана */
* {
    max-width: 100%;
}
/* ПОЛНОЕ ОТКЛЮЧЕНИЕ ВЫДЕЛЕНИЯ (кроме текстовых блоков) */
html, body, div, section, header, footer, nav, button, .card, .gallery-item, .req-card, .download-btn, .cta-btn {
    user-select: none;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    -webkit-tap-highlight-color: transparent;
}

/* ТОЛЬКО ТЕКСТ В ОПИСАНИЯХ МОЖНО ВЫДЕЛЯТЬ */
.about-content, .diary-entry, .req-card ul, .voice-message, .clock {
    user-select: text;
    -webkit-user-select: text;
    -moz-user-select: text;
    -ms-user-select: text;
}

/* Убираем синий фон при клике на ссылки */
a {
    -webkit-tap-highlight-color: transparent;
    outline: none;
}

/* Убираем выделение при фокусе */
:focus {
    outline: none;
}
    </style>
</head>
<body>
    
<canvas id="particlesCanvas"></canvas>
    <header>
        <nav>
            <div class="logo">IDK</div>
            <ul>
                <li><a href="#about">О игре</a></li>
                <li><a href="#gallery">Галерея</a></li>
                <li><a href="#requirements">Системные требования</a></li>
                <li><a href="#download">Скачать</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>IDK</h1>
            <p>Философская игра о человеке с деменцией</p>
            <a href="#download" class="cta-btn">СКАЧАТЬ ИГРУ</a>
        </div>
    </section>

    <section id="about" class="about">
        <h2>О ИГРЕ</h2>
        <div class="about-content">
            <p>IDK — У Джека есть семь дней. Пока деменция стирает его память, вы и ваша помощь способны замедлить неизбежное. Сможете ли вы помочь ему продержаться до конца?</p>
        </div>
    </section>

    <section id="gallery" class="gallery">
        <h2>ГАЛЕРЕЯ</h2>
        <div class="gallery-grid">
            <div class="gallery-item">
                <img src="https://i.pinimg.com/originals/52/bd/94/52bd948fd7c6daf6b9e1178406673716.jpg" alt="Скриншот 1">
            </div>
            <div class="gallery-item">
                <img src="https://static.kinguin.net/media/images/products/6349d3625e210700010c903d_fd2a4df88f18ef603fa7868ffa146f9c.jpg" alt="Скриншот 2">
            </div>
            <div class="gallery-item">
                <img src="https://www.digiseller.ru/preview/650560/p1_3366367_ced3a4ed.jpg" alt="Скриншот 3">
            </div>
        </div>
    </section>

    <section id="requirements" class="requirements">
        <h2>СИСТЕМНЫЕ ТРЕБОВАНИЯ</h2>
        <div class="requirements-grid">
            <div class="req-card">
                <h3>МИНИМАЛЬНЫЕ</h3>
                <ul>
                    <li>OS: Windows XP </li>
                    <li>CPU: норм</li>
                    <li>RAM: 1MB</li>
                    <li>GPU: По настроению</li>
                    <li>Storage: любой</li>
                </ul>
            </div>
            <div class="req-card">
                <h3>РЕКОМЕНДУЕМЫЕ</h3>
                <ul>
                    <li>OS: Windows VISTA</li>
                    <li>CPU: Microwave</li>
                    <li>RAM: печенье</li>
                    <li>GPU: iphone 5s</li>
                    <li>Storage: 1000000GB</li>
                </ul>
            </div>
        </div>
    </section>

    <section id="download" class="download">
        <h2>СКАЧАТЬ ИГРУ</h2>
        <p>Версия 1.0.0 | Размер: 2.5 GB</p>
        <button class="download-btn" id="downloadBtn">🦇 СКАЧАТЬ СЕЙЧАС 🦇</button>
        <div class="counter" id="downloadCounter">Загрузок: 0</div>
    </section>

    <footer>
        <p>© 2026 IDK. Все права защищены.</p>
    </footer>

    <script>
        // подсчет скок скачяло
let downloadCount = localStorage.getItem('downloadCount') || 0;
const counterElement = document.getElementById('downloadCounter');
const downloadBtn = document.getElementById('downloadBtn');

function updateCounter() {
    counterElement.innerHTML = `Загрузок: ${downloadCount}`;
}

updateCounter();

// кнопка скачять
downloadBtn.onclick = function() {
    // счетчик скачяваний
    downloadCount++;
    localStorage.setItem('downloadCount', downloadCount);
    updateCounter();
    
    // ебаная анимация
    downloadBtn.style.transform = 'scale(0.95)';
    setTimeout(() => {
        downloadBtn.style.transform = 'scale(1)';
    }, 200);
    
    
    
    
    
    // текстовый файл демо версии 
    const blob = new Blob(
        ['Это демо-версия игры IDK.\nСпасибо за скачивание!\n\nПолная версия выйдет скоро!'],
        { type: 'text/plain' }
    );
    const url = URL.createObjectURL(blob);
    const a = document.createElement('a');
    a.href = url;
    a.download = 'I_D_K.txt';
    document.body.appendChild(a);
    a.click();
    document.body.removeChild(a);
    URL.revokeObjectURL(url);
    
    // Сообщение
    alert('Скачивание началось! Спасибо за интерес к игре!');
};

// скролл до якоря
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            target.scrollIntoView({
                behavior: 'smooth',
                block: 'start'
            });
        }
    });
});

// Анимации еьаные
const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.style.opacity = '1';
            entry.target.style.transform = 'translateY(0)';
        }
    });
}, { threshold: 0.1 });

document.querySelectorAll('section').forEach(section => {
    section.style.opacity = '0';
    section.style.transform = 'translateY(30px)';
    section.style.transition = 'all 0.6s ease';
    observer.observe(section);
});
// ===== АНИМИРОВАННЫЙ ФОН С ЧАСТИЦАМИ =====
const canvas = document.getElementById('particlesCanvas');
const ctx = canvas.getContext('2d');

// Массив частиц
let particles = [];

// Количество частиц (чем больше, тем красивее, но тяжелее)
const PARTICLE_COUNT = 100;

// Настройки
let mouseX = null;
let mouseY = null;

// Функция изменения размера canvas
function resizeCanvas() {
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;
    initParticles();
}

// Создание частиц
function initParticles() {
    particles = [];
    for (let i = 0; i < PARTICLE_COUNT; i++) {
        particles.push({
            x: Math.random() * canvas.width,
            y: Math.random() * canvas.height,
            radius: Math.random() * 3 + 1, // размер от 1 до 4px
            speedX: (Math.random() - 0.5) * 0.5, // скорость по X
            speedY: (Math.random() - 0.5) * 0.5, // скорость по Y
            color: `hsl(${Math.random() * 60 + 320}, 70%, 60%)` // розово-красные оттенки
        });
    }
}


function drawParticles() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    
    for (let i = 0; i < particles.length; i++) {
        const p = particles[i];
        
        
        p.x += p.speedX;
        p.y += p.speedY;
        
        
        if (mouseX !== null && mouseY !== null) {
            const dx = p.x - mouseX;
            const dy = p.y - mouseY;
            const distance = Math.sqrt(dx * dx + dy * dy);
            const radius = 100;
            
            if (distance < radius) {
                const angle = Math.atan2(dy, dx);
                const force = (radius - distance) / radius * 2;
                p.x += Math.cos(angle) * force;
                p.y += Math.sin(angle) * force;
            }
        }
        
        
        if (p.x < 0) p.x = canvas.width;
        if (p.x > canvas.width) p.x = 0;
        if (p.y < 0) p.y = canvas.height;
        if (p.y > canvas.height) p.y = 0;
        
        // Рисуем частицу
        ctx.beginPath();
        ctx.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
        
        
        const gradient = ctx.createRadialGradient(p.x, p.y, 0, p.x, p.y, p.radius * 2);
        gradient.addColorStop(0, p.color);
        gradient.addColorStop(1, 'rgba(255, 65, 108, 0)');
        ctx.fillStyle = gradient;
        
        ctx.fill();
        
        
        ctx.shadowBlur = 10;
        ctx.shadowColor = p.color;
        ctx.fill();
        ctx.shadowBlur = 0;
    }
    
    
    ctx.beginPath();
    ctx.strokeStyle = 'rgba(255, 65, 108, 0.2)';
    ctx.lineWidth = 0.5;
    
    for (let i = 0; i < particles.length; i++) {
        for (let j = i + 1; j < particles.length; j++) {
            const dx = particles[i].x - particles[j].x;
            const dy = particles[i].y - particles[j].y;
            const distance = Math.sqrt(dx * dx + dy * dy);
            
            if (distance < 100) {
                ctx.beginPath();
                ctx.moveTo(particles[i].x, particles[i].y);
                ctx.lineTo(particles[j].x, particles[j].y);
                ctx.strokeStyle = `rgba(255, 65, 108, ${0.1 * (1 - distance / 100)})`;
                ctx.stroke();
            }
        }
    }
    
    requestAnimationFrame(drawParticles);
}


canvas.addEventListener('mousemove', (e) => {
    mouseX = e.clientX;
    mouseY = e.clientY;
});


canvas.addEventListener('mouseleave', () => {
    mouseX = null;
    mouseY = null;
});


window.addEventListener('resize', resizeCanvas);
resizeCanvas();
drawParticles();
color: `rgba(255, 255, 255, ${Math.random() * 0.5 + 0.5})` // белые частицы
const memories = [
    "Я здесь уже был?",
    "Кто я?",
    "Это мой дом?",
    "Вспомни...",
    "Не забывай...",
    "Где мои ключи?",
    "Лицо знакомое...",
    "Странное чувство..."
];

let memoryIndex = 0;
setInterval(() => {
    const memoryDiv = document.getElementById('memoryFloat');
    if (memoryDiv) {
        memoryDiv.textContent = memories[memoryIndex % memories.length];
        memoryIndex++;
    }
}, 8000);
let forgetElements = document.querySelectorAll('p, li, .req-card');
setInterval(() => {
    if (Math.random() > 0.7) {
        const randomElement = forgetElements[Math.floor(Math.random() * forgetElements.length)];
        randomElement.style.transition = 'opacity 2s';
        randomElement.style.opacity = '0.2';
        setTimeout(() => {
            randomElement.style.opacity = '1';
        }, 3000);
    }
}, 15000);
const symbols = ['📷', '🕰️', '🔑', '💭', '📜', '👤', '🏠', '💔', '❓'];
setInterval(() => {
    const container = document.getElementById('fallingMemories');
    if (container) {
        const item = document.createElement('div');
        item.className = 'falling-item';
        item.textContent = symbols[Math.floor(Math.random() * symbols.length)];
        item.style.left = Math.random() * 100 + '%';
        item.style.animationDuration = 4 + Math.random() * 5 + 's';
        item.style.fontSize = 16 + Math.random() * 30 + 'px';
        container.appendChild(item);
        setTimeout(() => item.remove(), 8000);
    }
}, 2000);

   
const voices = [
    "Кто ты?",
    "Это не твой дом...",
    "Вспомни моё имя...",
    "Ты обещал не забывать...",
    "Почему ты уходишь?",
    "Посмотри на фото...",
    "Я здесь, рядом...",
    "Не закрывай глаза..."
];

function showVoice() {
    const voiceDiv = document.getElementById('voiceMessage');
    if (voiceDiv && Math.random() > 0.85) {
        voiceDiv.textContent = voices[Math.floor(Math.random() * voices.length)];
        voiceDiv.style.opacity = '1';
        setTimeout(() => voiceDiv.style.opacity = '0', 4000);
    }
}

setInterval(showVoice, 12000);
setInterval(() => {
    if (Math.random() > 0.9) {
        const halluc = document.getElementById('hallucination');
        halluc.classList.add('show');
        setTimeout(() => halluc.classList.remove('show'), 2000);
    }
}, 30000);
    </script>
    <div id="memoryFloat" class="memory-float">Кто я?...</div>
    <div id="fallingMemories"></div>
    
    <div id="voiceMessage" class="voice-message"></div>
    <div id="hallucination" class="hallucination"></div>
    <div class="moon"></div>
    
</body>
</html>

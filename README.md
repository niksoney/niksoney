<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🌟 Apresentação Incrível</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Exo+2:wght@300;400;600&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            font-family: 'Exo 2', sans-serif;
            min-height: 100vh;
            overflow-x: hidden;
            color: white;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
            position: relative;
            z-index: 2;
        }
        
        .hero {
            text-align: center;
            padding: 4rem 0;
            position: relative;
        }
        
        .glitch {
            font-family: 'Orbitron', monospace;
            font-size: 4rem;
            font-weight: 900;
            text-transform: uppercase;
            position: relative;
            text-shadow: 0.05em 0 0 #00fffc, -0.03em -0.04em 0 #fc00ff,
                         0.025em 0.04em 0 #fffc00;
            animation: glitch 725ms infinite;
            margin-bottom: 1rem;
        }
        
        .glitch span {
            position: absolute;
            top: 0;
            left: 0;
        }
        
        .subtitle {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            opacity: 0.9;
            animation: fadeIn 2s ease-in;
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 1.5rem;
            margin: 3rem 0;
        }
        
        .tech-item {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            padding: 1.5rem;
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .tech-item:hover {
            transform: translateY(-10px) scale(1.05);
            background: rgba(255, 255, 255, 0.2);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4);
        }
        
        .tech-icon {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }
        
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        .pulse {
            animation: pulse 2s infinite;
        }
        
        .stats {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin: 2rem 0;
            flex-wrap: wrap;
        }
        
        .stat-item {
            text-align: center;
            padding: 1rem 2rem;
        }
        
        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }
        
        .neon-btn {
            background: transparent;
            border: 2px solid #00fffc;
            color: #00fffc;
            padding: 12px 30px;
            font-size: 1.1rem;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            margin: 0.5rem;
            font-family: 'Orbitron', monospace;
        }
        
        .neon-btn:hover {
            background: #00fffc;
            color: #0f0c29;
            box-shadow: 0 0 20px #00fffc;
        }
        
        @keyframes glitch {
            0% {
                text-shadow: 0.05em 0 0 #00fffc, -0.03em -0.04em 0 #fc00ff,
                             0.025em 0.04em 0 #fffc00;
            }
            15% {
                text-shadow: 0.05em 0 0 #00fffc, -0.03em -0.04em 0 #fc00ff,
                             0.025em 0.04em 0 #fffc00;
            }
            16% {
                text-shadow: -0.05em -0.025em 0 #00fffc, 0.025em 0.035em 0 #fc00ff,
                             -0.05em -0.05em 0 #fffc00;
            }
            49% {
                text-shadow: -0.05em -0.025em 0 #00fffc, 0.025em 0.035em 0 #fc00ff,
                             -0.05em -0.05em 0 #fffc00;
            }
            50% {
                text-shadow: 0.05em 0.035em 0 #00fffc, 0.03em 0 0 #fc00ff,
                             0 -0.04em 0 #fffc00;
            }
            99% {
                text-shadow: 0.05em 0.035em 0 #00fffc, 0.03em 0 0 #fc00ff,
                             0 -0.04em 0 #fffc00;
            }
            100% {
                text-shadow: -0.05em 0 0 #00fffc, -0.025em -0.04em 0 #fc00ff,
                             -0.04em -0.025em 0 #fffc00;
            }
        }
        
        @keyframes floating {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @media (max-width: 768px) {
            .glitch {
                font-size: 2.5rem;
            }
            
            .tech-grid {
                grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            }
        }
    </style>
</head>
<body>
    <div class="particles" id="particles"></div>
    
    <div class="container">
        <div class="hero">
            <h1 class="glitch" data-text="SEU NOME">SEU NOME</h1>
            <p class="subtitle">🚀 Desenvolvedor Full-Stack & Inovador Digital</p>
            
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number" id="projectsCount">0</div>
                    <div>Projetos Concluídos</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number" id="experienceYears">0</div>
                    <div>Anos de Experiência</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number" id="coffeeCups">0</div>
                    <div>Xícaras de Café</div>
                </div>
            </div>
            
            <div style="margin: 2rem 0;">
                <a href="#contact" class="neon-btn pulse">📧 Entrar em Contato</a>
                <a href="#projects" class="neon-btn">💼 Ver Projetos</a>
            </div>
        </div>
        
        <div class="tech-grid">
            <div class="tech-item floating" style="animation-delay: 0s;">
                <div class="tech-icon">⚛️</div>
                <div>React</div>
            </div>
            <div class="tech-item floating" style="animation-delay: 0.2s;">
                <div class="tech-icon">🐍</div>
                <div>Python</div>
            </div>
            <div class="tech-item floating" style="animation-delay: 0.4s;">
                <div class="tech-icon">🚀</div>
                <div>Node.js</div>
            </div>
            <div class="tech-item floating" style="animation-delay: 0.6s;">
                <div class="tech-icon">📱</div>
                <div>Flutter</div>
            </div>
            <div class="tech-item floating" style="animation-delay: 0.8s;">
                <div class="tech-icon">☁️</div>
                <div>AWS</div>
            </div>
            <div class="tech-item floating" style="animation-delay: 1s;">
                <div class="tech-icon">🤖</div>
                <div>AI/ML</div>
            </div>
        </div>
    </div>

    <script>
        // Partículas de fundo
        function createParticles() {
            const particles = document.getElementById('particles');
            const particleCount = 50;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.style.position = 'absolute';
                particle.style.width = Math.random() * 5 + 2 + 'px';
                particle.style.height = particle.style.width;
                particle.style.background = `hsl(${Math.random() * 360}, 100%, 70%)`;
                particle.style.borderRadius = '50%';
                particle.style.left = Math.random() * 100 + 'vw';
                particle.style.top = Math.random() * 100 + 'vh';
                particle.style.opacity = Math.random() * 0.7 + 0.3;
                particle.style.animation = `floating ${Math.random() * 6 + 4}s ease-in-out infinite`;
                particle.style.animationDelay = Math.random() * 5 + 's';
                
                particles.appendChild(particle);
            }
        }
        
        // Animação de contagem
        function animateCounter(elementId, target, duration = 2000) {
            const element = document.getElementById(elementId);
            let start = 0;
            const increment = target / (duration / 16);
            
            const timer = setInterval(() => {
                start += increment;
                if (start >= target) {
                    element.textContent = target;
                    clearInterval(timer);
                } else {
                    element.textContent = Math.floor(start);
                }
            }, 16);
        }
        
        // Efeito de digitação
        function typeWriter(element, text, speed = 100) {
            let i = 0;
            element.innerHTML = '';
            
            function typing() {
                if (i < text.length) {
                    element.innerHTML += text.charAt(i);
                    i++;
                    setTimeout(typing, speed);
                }
            }
            typing();
        }
        
        // Inicialização
        document.addEventListener('DOMContentLoaded', function() {
            createParticles();
            
            // Animar contadores
            setTimeout(() => animateCounter('projectsCount', 42), 500);
            setTimeout(() => animateCounter('experienceYears', 3), 1000);
            setTimeout(() => animateCounter('coffeeCups', 999), 1500);
            
            // Efeito de cursor piscante
            const glitch = document.querySelector('.glitch');
            setInterval(() => {
                glitch.style.borderRight = '2px solid #00fffc';
                setTimeout(() => {
                    glitch.style.borderRight = '2px solid transparent';
                }, 500);
            }, 1000);
            
            // Efeito parallax suave
            document.addEventListener('mousemove', (e) => {
                const particles = document.querySelectorAll('.particles div');
                particles.forEach(particle => {
                    const speed = parseFloat(particle.style.width) * 0.5;
                    const x = (window.innerWidth - e.pageX * speed) / 100;
                    const y = (window.innerHeight - e.pageY * speed) / 100;
                    particle.style.transform = `translateX(${x}px) translateY(${y}px)`;
                });
            });
        });
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rapheal's Univese</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Poppins:wght@300;400;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #0f0f23 0%, #1a1a2e 25%, #16213e 50%, #0f0f23 75%, #1a1a2e 100%);
            background-size: 400% 400%;
            animation: gradientShift 8s ease infinite;
            color: #ffffff;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
            position: relative;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        /* Floating particles */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }
        
        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: radial-gradient(circle, #ff6b6b, #4ecdc4);
            border-radius: 50%;
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); opacity: 0.7; }
            50% { transform: translateY(-20px) rotate(180deg); opacity: 1; }
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 2;
        }
        
        /* Header Section */
        .header {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }
        
        .header::before {
            content: '';
            position: absolute;
            top: -20px;
            left: 50%;
            transform: translateX(-50%);
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(255, 107, 107, 0.3) 0%, rgba(78, 205, 196, 0.3) 50%, transparent 70%);
            border-radius: 50%;
            z-index: -1;
            animation: pulse 4s ease-in-out infinite;
        }
        
        @keyframes pulse {
            0%, 100% { transform: translateX(-50%) scale(1); opacity: 0.7; }
            50% { transform: translateX(-50%) scale(1.1); opacity: 1; }
        }
        
        .main-title {
            font-family: 'Orbitron', monospace;
            font-size: 3.5em;
            font-weight: 900;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4, #ffeaa7);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: rainbowText 3s ease-in-out infinite;
            margin-bottom: 10px;
            text-shadow: 0 0 30px rgba(255, 107, 107, 0.5);
        }
        
        @keyframes rainbowText {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }
        
        .subtitle {
            font-size: 1.5em;
            color: #4ecdc4;
            margin-bottom: 20px;
            animation: slideInFromBottom 1s ease-out;
        }
        
        @keyframes slideInFromBottom {
            from { transform: translateY(30px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        
        /* Profile Avatar */
        .profile-avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            padding: 4px;
            margin: 20px auto;
            animation: rotate 10s linear infinite;
            box-shadow: 0 0 40px rgba(255, 107, 107, 0.6);
        }
        
        .profile-avatar::before {
            content: '🎌';
            font-size: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: #1a1a2e;
            border-radius: 50%;
            width: 100%;
            height: 100%;
        }
        
        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        /* About Section */
        .about-section {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            padding: 30px;
            margin-bottom: 40px;
            animation: fadeInUp 1s ease-out;
            position: relative;
            overflow: hidden;
        }
        
        .about-section::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4);
            border-radius: 20px;
            z-index: -1;
            animation: borderGlow 3s ease-in-out infinite;
        }
        
        @keyframes borderGlow {
            0%, 100% { opacity: 0.5; }
            50% { opacity: 1; }
        }
        
        @keyframes fadeInUp {
            from { transform: translateY(30px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        
        .about-item {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            padding: 10px;
            border-radius: 10px;
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .about-item:hover {
            background: rgba(255, 255, 255, 0.1);
            transform: translateX(10px);
        }
        
        .about-item .icon {
            font-size: 24px;
            margin-right: 15px;
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }
        
        /* Social Links */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
            flex-wrap: wrap;
        }
        
        .social-btn {
            display: inline-flex;
            align-items: center;
            padding: 12px 24px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            border: none;
            border-radius: 25px;
            color: white;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.4);
            animation: socialFloat 4s ease-in-out infinite;
        }
        
        .social-btn:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 8px 25px rgba(255, 107, 107, 0.6);
        }
        
        @keyframes socialFloat {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-5px); }
        }
        
        /* Stats Section */
        .stats-section {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 40px 0;
        }
        
        .stat-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 20px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
            animation: cardFloat 6s ease-in-out infinite;
        }
        
        .stat-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 35px rgba(255, 107, 107, 0.3);
        }
        
        @keyframes cardFloat {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-8px); }
        }
        
        .stat-card img {
            border-radius: 10px;
            width: 100%;
            height: auto;
            transition: all 0.3s ease;
        }
        
        .stat-card:hover img {
            transform: scale(1.05);
        }
        
        /* Skills Section */
        .skills-section {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 30px;
            margin: 40px 0;
            text-align: center;
        }
        
        .skills-title {
            font-family: 'Orbitron', monospace;
            font-size: 2.5em;
            margin-bottom: 20px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .skills-grid {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 20px;
        }
        
        .skill-icon {
            width: 60px;
            height: 60px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            transition: all 0.3s ease;
            cursor: pointer;
            animation: skillPulse 3s ease-in-out infinite;
        }
        
        .skill-icon:hover {
            transform: scale(1.2) rotate(10deg);
            box-shadow: 0 10px 25px rgba(255, 107, 107, 0.5);
        }
        
        @keyframes skillPulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
        
        /* Projects Section */
        .projects-section {
            margin: 40px 0;
        }
        
        .section-title {
            font-family: 'Orbitron', monospace;
            font-size: 2.5em;
            text-align: center;
            margin-bottom: 30px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
        }
        
        .project-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 25px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
            cursor: pointer;
            animation: projectFloat 8s ease-in-out infinite;
        }
        
        .project-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 20px 40px rgba(255, 107, 107, 0.3);
        }
        
        @keyframes projectFloat {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-5px); }
        }
        
        .project-emoji {
            font-size: 2.5em;
            margin-bottom: 15px;
            animation: emojiSpin 4s ease-in-out infinite;
        }
        
        @keyframes emojiSpin {
            0%, 100% { transform: rotate(0deg); }
            50% { transform: rotate(15deg); }
        }
        
        .project-title {
            font-size: 1.3em;
            font-weight: 600;
            color: #4ecdc4;
            margin-bottom: 10px;
        }
        
        .project-description {
            color: #b0b0b0;
            margin-bottom: 10px;
        }
        
        .project-status {
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9em;
            font-weight: 600;
            display: inline-block;
        }
        
        /* Quote Section */
        .quote-section {
            text-align: center;
            margin: 40px 0;
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 30px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .quote-text {
            font-size: 1.3em;
            font-style: italic;
            color: #4ecdc4;
            margin-bottom: 15px;
            animation: quoteGlow 3s ease-in-out infinite;
        }
        
        @keyframes quoteGlow {
            0%, 100% { text-shadow: 0 0 10px rgba(78, 205, 196, 0.5); }
            50% { text-shadow: 0 0 20px rgba(78, 205, 196, 0.8); }
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .main-title {
                font-size: 2.5em;
            }
            
            .subtitle {
                font-size: 1.2em;
            }
            
            .social-links {
                flex-direction: column;
                align-items: center;
            }
            
            .stats-section {
                grid-template-columns: 1fr;
            }
            
            .projects-grid {
                grid-template-columns: 1fr;
            }
        }
        
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        
        ::-webkit-scrollbar-track {
            background: rgba(255, 255, 255, 0.1);
        }
        
        ::-webkit-scrollbar-thumb {
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            border-radius: 10px;
        }
        
        ::-webkit-scrollbar-thumb:hover {
            background: linear-gradient(45deg, #4ecdc4, #ff6b6b);
        }
        
        /* Loading Animation */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .container > * {
            animation: fadeIn 1s ease-out forwards;
        }
        
        .container > *:nth-child(1) { animation-delay: 0.1s; }
        .container > *:nth-child(2) { animation-delay: 0.2s; }
        .container > *:nth-child(3) { animation-delay: 0.3s; }
        .container > *:nth-child(4) { animation-delay: 0.4s; }
        .container > *:nth-child(5) { animation-delay: 0.5s; }
        .container > *:nth-child(6) { animation-delay: 0.6s; }
        .container > *:nth-child(7) { animation-delay: 0.7s; }
        .container > *:nth-child(8) { animation-delay: 0.8s; }
    </style>
</head>
<body>
    <div class="particles"></div>
    
    <div class="container">
        <!-- Header Section -->
        <div class="header">
            <div class="profile-avatar"></div>
            <h1 class="main-title">👋 Hey Everyone, I'm Rapheal</h1>
            <h3 class="subtitle">✨ Welcome to My GitHub Universe! ✨</h3>
        </div>
        
        <!-- About Section -->
        <div class="about-section">
            <div class="about-item">
                <span class="icon">💻</span>
                <span>Building AI-powered tools and educational platforms</span>
            </div>
            <div class="about-item">
                <span class="icon">🌱</span>
                <span>Focused on learning, teaching, and empowering communities</span>
            </div>
            <div class="about-item">
                <span class="icon">🚴</span>
                <span>Passionate about cycling, robotics, and technology for good</span>
            </div>
            <div class="about-item">
                <span class="icon">🌍</span>
                <span>Open to collaboration on AI, education, and environmental projects</span>
            </div>
            <div class="about-item">
                <span class="icon">📲</span>
                <span>Offering AI and software solutions for social impact</span>
            </div>
        </div>
        
        <!-- Social Links -->
        <div class="social-links">
            <a href="mailto:raphealasomanikwabena@gmail.com" class="social-btn">
                📧 Gmail
            </a>
            <a href="https://www.linkedin.com/in/younggem/" class="social-btn">
                💼 LinkedIn
            </a>
            <a href="https://twitter.com/your_handle_here" class="social-btn">
                🐦 Twitter
            </a>
            <a href="https://www.youtube.com/@your_channel_name" class="social-btn">
                🎬 YouTube
            </a>
        </div>
        
        <!-- Stats Section -->
        <div class="stats-section">
            <div class="stat-card">
                <h3 style="color: #4ecdc4; margin-bottom: 15px;">📊 GitHub Stats</h3>
                <img src="https://github-readme-stats.vercel.app/api?username=Rapheal-Kwabena&show_icons=true&theme=radical&hide_border=true" alt="GitHub Stats" />
            </div>
            
            <div class="stat-card">
                <h3 style="color: #4ecdc4; margin-bottom: 15px;">🔥 Streak Stats</h3>
                <img src="https://github-readme-streak-stats.herokuapp.com?user=Rapheal-Kwabena&theme=radical&hide_border=true" alt="Streak Stats" />
            </div>
            
            <div class="stat-card">
                <h3 style="color: #4ecdc4; margin-bottom: 15px;">💻 Top Languages</h3>
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rapheal-Kwabena&layout=compact&theme=radical&hide_border=true" alt="Top Languages" />
            </div>
            
            <div class="stat-card">
                <h3 style="color: #4ecdc4; margin-bottom: 15px;">🏆 Trophies</h3>
                <img src="https://github-profile-trophy.vercel.app/?username=Rapheal-Kwabena&theme=radical&row=1&no-frame=true" alt="Trophies" />
            </div>
        </div>
        
        <!-- Skills Section -->
        <div class="skills-section">
            <h2 class="skills-title">💡 Languages & Tools</h2>
            <div class="skills-grid">
                <div class="skill-icon" title="Python">🐍</div>
                <div class="skill-icon" title="JavaScript">⚡</div>
                <div class="skill-icon" title="HTML">🌐</div>
                <div class="skill-icon" title="CSS">🎨</div>
                <div class="skill-icon" title="React">⚛️</div>
                <div class="skill-icon" title="Tailwind">🎯</div>
                <div class="skill-icon" title="Arduino">🔧</div>
                <div class="skill-icon" title="Figma">🎭</div>
                <div class="skill-icon" title="AI/ML">🤖</div>
                <div class="skill-icon" title="Node.js">💚</div>
                <div class="skill-icon" title="Git">📝</div>
                <div class="skill-icon" title="Docker">🐳</div>
            </div>
        </div>
        
        <!-- Projects Section -->
        <div class="projects-section">
            <h2 class="section-title">🌟 Featured Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-emoji">🎧</div>
                    <h3 class="project-title">Audiobook Summary Platform</h3>
                    <p class="project-description">Transform long audiobooks into AI-powered summaries with intelligent analysis and key insights extraction.</p>
                    <span class="project-status">🚧 In Development</span>
                </div>
                
                <div class="project-card">
                    <div class="project-emoji">🌿</div>
                    <h3 class="project-title">Environmental AI Chatbot</h3>
                    <p class="project-description">Advanced AI system that analyzes environmental images and provides comprehensive insights for sustainability.</p>
                    <span class="project-status">🔄 In Transition</span>
                </div>
                
                <div class="project-card">
                    <div class="project-emoji">🏫</div>
                    <h3 class="project-title">Edu Learn Quiz Platform</h3>
                    <p class="project-description">Interactive learning platform with dynamic quizzes, progress tracking, and personalized educational experiences.</p>
                    <span class="project-status">⚡ Active Development</span>
                </div>
            </div>
        </div>
        
        <!-- Contribution Graph -->
        <div class="stat-card" style="margin: 40px 0;">
            <h3 style="color: #4ecdc4; margin-bottom: 15px;">📈 Contribution Graph</h3>
            <img src="https://github-readme-activity-graph.vercel.app/graph?username=Rapheal-Kwabena&theme=github-compact&hide_border=true" alt="Contribution Graph" style="width: 100%; border-radius: 10px;" />
        </div>
        
        <!-- Quote Section -->
        <div class="quote-section">
            <div class="quote-text">
                "The best way to predict the future is to create it." 💫
            </div>
            <div style="color: #b0b0b0;">
                - Ready to build something amazing together? Let's connect! 🚀
            </div>
        </div>
    </div>
    
    <script>
        // Create floating particles
        function createParticles() {
            const particlesContainer = document.querySelector('.particles');
            const particleCount = 50;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                particle.style.left = Math.random() * 100 + '%';
                particle.style.top = Math.random() * 100 + '%';
                particle.style.animationDelay = Math.random() * 6 + 's';
                particle.style.animationDuration = (Math.random() * 3 + 3) + 's';
                
                // Random colors
                const colors = ['#ff6b6b', '#4ecdc4', '#45b7d1', '#96ceb4', '#ffeaa7'];
                const color = colors[Math.floor(Math.random() * colors.length)];
                particle.style.background = `radial-gradient(circle, ${color}, transparent)`;
                
                particlesContainer.appendChild(particle);
            }
        }
        
        // Initialize particles
        createParticles();
        
        // Add hover effects to project cards
        const projectCards = document.querySelectorAll('.project-card');
        projectCards.forEach(card => {
            card.addEventListener('mouseenter', () => {
                card.style.transform = 'translateY(-15px) scale(1.03)';
                card.style.boxShadow = '0 25px 50px rgba(255, 107, 107, 0.4)';
            });
            
            card.addEventListener('mouseleave', () => {
                card.style.transform = 'translateY(0) scale(1)';
                card.style.boxShadow = '0 5px 15px rgba(255, 107, 107, 0.2)';
            });
        });
        
        // Add click animation to skill icons
        const skillIcons = document.querySelectorAll('.skill-icon');
        skillIcons.forEach(icon => {
            icon.addEventListener('click', () => {
                icon.style.transform = 'scale(1.3) rotate(360deg)';
                icon.style.boxShadow = '0 15px 30px rgba(255, 107, 107, 0.6)';
                
                setTimeout(() => {
                    icon.style.transform = 'scale(1) rotate(0deg)';
                    icon.style.boxShadow = '0 5px 15px rgba(255, 107, 107, 0.3)';
                }, 300);
            });
        });
        
        // Add smooth scrolling animation
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const parallax = document.querySelector('.header::before');
            if (parallax) {
                parallax.style.transform = `translateY(${scrolled * 0.5}px)`;
            }
        });
        
        // Add typing effect to title
        const title = document.querySelector('.main-title');
        const originalText = title.textContent;
        title.textContent = '';
        
        let i = 0;
        function typeWriter() {
            if (i < originalText.length) {
                title.textContent += originalText.charAt(i);
                i++;
                setTimeout(typeWriter, 100);
            }
        }
        
        // Start typing effect after a short delay
        setTimeout(typeWriter, 500);
    </script>
</body>
</html>

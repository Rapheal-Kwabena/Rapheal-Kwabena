<!-- Rainbow Border Animation -->
<div align="center" style="
  position: relative;
  padding: 3px;
  border-radius: 16px;
  background: linear-gradient(45deg, 
    #ff0000, #ff7300, #fffb00, #48ff00, 
    #00ffd5, #002bff, #7a00ff, #ff00c8, #ff0000);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  margin-bottom: 2rem;
">
  <!-- Animated Typing Text with Gradient -->
  <div style="
    background: #0f0f15;
    border-radius: 13px;
    padding: 2rem 1rem;
  ">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=28&duration=4000&pause=500&color=FF7F50&center=true&vCenter=true&width=700&lines=✨+Hi+there!+I'm+Rapheal+Kwabena+Asomani+Gadoh;⚡+Full+Stack+Developer+%7C+AI+Innovator;🚀+Building+the+Future+with+Code+%F0%9F%92%BB;🎨+Pixel+Artist+%7C+Tech+Visionary+%F0%9F%8E%A8" alt="Animated typing text" />
  </div>
</div>

<style>
  @keyframes gradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }
</style>

<!-- Anime Profile Card with Neon Glow -->
<div align="center" style="
  position: relative;
  width: 90%;
  max-width: 800px;
  margin: 0 auto 3rem;
  padding: 2.5rem;
  border-radius: 20px;
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  box-shadow: 0 0 25px rgba(255, 105, 180, 0.6);
  border: 2px solid #ff69b4;
  overflow: hidden;
  animation: pulse 6s infinite alternate;
">
  <!-- Anime Glow Effect -->
  <div style="
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(
      45deg,
      transparent,
      rgba(255, 105, 180, 0.1),
      transparent
    );
    animation: shine 3s linear infinite;
  "></div>
  
  <h2 style="
    color: #ff69b4;
    font-size: 2rem;
    margin-bottom: 1.5rem;
    text-shadow: 0 0 10px rgba(255, 105, 180, 0.7);
    position: relative;
  ">
    <span style="
      position: absolute;
      left: -30px;
      animation: bounce 2s infinite;
    ">👨‍💻</span> About Me
  </h2>
  
  <div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5rem;
    color: #e0e0e0;
    font-size: 1.1rem;
    position: relative;
    z-index: 2;
  ">
    <div style="
      background: rgba(15, 15, 25, 0.7);
      padding: 1.2rem;
      border-radius: 12px;
      border-left: 3px solid #ff69b4;
      transition: transform 0.3s;
    ">💡 Passionate about AI-powered solutions and renewable energy tech</div>
    
    <div style="
      background: rgba(15, 15, 25, 0.7);
      padding: 1.2rem;
      border-radius: 12px;
      border-left: 3px solid #64ffda;
      transition: transform 0.3s;
    ">🛠️ Building AI environmental chatbot & audiobook platform</div>
    
    <div style="
      background: rgba(15, 15, 25, 0.7);
      padding: 1.2rem;
      border-radius: 12px;
      border-left: 3px solid #ff9e64;
      transition: transform 0.3s;
    ">🌍 Based in Ghana, collaborating globally</div>
    
    <div style="
      background: rgba(15, 15, 25, 0.7);
      padding: 1.2rem;
      border-radius: 12px;
      border-left: 3px solid #6495ff;
      transition: transform 0.3s;
    ">🚴‍♂️ Robotics enthusiast & cycling lover</div>
  </div>
</div>

<style>
  @keyframes pulse {
    0% { box-shadow: 0 0 25px rgba(255, 105, 180, 0.6); }
    50% { box-shadow: 0 0 35px rgba(100, 255, 218, 0.6); }
    100% { box-shadow: 0 0 25px rgba(255, 105, 180, 0.6); }
  }
  
  @keyframes shine {
    0% { transform: translateX(-100%) rotate(30deg); }
    100% { transform: translateX(100%) rotate(30deg); }
  }
  
  @keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
  }
  
  div[style*='border-left']:hover {
    transform: translateY(-5px) scale(1.02);
  }
</style>

<!-- Floating Tech Stack with Hover Effects -->
<div align="center" style="margin-bottom: 3rem;">
  <h2 style="
    color: #64ffda;
    font-size: 2rem;
    margin-bottom: 1.5rem;
    text-shadow: 0 0 10px rgba(100, 255, 218, 0.5);
    position: relative;
    display: inline-block;
  ">
    <span style="
      position: absolute;
      right: -40px;
      animation: float 3s ease-in-out infinite;
    ">🚀</span> Tech Stack & Tools
  </h2>
  
  <div style="
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
    max-width: 800px;
    margin: 0 auto;
  ">
    <!-- Each badge has unique animation -->
    <div style="
      position: relative;
      overflow: hidden;
      border-radius: 8px;
      transition: all 0.3s;
      animation: float 6s ease-in-out infinite;
    ">
      <img src="https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python" />
      <div style="
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(
          90deg,
          transparent,
          rgba(255,255,255,0.2),
          transparent
        );
        transform: translateX(-100%);
        animation: shine 2s infinite 0.5s;
      "></div>
    </div>
    
    <div style="
      position: relative;
      overflow: hidden;
      border-radius: 8px;
      transition: all 0.3s;
      animation: float 6s ease-in-out infinite 0.5s;
    ">
      <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" alt="JavaScript" />
      <div style="
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(
          90deg,
          transparent,
          rgba(255,255,255,0.2),
          transparent
        );
        transform: translateX(-100%);
        animation: shine 2s infinite 1s;
      "></div>
    </div>
    
    <!-- Additional tech badges with different animation delays -->
    <div style="animation-delay: 1s;">...</div>
    <div style="animation-delay: 1.5s;">...</div>
  </div>
</div>

<!-- Animated GitHub Stats Cards -->
<div align="center" style="
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  width: 90%;
  max-width: 900px;
  margin: 0 auto 3rem;
">
  <!-- Streak Stats with Particle Effect -->
  <div style="
    position: relative;
    overflow: hidden;
    border-radius: 15px;
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    box-shadow: 0 0 20px rgba(100, 255, 218, 0.3);
  ">
    <img src="https://github-readme-streak-stats.herokuapp.com?user=Rapheal-Kwabena&theme=radical&hide_border=true" alt="GitHub Streak" />
    <div style="
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      background: url('https://media.giphy.com/media/XgQUXvYavej9VvxQ6b/giphy.gif');
      background-size: cover;
      mix-blend-mode: screen;
      opacity: 0.15;
    "></div>
  </div>
  
  <!-- Language Stats with Floating Animation -->
  <div style="
    position: relative;
    overflow: hidden;
    border-radius: 15px;
    background: linear-gradient(135deg, #1a1a2e, #16213e);
    box-shadow: 0 0 20px rgba(255, 105, 180, 0.3);
    animation: float 6s ease-in-out infinite 1s;
  ">
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rapheal-Kwabena&layout=compact&theme=radical&hide_border=true" alt="Top Languages" />
  </div>
</div>

<!-- Project Cards with Anime Hover Effects -->
<div align="center" style="margin-bottom: 3rem;">
  <h2 style="
    color: #ff9e64;
    font-size: 2rem;
    margin-bottom: 1.5rem;
    text-shadow: 0 0 10px rgba(255, 158, 100, 0.5);
  ">
    <span style="
      display: inline-block;
      animation: spin 4s linear infinite;
    ">🌟</span> Featured Projects
  </h2>
  
  <div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    width: 90%;
    max-width: 900px;
    margin: 0 auto;
  ">
    <!-- Project 1 -->
    <a href="https://github.com/Rapheal-Kwabena/Audiobook-Summary-Website" style="
      position: relative;
      padding: 1.5rem;
      border-radius: 15px;
      background: linear-gradient(135deg, #1a1a2e, #16213e);
      box-shadow: 0 5px 15px rgba(255, 105, 180, 0.3);
      text-decoration: none;
      color: #e0e0e0;
      overflow: hidden;
      transition: all 0.4s;
      z-index: 1;
    ">
      <div style="
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(
          45deg,
          rgba(255,105,180,0.1),
          rgba(100,255,218,0.1)
        );
        z-index: -1;
        opacity: 0;
        transition: opacity 0.3s;
      "></div>
      
      <h3 style="
        color: #ff69b4;
        margin-bottom: 0.8rem;
        font-size: 1.4rem;
      ">🎧 Audiobook Summary Platform</h3>
      <p style="margin-bottom: 0.5rem;">AI-powered summaries of long audiobooks</p>
      <div style="
        display: flex;
        flex-wrap: wrap;
        gap: 0.5rem;
        margin-top: 1rem;
      ">
        <span style="
          background: rgba(255,105,180,0.2);
          padding: 0.3rem 0.6rem;
          border-radius: 20px;
          font-size: 0.8rem;
        ">AI</span>
        <span style="
          background: rgba(100,255,218,0.2);
          padding: 0.3rem 0.6rem;
          border-radius: 20px;
          font-size: 0.8rem;
        ">NLP</span>
      </div>
      
      <div style="
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 3px;
        background: linear-gradient(90deg, #ff69b4, #64ffda);
        transform: scaleX(0);
        transform-origin: left;
        transition: transform 0.4s;
      "></div>
    </a>
    
    <!-- Additional project cards -->
  </div>
</div>

<style>
  @keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }
  
  a[href*="github"]:hover {
    transform: translateY(-10px) scale(1.02);
    box-shadow: 0 15px 30px rgba(255, 105, 180, 0.4);
  }
  
  a[href*="github"]:hover div[style*="opacity: 0"] {
    opacity: 1;
  }
  
  a[href*="github"]:hover div[style*="scaleX(0)"] {
    transform: scaleX(1);
  }
</style>

<!-- Social Links with Interactive Effects -->
<div align="center" style="margin-bottom: 3rem;">
  <h2 style="
    color: #6495ff;
    font-size: 2rem;
    margin-bottom: 1.5rem;
    text-shadow: 0 0 10px rgba(100, 149, 255, 0.5);
  ">📬 Let's Connect</h2>
  
  <div style="
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
  ">
    <a href="https://www.linkedin.com/in/rapheal-kwabena-asomani-gadoh" style="
      position: relative;
      display: inline-block;
      transition: all 0.3s;
    ">
      <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
      <div style="
        position: absolute;
        bottom: -5px;
        left: 0;
        width: 100%;
        height: 2px;
        background: #0077B5;
        transform: scaleX(0);
        transition: transform 0.3s;
      "></div>
    </a>
    
    <a href="https://twitter.com/your_handle_here" style="
      position: relative;
      display: inline-block;
      transition: all 0.3s;
    ">
      <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter" />
      <div style="
        position: absolute;
        bottom: -5px;
        left: 0;
        width: 100%;
        height: 2px;
        background: #1DA1F2;
        transform: scaleX(0);
        transition: transform 0.3s;
      "></div>
    </a>
  </div>
</div>

<style>
  a[href*="linkedin"]:hover, 
  a[href*="twitter"]:hover {
    transform: translateY(-5px);
  }
  
  a[href*="linkedin"]:hover div, 
  a[href*="twitter"]:hover div {
    transform: scaleX(1);
  }
</style>

<!-- Animated Quote with Floating Particles -->
<div align="center" style="
  position: relative;
  width: 90%;
  max-width: 700px;
  margin: 0 auto;
  padding: 2rem;
  border-radius: 15px;
  background: linear-gradient(135deg, #1a1a2e, #16213e);
  box-shadow: 0 0 25px rgba(100, 149, 255, 0.4);
  overflow: hidden;
">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical" alt="Random quote" />
  
  <!-- Floating particles -->
  <div style="
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
  ">
    <div style="
      position: absolute;
      width: 5px;
      height: 5px;
      background: white;
      border-radius: 50%;
      opacity: 0.6;
      animation: floatParticle 15s linear infinite;
    "></div>
    <!-- Add more particles with different positions/delays -->
  </div>
</div>

<style>
  @keyframes floatParticle {
    0% {
      transform: translateY(0) translateX(0);
      opacity: 0;
    }
    10% {
      opacity: 0.6;
    }
    90% {
      opacity: 0.6;
    }
    100% {
      transform: translateY(-100px) translateX(50px);
      opacity: 0;
    }
  }
</style>

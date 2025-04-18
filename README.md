<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saket Atal ki Rachnayen</title>
  <!-- Google Fonts Integration -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&family=Raleway:wght@400;600;700&family=Playfair+Display:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary-color: #FF9933;
      --secondary-color: #138808;
      --text-color: #222;
      --background-light: #ffffff;
      --background-dark: #121212;
      --header-font: 'Playfair Display', serif;
      --body-font: 'Raleway', sans-serif;
      --menu-font: 'Poppins', sans-serif;
    }

    body {
      font-family: var(--body-font);
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom, var(--primary-color), var(--background-light));
      color: var(--text-color);
      transition: background-color 0.5s, color 0.5s;
      position: relative;
      min-height: 100vh;
      overflow-x: hidden;
    }

    body::before {
      content: "";
      background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="500" height="600" viewBox="0 0 500 600"><path d="M250,50 L350,200 L250,350 L150,200 Z" fill="%23138808" opacity="0.04"/><text x="140" y="260" font-family="Arial" font-size="40" font-weight="bold" fill="%23000080" opacity="0.05">INDIA</text></svg>');
      background-repeat: repeat;
      background-position: center;
      background-size: 300px;
      opacity: 0.15;
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      z-index: -1;
      pointer-events: none;
    }

    header {
      background: linear-gradient(135deg, #000080, #000000);
      color: white;
      padding: 2.5rem 2rem;
      text-align: center;
      z-index: 2;
      position: relative;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
      border-bottom: 3px solid var(--primary-color);
    }

    header h1 {
      font-family: var(--header-font);
      font-size: 3rem;
      margin: 0;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
      letter-spacing: 1px;
    }

    header p {
      font-style: italic;
      font-size: 1.3rem;
      margin-top: 0.5rem;
      font-weight: 300;
    }

    nav {
      position: absolute;
      top: 1.5rem;
      right: 1.5rem;
      z-index: 100;
    }

    .menu {
      display: none;
      background-color: rgba(255, 255, 255, 0.95);
      position: absolute;
      top: 3.5rem;
      right: 0;
      width: 350px;
      border: none;
      border-radius: 8px;
      z-index: 3;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
      overflow: hidden;
      animation: fadeIn 0.3s ease-in-out;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-10px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .menu a {
      display: block;
      padding: 14px 20px;
      color: #333;
      text-decoration: none;
      border-bottom: 1px solid rgba(0, 0, 0, 0.05);
      font-family: var(--menu-font);
      font-weight: 500;
      transition: all 0.2s ease;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
    }

    .menu a:hover {
      background-color: rgba(255, 153, 51, 0.1);
      padding-left: 25px;
      color: var(--primary-color);
    }

    .menu a:last-child {
      border-bottom: none;
    }

    .hamburger {
      font-size: 30px;
      cursor: pointer;
      background-color: rgba(255, 255, 255, 0.9);
      color: #000080;
      padding: 5px 15px;
      border-radius: 8px;
      box-shadow: 0 3px 8px rgba(0, 0, 0, 0.2);
      transition: all 0.3s ease;
    }

    .hamburger:hover {
      background-color: #fff;
      transform: scale(1.05);
    }

    .dark-mode {
      background: linear-gradient(to bottom, #000080, var(--background-dark));
      color: #f9f9f9;
    }

    .dark-mode .menu {
      background-color: rgba(30, 30, 30, 0.95);
    }

    .dark-mode .menu a {
      color: #f0f0f0;
      border-bottom: 1px solid rgba(255, 255, 255, 0.05);
    }

    .dark-mode .menu a:hover {
      background-color: rgba(255, 153, 51, 0.2);
    }

    .dark-mode .hamburger {
      background-color: rgba(30, 30, 30, 0.9);
      color: #f0f0f0;
    }

    .controls {
      position: fixed;
      bottom: 20px;
      left: 20px;
      background-color: rgba(255, 255, 255, 0.9);
      padding: 12px 16px;
      border-radius: 12px;
      display: flex;
      gap: 1.2rem;
      align-items: center;
      z-index: 4;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
      transition: all 0.3s ease;
    }

    .dark-mode .controls {
      background-color: rgba(30, 30, 30, 0.9);
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.4);
    }

    .controls button {
      background-color: var(--primary-color);
      color: white;
      border: none;
      padding: 8px 15px;
      border-radius: 6px;
      cursor: pointer;
      font-family: var(--body-font);
      font-weight: 600;
      transition: all 0.2s ease;
    }

    .controls button:hover {
      transform: translateY(-2px);
      box-shadow: 0 3px 8px rgba(0, 0, 0, 0.2);
    }

    .controls label {
      margin-right: 0.5rem;
      font-weight: 500;
    }

    .controls input[type="color"] {
      border: none;
      width: 35px;
      height: 35px;
      border-radius: 4px;
      cursor: pointer;
    }

    .main-content {
      padding: 2rem;
      position: relative;
      z-index: 1;
    }

    @media (max-width: 768px) {
      .menu {
        width: 280px;
      }
      
      header h1 {
        font-size: 2.2rem;
      }
      
      header p {
        font-size: 1.1rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Saket Atal ki Rachnayen</h1>
    <p>From the pen of Saket Atal</p>
  </header>
  
  <div class="main-content">
    <!-- Your page content will go here -->
  </div>
  
  <div class="controls">
    <button onclick="toggleTheme()">Light/Dark</button>
    <label for="textColor">Text Color:</label>
    <input type="color" id="textColor" onchange="changeTextColor(this.value)" />
  </div>
  
  <nav>
    <span class="hamburger" onclick="toggleMenu()">☰</span>
    <div class="menu" id="menu">
      <a href="index.html">Home</a>
      <a href="urdu-hindi-stories.html">क़लम से: कहानियाँ (Urdu & Hindi Stories)</a>
      <a href="urdu-hindi-poems.html">क़लम से: नज़्में और कविताएं (Urdu & Hindi Poems)</a>
      <a href="english-stories.html">From My Quill: Stories</a>
      <a href="english-poems.html">From My Quill: Poems</a>
      <a href="podcast.html">Podcast - Hind & Hindavi</a>
      <a href="video.html">Video Section - Kissa Jeevan Ka</a>
    </div>
  </nav>
  
  <script>
    // Hide any HTML tags that might be visible when page loads
    document.addEventListener('DOMContentLoaded', function() {
      // Ensure no HTML is visible to users
      const htmlElements = document.querySelectorAll('html, body, head, meta, script, style');
      htmlElements.forEach(element => {
        element.style.display = element.tagName === 'BODY' ? 'block' : 'none';
      });
    });

    function toggleMenu() {
      const menu = document.getElementById('menu');
      if (menu.style.display === 'block') {
        menu.style.opacity = '0';
        menu.style.transform = 'translateY(-10px)';
        setTimeout(() => {
          menu.style.display = 'none';
        }, 300);
      } else {
        menu.style.display = 'block';
        setTimeout(() => {
          menu.style.opacity = '1';
          menu.style.transform = 'translateY(0)';
        }, 10);
      }
    }

    function toggleTheme() {
      document.body.classList.toggle('dark-mode');
    }

    function changeTextColor(color) {
      document.body.style.color = color;
    }

    // Close menu when clicking outside
    document.addEventListener('click', function(event) {
      const menu = document.getElementById('menu');
      const hamburger = document.querySelector('.hamburger');
      
      if (menu.style.display === 'block' && 
          !menu.contains(event.target) && 
          event.target !== hamburger) {
        toggleMenu();
      }
    });
  </script>
</body>
</html>

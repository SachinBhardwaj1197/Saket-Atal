<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>साकेत अटल की रचनाएँ</title>
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
    }body {
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
}

.menu a:hover {
  background-color: rgba(255, 153, 51, 0.1);
  padding-left: 25px;
  color: var(--primary-color);
}

.hamburger {
  font-size: 30px;
  cursor: pointer;
  background-color: rgba(255, 255, 255, 0.9);
  color: #000080;
  padding: 5px 15px;
  border-radius: 8px;
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
}

.controls {
  position: fixed;
  bottom: 20px;
  left: 20px;
  background-color: rgba(255, 255, 255, 0.9);
  padding: 12px 16px;
  border-radius: 12px;
  display: flex;
  gap: 1rem;
  align-items: center;
  z-index: 4;
}

.controls label {
  font-weight: 500;
}

.main-content {
  padding: 2rem;
  position: relative;
  z-index: 1;
}

  </style>
</head>
<body>
  <header>
    <h1>साकेत अटल की रचनाएँ</h1>
    <p>From the pen of Saket Atal</p>
  </header>  <div class="main-content" id="main-content">
    <!-- Poem titles or content here -->
    <p>
गीत नया गाता हूँ

टूटे हुए तारों से फूटे बासंती स्वर
पत्थर की छाती मे उग आया नव अंकुर
झरे सब पीले पात
कोयल की कुहुक रात

प्राची मे अरुणिम की रेख देख पता हूँ
गीत नया गाता हूँ

टूटे हुए सपनों की कौन सुने सिसकी
अन्तर की चीर व्यथा पलको पर ठिठकी
हार नहीं मानूँगा,
रार नई ठानूँगा,

काल के कपाल पे लिखता मिटाता हूँ
गीत नया गाता हूँ ।
      - श्री अटल बिहारी वाजपेई जी</p>
  </div>  <div class="controls">
    <button onclick="toggleTheme()">Light/Dark</button>
    <label for="textColor">Text Color:</label>
    <input type="color" id="textColor" />
    <label for="fontSelector">Font:</label>
    <select id="fontSelector">
      <option value="Raleway">Raleway</option>
      <option value="Poppins">Poppins</option>
      <option value="Playfair Display">Playfair Display</option>
    </select>
  </div>  <nav>
    <span class="hamburger" onclick="toggleMenu()">☰</span>
    <div class="menu" id="menu">
      <a href="index.html">Home</a>
      <a href="urdu-hindi-stories.html">क़लम से: कहानियाँ</a>
      <a href="urdu-hindi-poems.html">क़लम से: नज़्में और कविताएं</a>
      <a href="english-stories.html">From My Quill: Stories</a>
      <a href="english-poems.html">From My Quill: Poems</a>
      <a href="podcast.html">Podcast - Hind & Hindavi</a>
      <a href="video.html">Video Section - Kissa Jeevan Ka</a>
      <a href="#" onclick="alert('Mobile: 7070946811\nEmail: sachinbhardwaj.sb05@gmail.com')">Contact Us</a>
    </div>
  </nav>  <footer style="text-align: center; padding: 1rem; font-size: 0.9rem; background-color: #f1f1f1;">
    © 2025 Saket Atal. All rights reserved.
  </footer>  <script>
    function toggleMenu() {
      const menu = document.getElementById('menu');
      menu.style.display = menu.style.display === 'block' ? 'none' : 'block';
    }

    function toggleTheme() {
      document.body.classList.toggle('dark-mode');
    }

    const colorPicker = document.getElementById('textColor');
    const mainContent = document.getElementById('main-content');

    colorPicker.addEventListener('input', function () {
      mainContent.style.color = this.value;
    });

    const fontSelector = document.getElementById('fontSelector');
    fontSelector.addEventListener('change', function () {
      mainContent.style.fontFamily = this.value;
    });
  </script></body>

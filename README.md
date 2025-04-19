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
}

.menu a:hover {
  background-color: rgba(255, 153, 51, 0.1);
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
  gap: 1rem;
  align-items: center;
  z-index: 4;
}

.dark-mode .controls {
  background-color: rgba(30, 30, 30, 0.9);
}

.controls input, .controls select {
  border: none;
  border-radius: 6px;
  padding: 6px;
  font-family: var(--body-font);
}

.main-content {
  padding: 2rem;
  position: relative;
  z-index: 1;
}

.contact-modal {
  display: none;
  position: fixed;
  z-index: 999;
  left: 0; top: 0; width: 100%; height: 100%;
  background-color: rgba(0, 0, 0, 0.6);
}

.contact-content {
  background-color: #fff;
  margin: 10% auto;
  padding: 2rem;
  border-radius: 10px;
  width: 90%;
  max-width: 400px;
  text-align: center;
}

.contact-content button {
  margin-top: 1rem;
  padding: 0.5rem 1.2rem;
  background-color: var(--primary-color);
  color: #fff;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

.dark-mode .contact-content {
  background-color: #222;
  color: #eee;
}

footer {
  text-align: center;
  padding: 1rem;
  background-color: #f0f0f0;
  font-size: 0.9rem;
  color: #444;
}

  </style>
</head>
<body>
  <header>
    <h1>साकेत अटल की रचनाएँ</h1>
    <p>From the pen of Saket Atal</p>
  </header>  <nav>
    <span class="hamburger" onclick="toggleMenu()">☰</span>
    <div class="menu" id="menu">
      <a href="index.html">Home</a>
      <a href="urdu-hindi-stories.html">क़लम से: कहानियाँ</a>
      <a href="urdu-hindi-poems.html">क़लम से: नज़्में और कविताएं</a>
      <a href="english-stories.html">From My Quill: Stories</a>
      <a href="english-poems.html">From My Quill: Poems</a>
      <a href="podcast.html">Podcast - Hind & Hindavi</a>
      <a href="video.html">Video Section - Kissa Jeevan Ka</a>
      <a href="#" onclick="showContact()">Contact Us</a>
    </div>
  </nav>  <div class="main-content">
    <!-- Your content goes here -->
  </div>  <div class="controls">
    <button onclick="toggleTheme()">Light/Dark</button>
    <label for="textColor">Text:</label>
    <input type="color" id="textColor" onchange="changeTextColor(this.value)"><label for="fontSelect">Font:</label>
<select id="fontSelect" onchange="changeFont(this.value)">
  <option value="Raleway">Raleway</option>
  <option value="Poppins">Poppins</option>
  <option value="Playfair Display">Playfair Display</option>
  <option value="Georgia">Georgia</option>
  <option value="Times New Roman">Times New Roman</option>
</select>

  </div>  <div id="contactModal" class="contact-modal">
    <div class="contact-content">
      <h3>Contact Us</h3>
      <p><strong>Mobile:</strong> 7070946811</p>
      <p><strong>Email:</strong> sachinbhardwaj.sb05@gmail.com</p>
      <button onclick="closeContact()">Close</button>
    </div>
  </div>  <footer>
    &copy; 2025 Saket Atal. All rights reserved.
  </footer>  <script>
    function toggleMenu() {
      const menu = document.getElementById('menu');
      menu.style.display = menu.style.display === 'block' ? 'none' : 'block';
    }

    function toggleTheme() {
      document.body.classList.toggle('dark-mode');
    }

    function changeTextColor(color) {
      document.body.style.color = color;
    }

    function changeFont(fontName) {
      document.body.style.fontFamily = fontName;
    }

    function showContact() {
      document.getElementById('contactModal').style.display = 'block';
    }

    function closeContact() {
      document.getElementById('contactModal').style.display = 'none';
    }
  </script></body>

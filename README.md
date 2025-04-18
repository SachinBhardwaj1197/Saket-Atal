<!DOCTYPE html><html lang="en"><head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saket Atal's Rachnayen</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: var(--bg);
      color: var(--text);
      transition: background-color 0.3s, color 0.3s;
    }:root {
  --bg: #ffffff;
  --text: #000000;
}

.dark-mode {
  --bg: #121212;
  --text: #ffffff;
}

header {
  padding: 1rem;
  background-color: #333;
  color: white;
  text-align: center;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.5rem 1rem;
  background-color: #444;
  color: white;
}

nav .menu {
  font-size: 1.5rem;
  cursor: pointer;
}

nav .theme-toggle {
  cursor: pointer;
}

.nav-links {
  display: none;
  flex-direction: column;
  background-color: #555;
  padding: 1rem;
}

.nav-links a {
  color: white;
  text-decoration: none;
  margin: 0.5rem 0;
}

.section {
  padding: 2rem;
}

h2 {
  margin-top: 0;
}

footer {
  background: #333;
  color: white;
  padding: 1rem;
  text-align: center;
}

.story, .poem {
  margin-top: 1rem;
  padding: 1rem;
  border-left: 3px solid #888;
  background-color: #f4f4f4;
}

  </style>
</head><body>
  <header>
    <h1>From the Pen of Saket Atal</h1>
    <p>A curated collection of emotions, reflections, and creativity in multiple languages and formats.</p>
  </header>  <nav>
    <div class="menu" onclick="toggleNav()">&#9776;</div>
    <div class="theme-toggle" onclick="toggleTheme()">Toggle Light/Dark</div>
  </nav>
  <div class="nav-links" id="navLinks">
    <a href="#kalam-urdu">क़लम से - Urdu/Hindi</a>
    <a href="#kalam-english">Kalam Se - English</a>
    <a href="#podcast">Hind & Hindavi Podcast</a>
    <a href="#video">Kissa Jeevan Ka (Video)</a>
  </div>  <div class="section" id="kalam-urdu">
    <h2>क़लम से (उर्दू / हिंदी)</h2>
    <p>"शब्दों में संवेदनाएँ, भावनाओं में कहानियाँ — यह अनुभाग है आपकी आत्मा को छू जाने वाली रचनाओं का। यहाँ आपको मिलेंगी उर्दू और हिंदी में दिल को छूने वाली कहानियाँ और नज़्में।"</p>
    <div class="story">
      <h3>कहानी का शीर्षक (placeholder)</h3>
      <p>यहाँ आपकी हिंदी/उर्दू कहानी प्रदर्शित होगी...</p>
    </div>
    <div class="poem">
      <h3>नज़्म / कविता (placeholder)</h3>
      <p>यहाँ आपकी कविता या नज़्म प्रदर्शित होगी...</p>
    </div>
  </div>  <div class="section" id="kalam-english">
    <h2>Kalam Se (English)</h2>
    <p>"Thoughts take flight in the language of the mind. This section is home to reflective stories and lyrical poems in English — simple yet profound narratives."</p>
    <div class="story">
      <h3>Story Title (placeholder)</h3>
      <p>Your English story will appear here...</p>
    </div>
    <div class="poem">
      <h3>Poem Title (placeholder)</h3>
      <p>Your English poem will appear here...</p>
    </div>
  </div>  <div class="section" id="podcast">
    <h2>Hind & Hindavi Podcast</h2>
    <p>"Echoes of language, literature, and life — the Hind & Hindavi Podcast is a deep dive into rich cultural roots through sound. Tune in and immerse yourself in meaningful conversations and stories."</p>
    <p><strong>Podcast episodes coming soon...</strong></p>
  </div>  <div class="section" id="video">
    <h2>Kissa Jeevan Ka (Video)</h2>
    <p>"Every life is a story, every story is a window into a soul. 'Kissa Jeevan Ka' brings you life’s narratives in moving pictures — poignant, real, and thought-provoking."</p>
    <p><strong>Videos will be featured here soon...</strong></p>
  </div>  <footer>
    <p>&copy; 2025 Saket Atal (Dr. Sachin Bhardwaj). All rights reserved.</p>
  </footer>  <script>
    function toggleNav() {
      const navLinks = document.getElementById("navLinks");
      navLinks.style.display = navLinks.style.display === "flex" ? "none" : "flex";
    }

    function toggleTheme() {
      document.body.classList.toggle("dark-mode");
    }
  </script></body></html>

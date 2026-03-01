<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Omwandho Graphic Lab</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
<style>
/* Base & Reset */
* { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Montserrat', sans-serif; }
body { background: #0f0f0f; color: #fff; line-height: 1.6; scroll-behavior: smooth; }
a { text-decoration: none; color: inherit; }
img { max-width: 100%; display: block; }

/* Header */
header { display:flex; justify-content: space-between; align-items:center; padding:20px 50px; background:#111; position: fixed; width:100%; z-index:1000;}
header h1 { font-size: 1.8rem; color: #00ffff; }
nav a { margin-left: 20px; font-weight:600; transition:0.3s; }
nav a:hover { color: #ff00ff; }

/* Hero Section */
.hero { height:100vh; display:flex; flex-direction: column; justify-content:center; align-items:center; text-align:center; background: linear-gradient(135deg,#0f0f0f,#1a1a1a);}
.logo3d { font-size: 4rem; font-weight: 900; color: #00ffff; text-shadow: 0 0 10px #00ffff, 0 0 20px #ff00ff, 0 0 30px #ff00ff; animation: spin 10s linear infinite; }
@keyframes spin { 0% { transform: rotateY(0deg); } 100% { transform: rotateY(360deg); } }
.hero h2 { font-size:2rem; margin-top:20px; color:#fff; }
.hero .cta { display:flex; gap:20px; margin-top:20px;}
.cta a { padding:12px 30px; border:2px solid #00ffff; color:#00ffff; font-weight:600; border-radius:5px; transition:0.3s;}
.cta a:hover { background:#00ffff; color:#111; }

/* Sections */
section { padding:100px 50px; }
section h2 { font-size:2.5rem; margin-bottom:40px; text-align:center; color:#ff00ff; }

/* About */
.about { display:flex; flex-wrap:wrap; gap:40px; align-items:center; justify-content:center; }
.about img { border-radius:10px; width:300px; }
.about .text { max-width:600px; }
.about .skills { margin-top:20px; }
.skill { margin-bottom:15px; }
.skill-name { margin-bottom:5px; font-weight:600; }
.skill-bar { width:100%; height:10px; background:#333; border-radius:5px; }
.skill-bar-fill { height:100%; background:#00ffff; border-radius:5px; width:0; transition:1s; }

/* Portfolio */
.portfolio-filters { text-align:center; margin-bottom:40px; }
.portfolio-filters button { padding:10px 20px; margin:0 10px; border:2px solid #ff00ff; background:transparent; color:#ff00ff; font-weight:600; cursor:pointer; border-radius:5px; transition:0.3s;}
.portfolio-filters button:hover, .portfolio-filters button.active { background:#ff00ff; color:#111; }
.portfolio-grid { display:grid; grid-template-columns: repeat(auto-fit, minmax(250px,1fr)); gap:20px; }
.portfolio-item { position:relative; cursor:pointer; overflow:hidden; border-radius:10px; }
.portfolio-item img { transition:0.5s; }
.portfolio-item:hover img { transform: scale(1.1); }
.portfolio-item .overlay { position:absolute; top:0; left:0; width:100%; height:100%; background:rgba(0,0,0,0.7); display:flex; justify-content:center; align-items:center; opacity:0; transition:0.5s; color:#fff; font-weight:600; font-size:1.2rem; text-align:center; padding:20px; }
.portfolio-item:hover .overlay { opacity:1; }

/* Services */
.services-grid { display:grid; grid-template-columns: repeat(auto-fit, minmax(250px,1fr)); gap:30px; }
.service { background:#111; padding:30px; border-radius:10px; text-align:center; transition:0.3s; }
.service:hover { background:#222; }
.service h3 { margin-bottom:15px; color:#00ffff; }
.service p { color:#fff; }

/* Contact */
.contact-form { max-width:600px; margin:0 auto; display:flex; flex-direction:column; gap:20px; }
.contact-form input, .contact-form textarea, .contact-form select { padding:12px; border-radius:5px; border:none; outline:none; font-size:1rem; }
.contact-form button { padding:12px; background:#ff00ff; border:none; color:#111; font-weight:600; cursor:pointer; transition:0.3s; border-radius:5px; }
.contact-form button:hover { background:#00ffff; color:#111; }

/* Footer */
footer { text-align:center; padding:30px 20px; background:#111; color:#fff; }
footer a { color:#00ffff; margin:0 10px; font-weight:600; transition:0.3s;}
footer a:hover { color:#ff00ff; }

/* Responsive */
@media(max-width:768px) {
  header { flex-direction:column; gap:10px; }
  .about { flex-direction:column; }
  .hero .logo3d { font-size:3rem; }
  .hero h2 { font-size:1.8rem; }
}
</style>
</head>
<body>

<!-- Header -->
<header>
  <h1>Omwandho Graphic Lab</h1>
  <nav>
    <a href="#about">About</a>
    <a href="#portfolio">Portfolio</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<!-- Hero -->
<section class="hero">
  <div class="logo3d">OGL</div>
  <h2>Turning Ideas into Stunning Visuals</h2>
  <div class="cta">
    <a href="#portfolio">View Portfolio</a>
    <a href="#contact">Get a Quote</a>
  </div>
</section>

<!-- About -->
<section id="about">
  <h2>About Me</h2>
  <div class="about">
    <img src="https://via.placeholder.com/300x400.png?text=Your+Photo" alt="Peter Omwandho">
    <div class="text">
      <p>Hi, I’m Peter Omwandho, founder of <strong>Omwandho Graphic Lab</strong>. I specialize in stunning 2D & 3D logos, posters, branding, and social media visuals.</p>
      <div class="skills">
        <div class="skill">
          <div class="skill-name">Logo Design</div>
          <div class="skill-bar"><div class="skill-bar-fill" style="width:95%;"></div></div>
        </div>
        <div class="skill">
          <div class="skill-name">Branding</div>
          <div class="skill-bar"><div class="skill-bar-fill" style="width:90%;"></div></div>
        </div>
        <div class="skill">
          <div class="skill-name">Posters</div>
          <div class="skill-bar"><div class="skill-bar-fill" style="width:85%;"></div></div>
        </div>
        <div class="skill">
          <div class="skill-name">Animation</div>
          <div class="skill-bar"><div class="skill-bar-fill" style="width:80%;"></div></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Portfolio -->
<section id="portfolio">
  <h2>Portfolio</h2>
  <div class="portfolio-filters">
    <button class="active" onclick="filterPortfolio('all')">All</button>
    <button onclick="filterPortfolio('logo')">Logos</button>
    <button onclick="filterPortfolio('poster')">Posters</button>
    <button onclick="filterPortfolio('social')">Social Media</button>
    <button onclick="filterPortfolio('animation')">Animations</button>
  </div>
  <div class="portfolio-grid">
    <div class="portfolio-item" data-category="logo">
      <img src="https://via.placeholder.com/300x200.png?text=Logo+1" alt="Logo 1">
      <div class="overlay">Logo Project 1</div>
    </div>
    <div class="portfolio-item" data-category="poster">
      <img src="https://via.placeholder.com/300x200.png?text=Poster+1" alt="Poster 1">
      <div class="overlay">Poster Project 1</div>
    </div>
    <div class="portfolio-item" data-category="social">
      <img src="https://via.placeholder.com/300x200.png?text=Social+Media+1" alt="Social 1">
      <div class="overlay">Social Media Project 1</div>
    </div>
    <div class="portfolio-item" data-category="animation">
      <img src="https://via.placeholder.com/300x200.png?text=Animation+1" alt="Animation 1">
      <div class="overlay">Animation Project 1</div>
    </div>
  </div>
</section>

<!-- Services -->
<section id="services">
  <h2>Services</h2>
  <div class="services-grid">
    <div class="service">
      <h3>Logo Design</h3>
      <p>Custom 2D & 3D logos to represent your brand perfectly.</p>
    </div>
    <div class="service">
      <h3>Branding Packages</h3>
      <p>Complete branding including visual identity and strategy.</p>
    </div>
    <div class="service">
      <h3>Posters & Flyers</h3>
      <p>Creative promotional designs for events, products, or campaigns.</p>
    </div>
    <div class="service">
      <h3>Social Media Graphics</h3>
      <p>Eye-catching visuals for Instagram, TikTok, Facebook, and more.</p>
    </div>
    <div class="service">
      <h3>Animations</h3>
      <p>Dynamic 2D & 3D animations for marketing, social media, and branding.</p>
    </div>
  </div>
</section>

<!-- Contact -->
<section id="contact">
  <h2>Contact Me</h2>
  <form class="contact-form" action="#" method="POST">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <select name="service" required>
      <option value="">Select Service</option>
      <option value="logo">Logo Design</option>
      <option value="branding">Branding</option>
      <option value="poster">Posters</option>
      <option value="social">Social Media Graphics</option>
      <option value="animation">Animations</option>
    </select>
    <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
    <button type="submit">Send Message</button>
  </form>
  <p style="text-align:center; margin-top:20px;">Or chat directly via <a href="https://wa.me/254758560246" target="_blank">WhatsApp</a></p>
</section>

<!-- Footer -->
<footer>
  <p>© 2026 Omwandho Graphic Lab | Connect with me:</p>
  <a href="#">Facebook</a> | <a href="#">TikTok</a> | <a href="#">YouTube</a>
</footer>

<!-- JS for Portfolio Filtering -->
<script>
const buttons = document.querySelectorAll('.portfolio-filters button');
const items = document.querySelectorAll('.portfolio-item');
function filterPortfolio(category) {
  buttons.forEach(btn => btn.classList.remove('active'));
  event.target.classList.add('active');
  items.forEach(item => {
    if(category==='all'||item.dataset.category===category){item.style.display='block';}else{item.style.display='none';}
  });
}
</script>

</body>
</html>

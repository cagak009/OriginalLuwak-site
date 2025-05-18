# OriginalLuwak-site
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>OriginalLuwak.com - Authentic Premium Luwak Coffee</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,700;1,700&family=Roboto:wght@400;500&display=swap');

    /* Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Roboto', sans-serif;
      color: #4b382a;
      background: #f7f1e7;
      line-height: 1.6;
      scroll-behavior: smooth;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* Container */
    .container {
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 20px;
    }

    /* Header */
    header {
      background-color: #3e2f1c;
      color: #f7f1e7;
      padding: 20px 0;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
      box-shadow: 0 3px 10px rgba(0,0,0,0.3);
      font-weight: 500;
    }

    .header-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 20px;
    }

    .logo {
      font-family: 'Playfair Display', serif;
      font-size: 1.8rem;
      font-weight: 700;
      letter-spacing: 3px;
      text-transform: uppercase;
      color: #d4af37; /* Gold color */
      cursor: default;
    }

    nav a {
      margin-left: 25px;
      font-weight: 500;
      color: #f7f1e7;
      transition: color 0.3s ease;
      font-size: 1rem;
    }

    nav a:hover {
      color: #d4af37;
    }

    /* Hero */
    .hero {
      background: url('https://images.unsplash.com/photo-1509042239860-f550ce710b93?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80') center center/cover no-repeat;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      position: relative;
      padding-top: 80px; /* header height */
      text-align: center;
      color: #f7f1e7;
    }

    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background: rgba(62, 47, 28, 0.65);
      z-index: 0;
    }

    .hero-content {
      position: relative;
      z-index: 1;
      max-width: 800px;
      padding: 0 20px;
    }

    .hero-content h1 {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 3.6rem;
      margin-bottom: 20px;
      text-transform: uppercase;
      letter-spacing: 5px;
      text-shadow: 2px 2px 5px rgba(0,0,0,0.7);
    }

    .hero-content p {
      font-size: 1.4rem;
      margin-bottom: 35px;
      font-weight: 400;
      font-style: italic;
      text-shadow: 1px 1px 4px rgba(0,0,0,0.6);
    }

    .btn-primary {
      background-color: #d4af37;
      color: #3e2f1c;
      border: none;
      padding: 15px 40px;
      font-size: 1.2rem;
      font-weight: 700;
      border-radius: 50px;
      cursor: pointer;
      box-shadow: 0 5px 15px rgba(212, 175, 55, 0.7);
      transition: background-color 0.3s ease;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      user-select: none;
    }

    .btn-primary:hover {
      background-color: #b8992c;
      box-shadow: 0 5px 20px rgba(184, 153, 44, 0.9);
    }

    /* Sections */
    section {
      padding: 80px 0;
    }

    section:nth-child(even) {
      background-color: #e6dccf;
    }

    h2.section-title {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 2.8rem;
      text-align: center;
      color: #3e2f1c;
      margin-bottom: 40px;
      text-transform: uppercase;
      letter-spacing: 3px;
    }

    .about-content,
    .features-content {
      max-width: 900px;
      margin: 0 auto;
      font-size: 1.15rem;
      color: #4b382a;
      line-height: 1.8;
      text-align: center;
      font-weight: 400;
    }

    /* Feature cards */
    .features-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      margin-top: 30px;
      gap: 25px;
    }

    .feature-card {
      background: #f7f1e7;
      border-radius: 20px;
      padding: 25px;
      flex: 1 1 250px;
      min-width: 250px;
      max-width: 320px;
      box-shadow: 0 5px 15px rgba(62, 47, 28, 0.15);
      display: flex;
      flex-direction: column;
      align-items: center;
      transition: box-shadow 0.3s ease;
    }

    .feature-card:hover {
      box-shadow: 0 8px 20px rgba(212, 175, 55, 0.5);
    }

    .feature-icon {
      font-size: 3.2rem;
      color: #d4af37;
      margin-bottom: 15px;
    }

    .feature-title {
      font-weight: 700;
      font-size: 1.3rem;
      margin-bottom: 10px;
      text-transform: uppercase;
      color: #3e2f1c;
      letter-spacing: 1.5px;
      text-align: center;
    }

    .feature-desc {
      font-size: 1rem;
      color: #6a5843;
      text-align: center;
    }

    /* Contact Section */
    .contact-btn-wrapper {
      text-align: center;
      margin-top: 25px;
    }

    /* Footer */
    footer {
      background-color: #3e2f1c;
      color: #f7f1e7;
      text-align: center;
      padding: 20px 10px;
      font-size: 0.9rem;
      user-select: none;
      margin-top: 30px;
    }

    /* Responsive */
    @media (max-width: 768px){
      .features-list {
        flex-direction: column;
        align-items: center;
      }

      .hero-content h1 {
        font-size: 2.8rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="header-container">
      <div class="logo" aria-label="Original Luwak Coffee Logo">OriginalLuwak</div>
      <nav aria-label="Primary navigation">
        <a href="#about">About</a>
        <a href="#features">Features</a>
        <a href="#contact">Order</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero" role="banner" aria-label="Premium Luwak coffee hero section">
      <div class="hero-content">
        <h1>Authentic Premium Luwak Coffee</h1>
        <p>Experience the rare and exquisite taste of naturally processed Kopi Luwak from Indonesia.</p>
        <button class="btn-primary" onclick="scrollToSection('contact')">Order Now</button>
      </div>
    </section>

    <section id="about" aria-labelledby="about-title">
      <h2 class="section-title" id="about-title">About Original Luwak</h2>
      <div class="about-content">
        Original Luwak coffee is one of the rarest and most sought-after coffees globally. Sourced from the wild civet-processed coffee beans, it undergoes a unique natural fermentation that gives it an extraordinary smooth and rich flavor. Our carefully harvested beans come directly from Indonesia's lush coffee plantations, delivering an authentic experience to coffee connoisseurs everywhere.
      </div>
    </section>

    <section id="features" aria-labelledby="features-title">
      <h2 class="section-title" id="features-title">Why Choose Original Luwak?</h2>
      <div class="container features-list">
        <article class="feature-card" tabindex="0">
          <div class="feature-icon" aria-hidden="true">☕</div>
          <div class="feature-title">Unique Flavor</div>
          <p class="feature-desc">A naturally fermented coffee with smooth, rich, and complex flavor notes, unlike any other coffee.</p>
        </article>
        <article class="feature-card" tabindex="0">
          <div class="feature-icon" aria-hidden="true">🌱</div>
          <div class="feature-title">100% Natural</div>
          <p class="feature-desc">Sustainably harvested with great respect for nature and tradition, ensuring top quality beans.</p>
        </article>
        <article class="feature-card" tabindex="0">
          <div class="feature-icon" aria-hidden="true">⭐</div>
          <div class="feature-title">Premium Quality</div>
          <p class="feature-desc">Handpicked and roasted to perfection to bring out the aroma and vibrant cup character.</p>
        </article>
      </div>
    </section>

    <section id="contact" aria-labelledby="contact-title">
      <h2 class="section-title" id="contact-title">Place Your Order</h2>
      <div class="contact-btn-wrapper">
        <button class="btn-primary" onclick="alert('Thank you for your interest! Please contact us at order@originalluwak.com')">Contact Us</button>
      </div>
    </section>
  </main>

  <footer>
    &copy; 2024 OriginalLuwak.com — All Rights Reserved &nbsp; | &nbsp; Crafted with ☕ and ❤️
  </footer>

  <script>
    function scrollToSection(id) {
      const el = document.getElementById(id);
      if(el){
        el.scrollIntoView({behavior: 'smooth'});
      }
    }
  </script>
</body>
</html>


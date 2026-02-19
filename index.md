---
layout: home
title: " "
---

<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
body {
  font-family: 'Space Grotesk', sans-serif;
  background: radial-gradient(circle at 20% 30%, #1e293b, #0b1120 60%);
  color: #e2e8f0;
  margin: 0;
  overflow-x: hidden;
}

/* HERO SECTION */
.hero {
  height: 90vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.hero img {
  width: 150px;
  border-radius: 50%;
  margin-bottom: 25px;
  border: 2px solid #38bdf8;
  box-shadow: 0 0 25px rgba(56,189,248,0.5);
}

.hero h1 {
  font-size: 60px;
  margin: 0;
  background: linear-gradient(90deg, #38bdf8, #6366f1);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.hero h2 {
  font-weight: 300;
  margin-top: 15px;
  color: #94a3b8;
}

.btn {
  margin: 20px 10px;
  padding: 12px 24px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  border: 1px solid #38bdf8;
  color: #38bdf8;
  transition: all 0.3s ease;
}

.btn:hover {
  background: #38bdf8;
  color: #0b1120;
  box-shadow: 0 0 15px #38bdf8;
}

/* SECTIONS */
.section {
  padding: 80px 12%;
  max-width: 1000px;
  margin: auto;
}

.section h3 {
  font-size: 32px;
  margin-bottom: 25px;
  border-left: 3px solid #38bdf8;
  padding-left: 15px;
}

.section p {
  line-height: 1.8;
  color: #cbd5e1;
}

/* RESEARCH CARDS */
.card-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 25px;
  margin-top: 40px;
}

.card {
  padding: 25px;
  border: 1px solid rgba(56,189,248,0.3);
  border-radius: 12px;
  transition: all 0.3s ease;
  background: rgba(15,23,42,0.6);
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 0 20px rgba(56,189,248,0.4);
  border-color: #38bdf8;
}
</style>

<section class="hero">
  <img src="/assets/1.jpg" alt="Sayantan">
  <h1>Sayantan Bhattacharya</h1>
  <h2>X-ray Astronomy • Black Holes • Computational Astrophysics</h2>
  <div>
    <a class="btn" href="/research">Explore Research</a>
    <a class="btn" href="/about">About Me</a>
  </div>
</section>

<section class="section">
  <h3>About</h3>
  <p>
    I am a physicist exploring the high-energy universe through X-ray observations,
    compact objects, and advanced computational techniques. My research focuses on
    understanding extreme astrophysical environments and the physics driving them.
  </p>
</section>

<section class="section">
  <h3>Research Areas</h3>
  <div class="card-container">
    <div class="card">
      <h4>X-ray Astronomy</h4>
      <p>Investigating high-energy emissions from compact and massive stellar systems.</p>
    </div>
    <div class="card">
      <h4>Black Hole Systems</h4>
      <p>Studying accretion processes and variability in black hole environments.</p>
    </div>
    <div class="card">
      <h4>Massive Stars</h4>
      <p>Understanding stellar evolution and feedback in extreme conditions.</p>
    </div>
    <div class="card">
      <h4>Computational Methods</h4>
      <p>Applying data-driven techniques to astrophysical datasets.</p>
    </div>
  </div>
</section>

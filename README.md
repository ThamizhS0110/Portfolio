# Ex01 Portfolio
## Date:22.01.2026

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM

### index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Thamizh | Portfolio</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Navbar -->
  <header>
    <h1 class="logo">Thamizh</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#tech">Tech Stack</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div class="hero-content">
        <div class="hero-text">
          <div class="hero-image">
            <img src="image.png" alt="Profile Picture">
          </div>
        <h2>Hello, I'm <span>Thamizh</span></h2>
        <p>Designer | Full Stack Developer | MERN Enthusiast</p>
        <p class="tagline">Building ideas into real-world digital products</p>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="section">
    <h2>About Me</h2>
    <p>
      I am a passionate college student focused on design, development, and digital creativity.
      I specialize in building clean UI, scalable applications, and modern web solutions.
      My goal is to create impactful digital products and grow as a full-stack developer.
    </p>
  </section>

  <!-- Skills Section -->
  <section id="skills" class="section light">
    <h2>Core Skills</h2>

    <div class="skill-box">
      <h3>Design</h3>
      <div class="skills">
        <span>UI/UX Design</span>
        <span>Canva</span>
        <span>Figma</span>
        <span>Wireframing</span>
        <span>Prototyping</span>
      </div>
    </div>

    <div class="skill-box">
      <h3>Frontend</h3>
      <div class="skills">
        <span>HTML</span>
        <span>CSS</span>
        <span>JavaScript</span>
        <span>React.js</span>
        <span>Responsive Design</span>
      </div>
    </div>

    <div class="skill-box">
      <h3>Backend</h3>
      <div class="skills">
        <span>Node.js</span>
        <span>Express.js</span>
        <span>REST APIs</span>
        <span>Authentication</span>
      </div>
    </div>

  </section>

  <!-- Tech Stack Section -->
  <section id="tech" class="section">
    <h2>Tech Stack</h2>
    <div class="stack">
      <span>MongoDB</span>
      <span>Express.js</span>
      <span>React.js</span>
      <span>Node.js</span>
      <span>Git & GitHub</span>
      <span>JWT Auth</span>
      <span>API Integration</span>
      <span>Cloud Basics</span>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="section light">
    <h2>Contact Me</h2>
    <p>Email: thamizh@email.com</p>
    <p>Location: India</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2026 Thamizh(212224040350) | Built using HTML & CSS</p>
  </footer>

</body>
</html>

```
###style.css
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Segoe UI", sans-serif;
}

body {
  background: #0b0b0b;
  color: #ffffff;
  line-height: 1.6;
}

/* Navbar */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 10%;
  background: #0f0f0f;
  position: sticky;
  top: 0;
  z-index: 100;
}

.logo {
  color: #ff3c3c;
  font-size: 1.6rem;
}

nav a {
  margin-left: 25px;
  text-decoration: none;
  color: #fff;
  font-weight: 500;
  transition: 0.3s;
}

nav a:hover {
  color: #ff3c3c;
}

/* Hero */
.hero {
  height: 90vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.hero h2 {
  font-size: 3.2rem;
}

.hero span {
  color: #ff3c3c;
}

.hero p {
  margin-top: 10px;
  font-size: 1.2rem;
  opacity: 0.85;
}

.tagline {
  margin-top: 8px;
  font-size: 1rem;
  opacity: 0.6;
}

.hero-image img {
  border-radius: 20px;
  width: 250px;
  height: 250px;
  object-fit: cover;
}

/* Sections */
.section {
  padding: 80px 10%;
  text-align: center;
}

.section h2 {
  font-size: 2.3rem;
  margin-bottom: 25px;
  color: #ff3c3c;
}

.section p {
  max-width: 800px;
  margin: auto;
  opacity: 0.85;
}

.light {
  background: #131313;
}

/* Skills */
.skill-box {
  margin-bottom: 40px;
}

.skill-box h3 {
  margin-bottom: 15px;
  color: #fff;
  font-size: 1.3rem;
}

.skills, .stack {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px;
}

.skills span {
  background: #1f1f1f;
  border: 1px solid #ff3c3c;
  color: #fff;
  padding: 10px 18px;
  border-radius: 25px;
  font-size: 0.9rem;
  transition: 0.3s;
}

.skills span:hover {
  background: #ff3c3c;
  transform: translateY(-3px);
}

/* Tech Stack */
.stack span {
  background: #1f1f1f;
  border: 1px solid #ff3c3c;
  color: #fff;
  padding: 10px 18px;
  border-radius: 25px;
  font-size: 0.9rem;
  transition: 0.3s;
}

.stack span:hover {
   background: #ff3c3c;
  transform: translateY(-3px);
}

.mern {
  border: 1px solid #ff3c3c !important;
  color: #ff3c3c;
  font-weight: 600;
}

/* Footer */
footer {
  background: #0f0f0f;
  padding: 20px;
  text-align: center;
  font-size: 0.9rem;
  opacity: 0.6;
}

```
## OUTPUT
<img width="1886" height="970" alt="image" src="https://github.com/user-attachments/assets/82b42e46-5f6b-40ff-b7d4-bcdaa57bc1b2" />
<img width="1896" height="976" alt="image" src="https://github.com/user-attachments/assets/79417ba2-95d2-44de-8465-03517895cbc2" />
<img width="1843" height="959" alt="image" src="https://github.com/user-attachments/assets/34115de3-c005-45ea-bca2-9d8eb0696318" />



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.

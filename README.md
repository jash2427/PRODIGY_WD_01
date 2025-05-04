# PRODIGY_WD_01
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Prodigy InfoTech</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
    }

    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background-color: transparent;
      color: white;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      transition: background-color 0.3s, color 0.3s;
      z-index: 1000;
    }

    nav.scrolled {
      background-color: #333;
      color: #fff;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    .brand-title {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .nav-links {
      display: flex;
      gap: 1rem;
    }

    nav a {
      text-decoration: none;
      color: inherit;
      padding: 0.5rem 1rem;
      transition: background-color 0.3s, color 0.3s;
    }

    nav a:hover {
      background-color: #fff;
      color: #333;
      border-radius: 4px;
    }

    section {
      padding: 100px 20px 80px;
      margin-top: 60px;
      height: auto;
      position: relative;
    }

    /* Sticky + Animated section heading in left corner */
    .section-heading {
      position: absolute;
      top: 20px;
      left: 20px;
      font-size: 1.5rem;
      color: #444;
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 1px;
      z-index: 500;
      opacity: 0;
      transform: translateY(-10px);
      transition: opacity 0.6s ease, transform 0.6s ease;
    }

    .section-heading.visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* Animation styles for section content */
    .fade-in {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.6s ease, transform 0.6s ease;
    }

    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* Section specific styles */
    #home {
      background: linear-gradient(to right, #4facfe, #00f2fe);
      color: white;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
    }

    #home h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
    }

    #home p {
      font-size: 1.5rem;
      max-width: 700px;
    }

    #about {
      background-color: #d7f0f4;
      text-align: center;
    }

    #about h1 {
      font-size: 2.5rem;
      margin-top: 40px;
      margin-bottom: 1rem;
      color: #333;
    }

    #about p {
      font-size: 1.2rem;
      max-width: 800px;
      margin: 0 auto;
      color: #444;
      line-height: 1.6;
    }

    /* Services Section with a distinct background color */
    #services {
      background-color: #f8d7da; /* Light red background */
      text-align: center;
    }

    #services h1 {
      font-size: 2rem;
      margin-top: 40px;
      color: #333;
    }

    #services p {
      font-size: 1.2rem;
      color: #444;
    }

    /* Contact Section with a distinct background color */
    #contact {
      background-color: #d4edda; /* Light green background */
      text-align: center;
    }

    #contact h1 {
      font-size: 2rem;
      margin-top: 40px;
      color: #333;
    }

    #contact p {
      font-size: 1.2rem;
      color: #444;
    }

    /* Scroll to top button */
    #scrollToTop {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 50%;
      padding: 15px;
      font-size: 18px;
      cursor: pointer;
      display: none;
      z-index: 1000;
      transition: opacity 0.3s;
    }

    #scrollToTop:hover {
      background-color: #0056b3;
    }

    /* Footer Styles */
    footer {
      background-color: #333;
      color: white;
      padding: 20px;
      text-align: center;
    }

    footer a {
      color: #fff;
      text-decoration: none;
      margin: 0 10px;
      font-size: 20px;
    }

    footer a:hover {
      color: #007bff;
    }

  </style>
</head>
<body>

  <!-- Navigation Bar -->
  <nav id="navbar">
    <div class="brand-title">Prodigy InfoTech</div>
    <div class="nav-links">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <!-- Home Section -->
  <section id="home">
    <div class="section-heading">Home</div>
    <h1 class="fade-in">Prodigy InfoTech</h1>
    <p class="fade-in">Providing World Class E-Learning Experience with Real World Internships</p>
  </section>

  <!-- About Section -->
  <section id="about">
    <div class="section-heading">About Us</div>
    <h1 class="fade-in">Transforming the Way People Learn</h1>
    <p class="fade-in">
      Our mission is to create innovative and accessible learning solutions that empower people of all ages and backgrounds to achieve their full potential. Whether you're a student looking to improve your grades, a professional seeking to upskill, or an organization looking to enhance employee training, we have the tools and resources you need to succeed.
    </p>
  </section>

  <!-- Services Section -->
  <section id="services">
    <div class="section-heading">Services</div>
    <h1 class="fade-in"></h1>
    <p class="fade-in">We offer internships, online training, workshops, and career guidance in the tech industry.</p>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <div class="section-heading">Contact</div>
    <h1 class="fade-in">Let’s talk about

Love to hear from you!</h1>
    <p class="fade-in">Email us at: contact@prodigyinfotech.com</p>
  </section>

  <!-- Scroll to Top Button -->
  <button id="scrollToTop">&#8593;</button>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Prodigy InfoTech. All Rights Reserved.</p>
    <div>
      <a href="https://facebook.com" target="_blank">Facebook</a>
      <a href="https://twitter.com" target="_blank">Twitter</a>
      <a href="https://linkedin.com" target="_blank">LinkedIn</a>
    </div>
  </footer>

  <!-- JavaScript -->
  <script>
    const navbar = document.getElementById("navbar");

    // Scroll effect for navbar
    window.addEventListener("scroll", () => {
      if (window.scrollY > 50) {
        navbar.classList.add("scrolled");
      } else {
        navbar.classList.remove("scrolled");
      }

      // Scroll to top button visibility
      const scrollButton = document.getElementById("scrollToTop");
      if (window.scrollY > 300) {
        scrollButton.style.display = "block";
      } else {
        scrollButton.style.display = "none";
      }
    });

    // Scroll to top action
    document.getElementById("scrollToTop").addEventListener("click", () => {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    });

    // Intersection Observer for headings and fade-in content
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add("visible");
        }
      });
    }, {
      threshold: 0.1
    });

    // Observe headings and fade-in elements
    document.querySelectorAll(".section-heading, .fade-in").forEach(el => {
      observer.observe(el);
    });
  </script>

</body>
</html>

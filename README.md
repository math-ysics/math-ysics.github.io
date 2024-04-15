<html>
<head>
<style>
  /* General styles */
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: "Times New Roman", Times, serif;
    color: white; /* Setting default text color to white */
    line-height: 1.6;
    padding: 10px;
    background-image: url('https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/city.png');
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    backdrop-filter: blur(5px);
  }

  /* Specific background for content sections */
  main > header, main > section {
      background-color: rgba(255, 255, 255, 0.38);
      padding: 20px;
      border-radius: 10px;
      margin-top: 20px;
  }
  
  /* Flex container specific rules */
  div[style*="flex"] {
      background-color: transparent;
      padding: 7px;
  }
  
  main {
      background-color: transparent;
      padding: 10px;
      border-radius: 10px;
  }

  /* Header styles */
  h1, h2 {
      font-size: 24px;
      margin-top: 20px;
      margin-bottom: 5px;
      font-weight: bold;
      color: #d6336c; /* Changed to match the link color */
  }
  
  /* Custom header in the site's header section */
  header h1 {
      font-size: 32px;
      color: #d6336c; /* Ensuring consistency for all headers */
      margin-bottom: 10px;
      font-weight: bold;
  }

  /* Paragraph styles */
  p {
    font-size: 18px;
    font-style: italic;
    color: white; /* Ensuring paragraphs are white */
    margin-bottom: 10px;
  }

  /* Link styles */
  a {
    color: #d6336c; /* Pink color for links */
    text-decoration: none;
  }

  a:hover {
    text-decoration: underline;
  }

  img {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
  }

  @media (max-width: 768px) {
    h1, h2 {
      font-size: 22px;
    }

    p {
      font-size: 16px;
    }
  }

  /* Override styles for GitHub Pages or specific containers */
  .container-lg.px-3.my-5.markdown-body h1 a,
  .container-lg.px-3.my-5.markdown-body h1 a:visited {
    color: #333 !important;
    background-color: transparent !important;
    text-decoration: none !important;
    pointer-events: none;
    cursor: default;
  }

  .container-lg.px-3.my-5.markdown-body > h1:first-of-type {
    display: none !important;
  }

  /* Custom header in the site's header section */
  header h1 {
    font-size: 32px;
    color: #0056b3;
    margin-bottom: 10px;
    font-weight: bold;
  }
    /* New styles for purple images */
  .purple-images img {
    height: 200px; /* Set a fixed height for all purple images */
    width: auto; /* Adjust width automatically to maintain aspect ratio */
    object-fit: cover; /* Ensures the image covers the assigned area */
  }

  .fade-in {
      opacity: 0;
      transition: opacity 0.5s;
  }
  
  .appear {
      opacity: 1;
  }
</style>


</head>
<body>

<header>
  <h2>Hi, I'm Michael, an undergraduate student at the California Institute of Technology.</h2>
</header>
<main>
<section id="about">
  <h2>About Me</h2>
  <p>I'm interested in AI, statistics, theoretical astrophysics, and computational fluid dynamics.</p>
  <p>In research, I believe we should embody <a href="https://science.nasa.gov/mission/mer-opportunity/">opportunity</a>, <a href="https://mars.nasa.gov/msl/home/">curiosity</a>, and <a href="https://mars.nasa.gov/mars2020/">perseverance</a>.</p>
  <hr>
  <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/quote.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/quote.png" /></a>
  <hr>
  <p>Harmony of red and blue:</p>
  <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/graph.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/graph.png" /></a>
  <hr>
  <p>A beautiful set!</p>
  <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/mandelbrot%20set.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/mandelbrot%20set.png" /></a>
  <hr>
  <p>Have some purple:</p>
  <div style="display: flex;">
    <div style="display: flex;" class="purple-images">
        <div style="flex: 1;">
          <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple1.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple1.png" /></a>
        </div>
        <div style="flex: 1;">
          <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple2.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple2.png" /></a>
        </div>
        <div style="flex: 1;">
          <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple3.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple3.png" /></a>
        </div>
        <div style="flex: 1;">
          <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple4.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple4.png" /></a>
        </div>
    </div>
  </div>
</section>
</main>

<script>
document.addEventListener('DOMContentLoaded', function () {
    // Existing animations
    animateHeaders();
    addShadowToImages();
    fadeInOnScroll();

    // Enhanced Smooth Scrolling
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            const targetId = this.getAttribute('href');
            const targetPosition = document.querySelector(targetId).offsetTop;
            window.scrollTo({
                top: targetPosition - 10, // Adjusts to stop slightly before the section for a better view, if needed
                behavior: 'smooth'
            });
        });
    });

    // Tooltip Information
    document.querySelectorAll('[data-tooltip]').forEach(item => {
        item.addEventListener('mouseenter', () => {
            const tooltip = document.createElement('div');
            tooltip.textContent = item.getAttribute('data-tooltip');
            tooltip.className = 'tooltip';
            document.body.appendChild(tooltip);
            tooltip.style.top = `${item.offsetTop + item.offsetHeight}px`;
            tooltip.style.left = `${item.offsetLeft}px`;
        });
        item.addEventListener('mouseleave', () => {
            document.querySelector('.tooltip').remove();
        });
    });
});

function animateHeaders() {
    const headers = document.querySelectorAll('h1, h2');
    headers.forEach(header => {
        header.addEventListener('mouseenter', () => {
            header.style.transition = 'transform 0.3s';
            header.style.transform = 'scale(1.05)';
        });
        header.addEventListener('mouseleave', () => {
            header.style.transition = 'transform 0.3s';
            header.style.transform = 'scale(1)';
        });
    });
}

function addShadowToImages() {
    const images = document.querySelectorAll('img');
    images.forEach(img => {
        img.addEventListener('mouseenter', () => {
            img.style.transition = 'box-shadow 0.3s, transform 0.3s'; // Added transform to the transition
            img.style.boxShadow = '0 4px 8px rgba(0,0,0,0.5)';
            img.style.transform = 'scale(1.03)'; // Scale the image up
        });
        img.addEventListener('mouseleave', () => {
            img.style.transition = 'box-shadow 0.3s, transform 0.3s'; // Ensure the transition applies to transform as well
            img.style.boxShadow = 'none';
            img.style.transform = 'scale(1)'; // Scale back to normal
        });
    });
}

function fadeInOnScroll() {
    const faders = document.querySelectorAll('.fade-in');
    const appearOptions = {
        threshold: 0.5,
        rootMargin: "0px"
    };
    const appearOnScroll = new IntersectionObserver(function(
        entries,
        appearOnScroll
    ) {
        entries.forEach(entry => {
            if (!entry.isIntersecting) {
                return;
            } else {
                entry.target.classList.add('appear');
                appearOnScroll.unobserve(entry.target);
            }
        });
    }, appearOptions);

    faders.forEach(fader => {
        appearOnScroll.observe(fader);
    });
}
</script>


</body>
</html>

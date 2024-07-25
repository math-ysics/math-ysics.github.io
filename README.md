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
      color: white; /* Maintaining the default text color as white */
      line-height: 1.6;
      padding: 10px;
      background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/city.png');
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
      background-repeat: no-repeat; /* Ensure the background does not repeat */
      height: 100vh; /* Set the minimum height to 100% of the viewport height */
      min-height: 100%; /* Ensures minimum height is the full height of the content or viewport */
      width: 100vw; /* Cover the full viewport width */
      position: relative; /* Needed for fixed positioning context */
      overflow: auto; /* Allow scrolling on the page */
      backdrop-filter: blur(5px); /* Apply blur effect across the entire background */
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
      background-color: transparent; /* Keeping main content transparent */
      padding: 20px;
      border-radius: 10px;
      margin-top: 20px;
      position: relative; /* Positioned within the context of the body */
      z-index: 2; /* Ensure it is above the blurred background */
  }

  /* Header styles */
  h1, h2 {
      font-size: 24px;
      margin-top: 20px;
      margin-bottom: 5px;
      font-weight: bold;
      color: #eb3d44; /* Changed to match the link color */
  }
  
  /* Custom header in the site's header section */
  header h1 {
      font-size: 32px;
      color: #eb3d44; /* Ensuring consistency for all headers */
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
    color: #eb3d44; /* Pink color for links */
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

  .resized-centered-img {
    width: 55%; /* Resize to x% of the original width */
    display: block; /* Makes the image block level for margin auto to work */
    margin: 0 auto; /* Centers the image horizontally */
  }

  .quote-section {
      text-align: center;
      padding: 40px 20px;
      margin: 20px 0;
      background-color: rgba(255, 255, 255, 0.38);
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      min-height: 200px;
      transition: transform 0.3s ease; /* Add transition for smooth effect */
  }
  
  .quote-section q {
      font-size: 38px;
      color: #eb3d44;
      font-style: italic;
      font-weight: bold;
      display: block;
      margin: 0;
      line-height: 1.2;
      max-width: 80%;
      transition: transform 0.3s ease; /* Add transition for smooth effect */
  }

</style>


</head>
<body>

<header>
  <h2>Hi, I'm Michael, an undergraduate student at the California Institute of Technology.</h2>
</header>

<section class="quote-section">
  <q>Be stochastic.</q>
</section>

<main>
<section id="about">
  <h2>About Me</h2>
  <p>I'm interested in AI, statistics, theoretical astrophysics, and computational fluid dynamics.</p>
  <p>In research, I believe we should embody <a href="https://science.nasa.gov/mission/mer-opportunity/">opportunity</a>, <a href="https://mars.nasa.gov/msl/home/">curiosity</a>, and <a href="https://mars.nasa.gov/mars2020/">perseverance</a>.</p>
  <hr>
  <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/quote.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/quote.png" /></a>
  <!-- <hr>
  <p>Harmony of red and blue:</p>
  <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/graph.png">
    <img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/graph.png" class="resized-centered-img" />
  </a>
  <hr>
  <p>A beautiful set!</p>
  <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/mandelbrot%20set.png">
    <img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/mandelbrot%20set.png" class="resized-centered-img" />
  </a>
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
  </div> -->
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
    const elements = document.querySelectorAll('h1, h2, .quote-section');
    elements.forEach(element => {
        element.addEventListener('mouseenter', () => {
            element.style.transition = 'transform 0.3s';
            element.style.transform = 'scale(1.05)';
        });
        element.addEventListener('mouseleave', () => {
            element.style.transition = 'transform 0.3s';
            element.style.transform = 'scale(1)';
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

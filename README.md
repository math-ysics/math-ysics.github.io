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
      color: white;
      line-height: 1.6;
      padding: 10px;
      background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/city.png');
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
      background-repeat: no-repeat;
      min-height: 100vh; /* Changed from height: 100vh to min-height: 100vh */
      width: 100vw;
      position: relative;
      overflow-x: hidden; /* Prevent horizontal scrolling */
      overflow-y: auto; /* Allow vertical scrolling */
      backdrop-filter: blur(5px);
  }

  /* Add a pseudo-element to extend the blur effect */
  body::after {
      content: "";
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      z-index: -1;
      backdrop-filter: blur(5px);
  }

  /* Rest of the CSS remains unchanged */
  main > header, main > section {
      background-color: rgba(255, 255, 255, 0.38);
      padding: 20px;
      border-radius: 10px;
      margin-top: 20px;
  }
  
  div[style*="flex"] {
      background-color: transparent;
      padding: 7px;
  }
  
  main {
      background-color: transparent;
      padding: 20px;
      border-radius: 10px;
      margin-top: 20px;
      position: relative;
      z-index: 2;
  }

  h1, h2 {
      font-size: 24px;
      margin-top: 20px;
      margin-bottom: 5px;
      font-weight: bold;
      color: #eb3d44;
  }
  
  header h1 {
      font-size: 32px;
      color: #eb3d44;
      margin-bottom: 10px;
      font-weight: bold;
  }

  p {
    font-size: 18px;
    font-style: italic;
    color: white;
    margin-bottom: 10px;
  }

  a {
    color: #eb3d44;
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

  header h1 {
    font-size: 32px;
    color: #0056b3;
    margin-bottom: 10px;
    font-weight: bold;
  }

  .purple-images img {
    height: 200px;
    width: auto;
    object-fit: cover;
  }

  .fade-in {
      opacity: 0;
      transition: opacity 0.5s;
  }
  
  .appear {
      opacity: 1;
  }

  .resized-centered-img {
    width: 55%;
    display: block;
    margin: 0 auto;
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
      transition: transform 0.3s ease;
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
      transition: transform 0.3s ease;
  }

  .poem {
    font-style: italic;
    color: #eb3d44;
    margin-top: 20px;
    text-align: center;
    font-size: 18px;
    line-height: 1.6;
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
  <hr>
  <div class="poem">
    Upon the loom of eternal Chronos we entwine,<br>
    With each lambent scintilla our boundless phantasms shine.<br>
    <br>
    Through epoch nights and auroral reverie,<br>
    May the stars align this bimillenary.<br>
    <br>
    From hushed arcana of ancients erst exiled,<br>
    Thou hast erected vaults of grandeur vast;<br>
    In sanctified halls thusly shadows reconciled,<br>
    Erudition flourishes transcending mortal cast.<br>
    <br>
    In the symphony of sagacity divine,<br>
    And labyrinthine depths wherein enigmas quiesce;<br>
    A magnum opus by celestial designs,<br>
    Emerges from the cosmos' silent accresce.
  </div>
</section>
</main>

<script>
document.addEventListener('DOMContentLoaded', function () {
    animateHeaders();
    addShadowToImages();
    fadeInOnScroll();

    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            const targetId = this.getAttribute('href');
            const targetPosition = document.querySelector(targetId).offsetTop;
            window.scrollTo({
                top: targetPosition - 10,
                behavior: 'smooth'
            });
        });
    });

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
            img.style.transition = 'box-shadow 0.3s, transform 0.3s';
            img.style.boxShadow = '0 4px 8px rgba(0,0,0,0.5)';
            img.style.transform = 'scale(1.03)';
        });
        img.addEventListener('mouseleave', () => {
            img.style.transition = 'box-shadow 0.3s, transform 0.3s';
            img.style.boxShadow = 'none';
            img.style.transform = 'scale(1)';
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

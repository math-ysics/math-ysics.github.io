<html>
<head>
<style>
  /* Existing styles */
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: "Times New Roman", Times, serif;
    color: #333;
    line-height: 1.6;
    padding: 10px;
    // background-color: #f4f4f9;
    background-image: url('https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/city.png'); /* Add your desired background image URL here */
    background-size: cover;
    background-position: center;
    background-attachment: fixed; /* Optional: makes the background fixed during scrolling */
    backdrop-filter: blur(5px); /* Apply Gaussian blur to the background image */
  }

  /* Target only top-level sections under main for background styling */
  main > header, main > section {
      background-color: rgba(255, 255, 255, 0.55); /* White background with opacity */
      padding: 20px; /* Sufficient padding */
      border-radius: 10px; /* Rounded corners */
      margin-top: 20px; /* Top margin for spacing */
  }
  
  /* Specific styles for flex containers to avoid reapplying backgrounds */
  div[style*="flex"] {
      background-color: rgba(255, 255, 255, 0); /* Essentially no background to avoid double layer */
      padding: 6px;
  }
  
  /* Ensure the main tag itself does not add extra background beyond what its children have */
  main {
      background-color: rgba(255, 255, 255, 0); /* No background */
      padding: 10px;
      border-radius: 10px; /* Consistent rounded corners */
  }


  h1, h2 {
    font-weight: bold;
    color: #0056b3;
  }

  h1 {
    font-size: 24px;
    margin-top: 20px;
    margin-bottom: 5px;
  }

  h2 {
    font-size: 24px;
    margin-top: 20px;
    margin-bottom: 5px;
  }

  p {
    font-size: 18px;
    font-style: italic;
    color: #555;
    margin-bottom: 10px;
  }

  a {
    color: #d6336c;
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
    h1 {
      font-size: 28px;
    }

    h2 {
      font-size: 22px;
    }

    p {
      font-size: 16px;
    }
  }

  /* New style to override GitHub Pages theme styles */
  .container-lg.px-3.my-5.markdown-body h1 a,
  .container-lg.px-3.my-5.markdown-body h1 a:visited {
    color: #333 !important; /* Override text color */
    background-color: transparent !important; /* Remove any background */
    text-decoration: none !important; /* No underline */
    pointer-events: none; /* Disable it as a link */
    cursor: default;
  }

  /* Hide the theme's automatically generated header (if it is separate from your custom header) */
  .container-lg.px-3.my-5.markdown-body > h1:first-of-type {
    display: none !important;
  }

  /* Custom header styling */
  header h1 {
    font-size: 32px;
    color: #0056b3;
    margin-bottom: 10px;
    font-weight: bold;
  }
</style>

</head>
<body>

<header>
  <h1>Hi, I'm Michael, an undergraduate student at the California Institute of Technology.</h1>
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
  <p>Purple:</p>
  <div style="display: flex;">
    <div style="flex: 1;">
      <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple1.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple1.png" height="200" /></a>
    </div>
    <div style="flex: 1;">
      <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple2.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple2.png" height="200" /></a>
    </div>
    <div style="flex: 1;">
      <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple3.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple3.png" height="200" /></a>
    </div>
    <div style="flex: 1;">
      <a href="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple4.png"><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple4.png" height="200" /></a>
    </div>
  </div>
</section>
</main>

<script>
document.addEventListener('DOMContentLoaded', function () {
    // Function to animate headers on hover
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

    // Function to add shadow to images on hover
    const images = document.querySelectorAll('img');
    images.forEach(img => {
        img.addEventListener('mouseenter', () => {
            img.style.transition = 'box-shadow 0.3s';
            img.style.boxShadow = '0 4px 8px rgba(0,0,0,0.5)';
        });
        img.addEventListener('mouseleave', () => {
            img.style.transition = 'box-shadow 0.3s';
            img.style.boxShadow = 'none';
        });
    });
});
</script>

</body>
</html>

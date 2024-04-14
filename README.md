<html>
<head>

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
    color: white; /* Default text color set to white */
    line-height: 1.6;
    padding: 10px;
    background-image: url('https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/city.png');
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    backdrop-filter: blur(5px);
  }

  /* Specific styles for sections and headers */
  main > header, main > section {
      background-color: rgba(255, 255, 255, 0.55); /* Semi-transparent white background for general sections */
      padding: 20px;
      border-radius: 10px;
      margin-top: 20px;
  }

  /* New class for special header */
  .special-header {
    background-color: rgba(255, 255, 255, 0.8); /* More opaque white background */
    padding: 15px;
    border-radius: 10px;
    margin: 10px 0;
    text-align: center; /* Center the text */
  }

  h1, h2 {
    font-size: 24px;
    color: #0056b3; /* Blue color for headers */
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
    h1, h2 {
      font-size: 22px;
    }
    p {
      font-size: 16px;
    }
  }
</style>

</head>
<body>

<header class="special-header">
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

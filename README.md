<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
    <title>Michael's Personal Website</title>
    <style>
        img {
            max-width: 100%;
            height: auto;
        }
        .gallery img {
            margin-bottom: 1rem;
        }
        .gallery div {
            margin: 0.5rem;
        }
    </style>
</head>
<body>
    <header>
        <nav class="container-fluid">
            <ul>
                <li><strong>Michael's Portfolio</strong></li>
            </ul>
            <ul>
                <li><a href="#about">About Me</a></li>
                <li><a href="#research">Research</a></li>
                <li><a href="#gallery" role="button">Gallery</a></li>
            </ul>
        </nav>
    </header>
    <main class="container">
        <section>
            <hgroup>
                <h1>Hi, I'm Michael</h1>
                <h2>Undergraduate Student at Caltech</h2>
            </hgroup>
            <p>I'm interested in AI, statistics, theoretical astrophysics, and computational fluid dynamics.</p>
            <p>In research, I believe we should embody <a href="https://science.nasa.gov/mission/mer-opportunity/">opportunity</a>, <a href="https://mars.nasa.gov/msl/home/">curiosity</a>, and <a href="https://mars.nasa.gov/mars2020/">perseverance</a>.</p>
            <figure>
                <img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/quote.png" alt="Inspirational Quote"/>
                <figcaption>Harmony of red and blue</figcaption>
            </figure>
            <figure>
                <img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/graph.png" alt="Graph Image"/>
                <figcaption>A beautiful set!</figcaption>
            </figure>
            <figure>
                <img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/mandelbrot%20set.png" alt="Mandelbrot Set"/>
                <figcaption>Visualizing the Mandelbrot Set</figcaption>
            </figure>
            <h2>A Very Fine House (Avery House!):</h2>
            <div class="gallery" style="display: flex; flex-wrap: wrap; justify-content: space-around;">
                <div><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple1.png" alt="Avery House 1" /></div>
                <div><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple2.png" alt="Avery House 2" /></div>
                <div><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple3.png" alt="Avery House 3" /></div>
                <div><img src="https://raw.githubusercontent.com/math-ysics/math-ysics.github.io/main/docs/assets/images/purple4.png" alt="Avery House 4" /></div>
            </div>
        </section>
    </main>
    <footer class="container">
        <small><a href="https://avery.caltech.edu/">Visit Avery House</a> • <a href="#top">Back to top</a></small>
    </footer>
</body>
</html>

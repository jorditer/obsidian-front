```html
<body>
    <main> <!-- Encapsulates dominant content, not nav nor footer-->
        <header> <!-- Container for navigational links or introductory content-->
            <h3>Intro!</h3>
        </header>
        <section> <!-- Separates chapters, content with the same theme-->
            <article> <!-- standalone content -->
                <h3>Animales!</h3>
                <h4>Factos sobre los animales</h4>
                <aside>Bibliografia, comentarios, informacion adicional (not required, enhances another element)</aside>
            </article>
        </section>

    </main>
    <nav> <!-- Navigational links-->
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
        </ul>
    </nav>
    <figure> <!-- figure encapsulates media (images, illustrations, diagrams, code snippets, etc.) -->
        <img src="overwatch.jpg">
        <figcaption>This picture shows characters from Overwatch.</figcaption> <!-- figcaption describes an image-->
    </figure>
    <audio>
        <source src="iAmAnAudioFile.mp3" type="audio/mp3"> <!-- Audio -->
    </audio>
    <video src="coding.mp4" controls>Video not supported</video> <!-- Video not supported only appears if the video doesn't load -->
      
    <footer>
        <p>Contact info!</p> <!-- Copyright, Terms of use, Site map, reference to links, contact info-->
    </footer>

</body>
```
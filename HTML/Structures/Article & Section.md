A section separaters chapters, and englobes content with the same theme. Article is de division of the content within an article

The first element of an article should always be a heading.
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
</body>
```
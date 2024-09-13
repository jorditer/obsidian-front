## Header
Represents introductory content or navigational aids.
```html
<header>
  <a class="logo" href="#">Cute Puppies Express!</a>
  <img src="mdn-logo-sm.png" alt="MDN logo" />
</header>

<article>
  <header>
    <h1>Beagles</h1>
    <time>08.12.2014</time>
  </header>
  <p>I love beagles <em>so</em> much! Like, really, a lot. They’re adorable and their ears are so, so snugly soft!</p>
</article>
```
## Body
The actual content of the webpage
```html
<html lang="en">
  <head>
    <title>Document title</title>
  </head>
  <body>
    <p>
      The <code>&lt;body&gt;</code> HTML element represents the content of an
      HTML document. There can be only one <code>&lt;body&gt;</code> element in
      a document.
    </p>
  </body>
</html>
```
## Main
The dominant content of the body. Should be unique to the document, so there should be only one per page.
```html
<body>
  <a href="#main-content">Skip to main content</a>

  <!-- navigation and header content -->

  <main id="main-content">
    <!-- main page content -->
  </main>
</body>
```
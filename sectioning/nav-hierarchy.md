---
title: <nav> hierarchy
---
To do
Test cases to evaluate

## Code
```
  <body>
    <header>
      <p class="siteID">Site Identifier</p>
      <nav>
        <a href="#main">Skip to Main Content</a>
        <a rel="alternate" href="/es/this.html" hreflang="es">En Espanol</a>
        <a href="login.html">Log In</a>
      </nav>
    <header>
    <main id="main">

    </main>
    <nav>
      <h2>Site Map</h2>
      <a href="/fruit/">Fruit</a>
      <a href="/dairy/">Dairy</a>
      <a href="/vegetables/">Vegetables</a>
    </nav>
    <footer>
      <p><small>&copy; self</small></>
      <nav>
        <a rel="license" href="privacy.html">Privacy</a>
        <a href="about.html">About Us</a>
        <a href="contact.html">Contact Us</a>
      </nav>
    </footer>
  </body>
```

1. body > nav
2. body > header > nav
2. body > footer > nav
2. body > main > nav

## Expectation
The nav blocks play different roles relating to the part of the document.  Role of nav should be determned programmatically given standards compliant semantic structure.  Principles of use standards, semantic markup, and minize redundance conflicts with [ARIA Landmark guidance](ttps://www.w3.org/TR/wai-aria-practices/examples/landmarks/navigation.html)

Use of ```nav``` in header and footer blocks is intended to impress that these links are part of major site navigation.

* Site Nav. Hierarchical Navigation.  Typical for accessing a sites main sections, 'fat footer', 'site map', or Category
* Site Banner Nav.  Global utilities.  Typcial of site options link alternate language, log in, etc.
* Site Footer Nav.  Shared global resources.  Typical of links to legal content like privacy, terms, about, contact
* Main Nav.  Lateral navigation.  Typical for a table of contents menus used to access related resources, or SubCategory.


## Actual

## Discussion
Arguement is made to use only one ```nav``` per document.  The HTML5.2 notes it is "intended for major navigation blocks"


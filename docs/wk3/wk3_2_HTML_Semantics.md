# HTML Semantics

## Why Semantic HTML Elements ? 



**Semantic elements add meaning to the html tags** so that search engines, screen readers, and web browsers can make sense of it.



> Semantic html elements clearly describe their **purpose to both the browser and the developer**, allowing the information to be consumed in the correct format **according to the user**.

<br>

![page_talking](https://internetingishard.com/html-and-css/icons/social/semantic-markup-096a41.png ':size=400')


<p align="center"><a href="https://internetingishard.com/html-and-css/icons/social/semantic-markup-096a41.png"><em>Semantic HTML Tutorial</em></a> <em>- internetingishard.com</em></p>
You have already been using basic semantic elements:

- &lt;html>
- &lt;head>
- &lt;body>
- &lt;img>
- &lt;p>
- &lt;h1>, &lt;h2>, etc  

# Semantics: Page Structure



There are [many html semantic elements](https://learn-the-web.algonquindesign.ca/topics/html-semantics-cheat-sheet/) which are part of HTML5.

From here on, we will incorporate the following html elements into our sites:

- `<header>`
- `<nav>`
- `<article>`
- `<section>`
- `<aside>`
- `<footer>`
- `<figure>` and `<figcaption>`
- `<time>`
- `<address>`



Consider these commonly used website layouts:



<img src="https://internetingishard.com/html-and-css/semantic-html/html-sectioning-elements-00c3fd.png" style="width:300px;">

<p align="center"><a href="https://internetingishard.com/html-and-css/semantic-html/"><em>Semantic HTML</em></a> <em>- internetingishard.com</em></p>  

<br>

![HTML5 Semantic Elements](https://www.w3schools.com/html/img_sem_elements.gif)

<p align="center"><a href="https://www.w3schools.com/html/html5_semantic_elements.asp"><em>HTML Semantic Elements</em></a> <em>- w3schools.org</em></p>

<br>

**`<header>`**

Found at the top of a document, a section, or an article and  usually contains the main heading. It may some navigation and search tools.

```html
<header>
    <h1>My Amazing Company</h1>
</header>
```
<br>

**`<nav>`**

The navigation bar. Defines the navigation functionality for the page.

```html
<nav>
  <ul>
    <li><a href="/home">Home</a></li>
    <li><a href="/about">About</a></li>
    <li><a href="/contact">Contact us</a></li>
  </ul>
</nav>
```
<br>

**`<article>`**

 A block of related content that makes sense on its own without the rest of the page (e.g., a single blog post or a sales item in an e-commerce website).



**`<section>`**

 A thematic grouping of content that constitutes one single piece of functionality. (e.g., a set of article headlines, blog posts or summaries). Often used to group  `<article>` elements.

It's recommended to start a `<section>` with a heading.

```html
<section>
  <h2>Top Stories</h2>
    
  <section>
    <h3>News</h3>
    <article>Story 1</article>
    <article>Story 2</article>
    <article>Story 3</article>
  </section>
    
  <section>
    <h3>Sport</h3>
    <article>Story 1</article>
    <article>Story 2</article>
    <article>Story 3</article>
  </section>

</section>
```
<br>

**`<aside>`**

Defines content that is not directly related to the main content but can provide additional information indirectly related to it (glossary entries,  author biography, related links, etc.).

Should be related to the surrounding content.

<br>

**`<footer>`**

Generally found at the bottom of a document or section.  Typically contains the author of the document, copyright  information, links to terms of use, contact information, etc.

```html
 <footer>
  <p>Author: Mauricio Buschinelli</p>
  <p>Contact information: <a href="mailto:someone@example.com">
  someone@example.com</a>.</p>
</footer> 
```
<br>

**`<figure>`** and **`<figcaption>`**

Used together in order to add information or a visual explanation to an image. Wrap your image content around `<figure>` and use `<figcaption>` to add  captions. 

```html
<figure>
  <img src="pic_trulli.jpg" alt="Trulli">
  <figcaption>Fig1. - Trulli, Puglia, Italy.</figcaption>
</figure> 
```
<br>

**`<time>`**

Used to define a time and a date as human-readable text and machine-readable information.

*Code*

```html
<p>We open at <time>10:00</time> every morning.</p>

<p>I have a date on <time datetime="2008-02-14 20:00">Valentines day</time>.</p> 
```

*Result*

<div style="background-color: rgb(248, 248, 246)">
	<p>We open at <time>10:00</time> every morning.</p>
	<p>I have a date on <time datetime="2008-02-14 20:00">Valentines day</time>.</p>     
</div>
<br>


**`<address>`**

Defines contact information for the author of the article or web page. Should not be used for arbitrary physical addresses.

```html
<address>
	Please contact <a href='mailto:troymcclure@example.com'>Troy
	McClure</a> for questions about this article.
</address>
```
<br>

**`<main>`**

Specifies a big area in the center that contains most of the unique content of a given webpage. Used only once on a page.
<br>

# What about `<div>` ?

Divs are still useful as containers for very custom jobs but they are meaningless semantically.

**Avoiding using divs and use semantic elements whenever possible.**

For machines (browsers, screen readers and search engines) **a div means a generic container**, even if it has been labeled with an id.

> **Semantic elements are better because they are:**
> - Cleaner for developers
> - Understandable to machines  

Below is a comparison of a website organized with divs vs semantic elements (from [springboardseo.com](https://www.springboardseo.com/resources/what-is/semantic-html.html)).

<br>

![Semantic HTML5 layout, with structural HTML elements](https://www.springboardseo.com/img/html5-semantic-page-layout.jpg)

 <p align="center"><em>Using Semantic Elements</em></p>
 <br>

![Non-semantic HTML layout, with generic divs](https://www.springboardseo.com/img/non-semantic-html-layout.jpg)

<p align="center"><em>Using Divs</em></p>
<br>

# References & Diving Deeper

> **I strongly encourage you to read the** [**Semantic HTML**](https://internetingishard.com/html-and-css/semantic-html/) by internetingishard.com  

Other useful references:  

- [Document and website structure](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure) by MDN Web Docs

- [HTML5 Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp) by W3Schools

- [**HTML semantics cheat sheet**](https://learn-the-web.algonquindesign.ca/topics/html-semantics-cheat-sheet/) by algonquindesign.ca
# Semantic Tags in HTML

## Introduction
The semantic tags are the tags that defines its working by its name itself. It is a newly added feature in HTML5. When semantic tags were not introduced only `div` tags are used for defining different tags. But after introducing semantic tags we can define different sections by using different tag names. For e.g. if we have to define heading of a section we use `heading` tag which is easily understandable by person. It also easy for the browser to distinguish between different tags by using semantic tags.

## Basic difference between semantic and non-semantic tags
The non-semantic tags were used earlier when semantic tags were not introduced, but now the semantic tags made the work of defining different parts of the webpage very easy. Earlier we use `div` tags having id defining the nature of that tag. For e.g. `<div id="header">`,  `<div id="footer">` were used to define header and footer of the document. But after using semantic tags the similar work can be done using `<header>` and `<footer>` tags.

## Some common Semantic tags
Few commonly used semantic tags are described below.

### `<header>`
The `<header>` tag is used to defines the header part of the webpage. It contains various information related to the title and heading of the webpage. We can have several `<header>` elements in one HTML document. It may also have different heading elements havine tags `<h1>` to `<h6>`.

Syntax - `<header>` ...... content ....... `</header>`

### `<footer>`
The `<footer>` tag is used to defines the footer part of the webpage. It contains various information related to authorship, contact details, back to top links, various links, previous and next document links and many more. It is defined at the bottom of the webpage.

Syntax - `<footer>` ...... content ....... `</footer>`

### `<article>`
The `<article>` tag is used to defines a self-contained composition of a webpage. Some of the basic examples of `article` tag are a magazine article, newspaper article and blogs.

Syntax - `<article>` ...... content ....... `</article>`

### `<section>`
The `<section>` tag is used to group similar content of the webpage together. We can use `<section>` tags for defining various sections like about us, contact etc. 

Syntax - `<section>` ...... content ....... `</section>`

### `<nav>`
The `<nav>` tag is used to define navigation bar which comes at the top of the webpage. The navigation bar contains different links like- home, search etc. In simple words, The `<nav>` tag defines a set of navigation links.

Syntax - `<nav>` ...... content ....... `</nav>`

### `<aside>`
The `<aside>` HTML tag represents a portion of a document whose content is indirectly related to the document's main content. `<aside>` tags are represented as sidebars in the webpage. 

Syntax - `<aside>` ...... content ....... `</aside>`

### `<figure>` and `<figcaption>`
The `<figure>` tag is used to define diagrams, photos etc. In this `<figure>` tag we have another tag which is known as `<figcaption>` which is defined within the `<figure>` tag used to define the caption of the figure. 

Syntax - `<figure>`

  `<img src="nature.jpg">`

  `<figcaption>`  Fig1. - Nature Picture.  `</figcaption>`

`</figure>`

### `<main>`
The `<main>` tag is used to represents a portion which is the main content of the document.

Syntax - `<main>` ...... content ....... `</main>`

### `<details>`
The `<details>` tag specifies additional details that the user can open and close on demand. The `<details>` tag is often used to create an interactive widget that the user can open and close. By default, the widget is closed. When open, it expands, and displays the content within it. 

The `<summary>` tag is used as the first child element of the `<details>` tag. 

Syntax - 

```
<details>
        <summary>Do you know what a blog is?</summary>
        <p>In 1994, when blogs began, a blog was more of a personal diary that people shared online. In this online journal, you could talk about your daily life or share about things that you were doing. Then, people saw an opportunity to communicate information in a new way online. Thus began the beautiful world of blogging.</p>
      </details>
```

### `<time>`
The `<time>` tag is used to define time and date within the webpage.

## Hope you like this! Thanks
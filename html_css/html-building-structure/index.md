## HTML Building Structure

In HTML different components are used to make up this language. When we start making a website, we need to learn which HTML element is best to display different types of content. It’s also important to understand how an element is visually displayed on a webpage. If we write code, that code must be semantically correct.


#### What is the semantic code?

Semantic code is essentially code that carries its own meaning. The elements that we use must have proper meaning and structure and we can do that by using proper elements.

#### Semantic element.

The semantic element has clearly described its meaning for the developer and browser. `<aside>`,`<header>`, `<article>`, `<nav>`, `<main>`, `<section>`, `<summary>`,`<footer>` etc. are semantic elements. Every element has some meaning. `<h>` is a semantic element, which gives the text, it wraps around, the meaning of a top-level heading on your page. One of the benefits of semantic markup is search engines will consider its contents as important keywords to influence the page’s search rankings. Screen readers can use it as a signpost to help visually impaired users navigate a page.


#### Non-Semantic element.

The element that does not have any semantic meaning in a page is called a non-semantic element. The non-semantic element can be used anywhere on a page. `<div>` and `<span>` are generic elements, they have no semantic value. Both `<div>` and `<span>`, are extremely valuable when building a website in that they give us the ability to apply targeted styles to a contained set of content.


### Block Element and Inline Element

Most elements are block or inline-level elements.


#### Block-level Element

A block-level element always starts on a new line and takes up the full width available. Block-level Element occupies the entire space of its parent element and creates a block. A `<div>` is a block-level element and it is used to group a large number of elements.

```html
<div class="social">
  <p>Shala Amachi Tuamchi(SAT)</p>
  <p>SAT is an organization which connects the all schools of Maharashtra at a single point. Education is the most powerful weapon which can be used to change the world.</p>
  <p>With the help of internet we connect the two different schools of different levels. Also we conduct various activities for the students of rural areas as well as for the unprivileged schools.</p>
</div>
```

#### Inline-level Element

An inline element does not start on a new line and only takes up as much width as necessary. Inline elements are those which only occupy the space bounded by the tags defining the element, instead of breaking the flow of the content. A `<span>` is an inline-level element it is used to group a small number of elements.

```html
<p>Soon we'll be <span class="tooltip">writing HTML</span> with the best of them.</p>
```

### Basic Structure Element

#### Header

The `<header>` contains information related to the title and heading of the related content. It is the top of a page. A heading, introductory text, and even navigation are included in the header.

#### Headings

Headings are block-level elements, and they come in six different types :`<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, and `<h6>`.The primary heading of a page or section should be marked up with an `<h1>` element and subsequent headings should use `<h2>`, `<h3>`, `<h4>`, `<h5>`, and `<h6>` elements.

```html
<h1>...</h1>
<h2>...</h2>
.
.
<h6>...</h6>
```

#### Navigation

The `<nav>` element identifies a section of major navigational links on a page. The `<nav>` element will link to other pages within the same website or to parts of the same web page. Miscellaneous one-off links should not be wrapped within the `<nav>` element, they should use the anchor <a>element and the anchor element alone.

```html
<nav>...</nav>
```

#### Section

The `<section>` element is used to identify a thematic grouping of content, which generally, but not always, includes a heading. Each `<section>` should be identified, typically by including a heading and paragraph as a child of the `<section>` elements.

```html
<section>...</section>
```

#### Article

The `<article>` element is used to identify a section of independent, self-contained content that may be independently distributed or reused. If the content adds to the document outline and it can be independently redistributed or syndicated, use the `<article>` element.

```html
<article>...</article>
```

#### Aside

The `<aside>` element represents a portion of a document whose content is only indirectly related to the document's main content. Asides are frequently presented as sidebars or call-out boxes.

```html
<aside>...</aside>
```

#### Footer

The `<footer>` element is at the closing or end of a page, article, section, or other segments of a page. Content within the `<footer>` element should be relative information and should not diverge from the document or section it is included within.

```html
<footer>...</footer>
```

#### Creating Hyperlink

Hyperlinks are one of the most exciting innovations the Web has to offer. It provides the ability to link from one web page or resource to another. Hyperlinks are established using the anchor, `<a>` inline-level element. In order to create a link from one page to another, the href attribute, known as a hyperlink reference, is required. The href attribute value identifies the destination of the link.

``` html
<a href="http://shalaamachitumachi.org">SAT</a>
```

### Relative and Absolute Paths

The two most common types of links are links to other pages of the same website and links to other websites.

#### Relative Path

Links pointing to other pages of the same website will have a relative path. The `href` attribute value needs to include only the filename of the page.

```html
<a href="contact.html">Contact</a>
```

#### Absolute Path

Linking to other websites outside of the current one requires an absolute path, where the `href` attribute value must include the full domain. Opening a link in a new window, use the `target` attribute with a value of `_blank`. The `target` attribute determines exactly where the link will be displayed, and the `_blank` value specifies a new window.

```html
<a href="http://www.google.com/">Google</a>
<a href="http://www.shalaamachitumachi.io/" target="_blank">SAT</a>
```

#### Linking to Parts of the Same Page

We can create an on-page link by first setting an id attribute on the element we wish to link to, then using the value of that id attribute within an anchor element’s `href` attribute.

```html
<body id="top">
  ...
  ...
  ...
  <a href="#top">Back to top</a>
  ...
</body>
```

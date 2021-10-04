## Intro HTML and CSS

**A website is a collection of web pages. Webpages are mostly made in three languages HTML, CSS, and Javascript. Using these three languages we can make beautiful and functional websites. These three languages are different from each other.**

### What is HTML?
HTML stands for HyperText Markup Language.

HTML gives content structure and meaning by defining that content as, for example, headings, paragraphs, or images. HTML uses tags to help you add paragraphs, headers, pictures, and other pieces of structure. HTML helps us write something on a website.

### What is CSS?
CSS stands for Cascading Style Sheets

CSS is a presentation language created to style the appearance of content. It is more involved with changing a website's style rather than its content. Kind of like changing the font size, font color and positioning on a word document.


### Common HTML terms
We begin with three common HTML term elements, tags, and attributes.

#### Elements
Elements are the basic building blocks of the HTML. HTML is composed of elements. These elements structure the webpage and define its content. An HTML element is a unit of content in an HTML document formed by HTML tags and the text or media it contains. We have lots of elements, for example, p (paragraph), div, article, nav, section, header, button, img (image), etc. Elements are identified by the use of less-than and greater-than angle brackets, < > surrounding the element name.

```html
<p> Introduction </p>
```

#### Tags
The use of less-than and greater-than angle brackets surrounding an element creates what is known as a tag.

Opening Tag `<p>` — The tag type is surrounded by less-than and greater-than angle brackets.

Closing tag `</p>` — Closing tags have a forward slash (`/`) inside of them.
An anchor link, for example, will have an opening tag of `<a>` and a closing tag of `</a>`. What falls between these two tags will be the content of the anchor link.

```html
<a>...</a>
```

#### Attributes
Attributes are properties used to provide additional information about an element. Most common attributes id attribute, class attribute, src attribute, href attribute. Generally attributes consist of a name and a value.

```html
<a href="http://shalaamachituamachi.org/">SAT</a>
```

The preceding code will display the text "SAT" on the web page. We click on SAT then open a link http://shalaamachituamachi.org/.


### HTML Document structure
All HTML documents have a required structure that includes the following declaration and elements <!DOCTYPE html>, <html>, <head>, <body> HTML documents are plain text documents saved with an .html file. Tags are one of the most important parts of an HTML Document. An HTML Document is mainly divided into two parts one is head and other is body.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>SAT</title>
  </head>
  <body>
    <p>Shala Amachit Tumachi is a non-profit organization.</p>
  </body>
</html>
```

`<head>` — This contains the information about the HTML document like Meta Data, Title of page, HTML Version.

`<body>` — This contains everything you want to display on the Web Page.

`<!DOCTYPE html>` — The document type declaration. Use to tells html version. Doctype is the shortest string of characters that counts as a valid doctype.

`<html>` — This is called HTML root element and used to wrap all the code.


### Common CSS Terms
Selectors, Properties, and value these are common CSS Terms.

#### Selectors
CSS selectors are used to finding the html element you want to style. Selector selectors type Class selector, ID Selector, Universal Selector, Attribute Selectors.

CSS Class Selectors — To select elements with a specific class, write a period (.) character. In the following example “container” is class

```css
.container {
  text-align: center;
  color: red;
}
```

ID Selector — The id selector uses the id attribute of an HTML element. The (#) sign is used to show the id selector. The banner is an id element.

```css
#banner {
  text-align: center;
  padding: 24px 32px;
}
```

Universal Selector — The universal selector (*) selects all HTML elements on the page.

```css
* {
  margin: 0 auto
  padding: 24px 32px;
  background: #ffffff;
}
```

Attributes selectors — The selector is used to select elements with a specified attribute. <a> element with target attribute.

```css
a [target]{
  margin: 0 auto;
  background-color: #ffffff;
}
```

#### Properties

Once an element is selected, a property determines the styles that will be applied to that element. Property names fall after a selector, within the curly brackets `{}`.There are numerous properties we can use such as color, font, font-size, margin, padding, height, width, background and so many.

```css
p {
  font-size: 24px;
  margin: 0 auto;
  background-color: rgb(244 244 244);
}
```

#### Values

CSS selectors are used to finding the html element you want to style. Once an element is selected, a property determines the styles that will be applied to that element. Values can be identified as the text between the colon “:” and semicolon “:”. Here color is property and orange value, font-size is property and 16px value.

```css
p {
  color: orange;
  font-size: 16px;
}
```
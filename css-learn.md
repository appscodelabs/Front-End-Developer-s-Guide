# CSS Note

Source : <strong> Rachel Andrew - The CSS3 Anthology 4th Edition - 2012 </strong>

___
___

## KEYNOTES

* Inline styles have one major disadvantage: it’s impossible to reuse them. Additionally, because inline styles are located within the page’s markup, it makes the code difficult to read and maintain.
* Another approach for applying CSS styles to your web pages is to use the style element:

```html
<style>
⋮ CSS styles go in here…
</style>
```

The style tags are placed inside the head element, and while it’s nice and simple

* An external stylesheet is a file (usually given a .css filename) that contains a website’s CSS styles, keeping them separate from any one web page. Multiple pages can link to the same .css file, and any changes you make to the style definitions in that file will affect all the pages that link to it.

To link a document to an external stylesheet (say, styles.css), we simply place a link
element within the document’s head element:

```html
<link rel="stylesheet" href="style.css" />
```

## CSS Syntax

A style sheet is a collection of style definitions. Every CSS style definitions has two main components:

* A list of one or more selectors, separated by commas, define the element or elements to which the style will be applied.
* The declaration block, separated by curly braces {..} , specifies what the rule atually does.

```css
h1, h2 {
font-family: "Times New Roman", Times, serif;
color: #3366cc;
}
h1, h2 {
font-family: "Times New Roman", Times, serif; color: #3366cc;
}
```
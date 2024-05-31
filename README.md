# Web Development

## HTML

### lang

We should alwyas include the `lang` attribute inside the html tag, to declare the language of the Web page. This is meant to assist search engines and browsers.

```html
<!DOCTYPE html>
<html lang="en">
  <body>
    ...
  </body>
</html>
```

Country codes can also be added to the language code in the lang attribute. So, the first two characters define the language of the HTML page, and the last two characters define the country.

```html
<!DOCTYPE html>
<html lang="en-US">
  <body>
    ...
  </body>
</html>
```

### Style

`style` attribute is used for styling HTML elements

- `backgroud-color` => for background color
- `color` => for text color
- `font-family` => for text fonts
- `font-size` => for text sizes
- `text-align` => for text alignment

```html
<p
  style="background-color: blue; color: white; font-family: sans-serif; font-size: 16px; text-align: center; "
>
  Frontend
</p>
```

### hr tag

`hr` tag is known as horizontal rule tag, used to give horizontal line in the website

```html
<hr />
```

### HTML Text Formatting Inline Elements

- `b` => bold text
- `strong` => important text
- `i` => italic text
- `em` => emphasized text
- `mark` => marked text
- `small` => smaller text
- `del` => deleted text
- `ins` => inserted text
- `sub` => subscript text
- `sup` => superscript text

```html
<!-- for bold text -->
<b>Hello World!</b>

<!-- for important text -->
<strong>Hello World!</strong>

<!-- for italic text -->
<i>Hello World!</i>

<!-- for emphasized text -->
<em>Hello World!</em>

<!-- for marked/highlighted text -->
<mark>Hello World!</mark>

<!-- for small text -->
<small>Hello World!</small>

<!-- for deleted text -->
<del>Hello World!</del>

<!-- for inserted text -->
<ins>Hello World!</ins>

<!-- for subscript text -->
<sub>Hello World!</sub>

<!-- for superscript text -->
<sup>Hello World!</sup>
```

### Anchor tag

`a` tag is used to add some hyperlinks to the html file

```html
<a target="_blank" href="https://en.wikipedia.org/wiki/HTML" title="HTML"
  >HTML</a
>
```

- target attribute is used to open the link in a new tab on default.
- href attribute is used to provide the actual url link.
- title attribute is used to provide the tooltip information of the hyperlink text.

### Image tag

`img` tag is used to add images to the html file
`alt` is the field which will be displayed when there is some issue due which the website cannot load the image

```html
<img
  src="/assets/images/css.png"
  alt="html-css-javascript"
  style="width: 100%; max-width: 600px"
  title="CSS"
/>

<!-- Change the  src attribute with the original location of the image. -->
```

### Lists

- Unordered List

`ul` tag is known as the Unordered List tag. This tag is used to list out things with bullets

```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

- The CSS `list-style-type` property is used to define the style of the list item marker. It can have one of the following values:

|  Value   | Description                                   |
| :------: | :-------------------------------------------- |
|  `disc`  | Sets the list item marker to bullet (default) |
| `circle` | Sets the list item marker to a circle         |
| `square` | Sets the list item marker to a square         |
|  `none`  | The list items will not be marked             |

```html
<ul style="list-style-type: disc;">
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

- Nested HTML lists

```html
<ul>
  <li>HTML</li>
  <li>
    CSS
    <ul>
      <li>Inline CSS</li>
      <li>Separate CSS</li>
    </ul>
  </li>
  <li>JavaScript</li>
</ul>
```

- Ordered List

`ol` tag is known as the Ordered List tag. This tag is used to list out things with numbers.

The list items are marked with numbers by default.

```html
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```

- The `type` attribute of the ordered list tag, defines the type of the list item marker:

|     Type     | Description                                            |
| :----------: | :----------------------------------------------------- |
| `type = "1"` | The list will be numbered with numbers (default)       |
| `type = "A"` | The list will be numbered with uppercase letters       |
| `type = "a"` | The list will be numbered with lowercase letters       |
| `type = "I"` | The list will be numbered with uppercase roman numbers |
| `type = "i"` | The list will be numbered with lowercase roma numbers  |

```html
<ol type="1">
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```

- Control List Counting

By default, an ordered list will start counting from 1. If you want to start counting from a specified number, you can use the `start` attribute:

```html
<ol start="10">
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```

### Linebreak

`br` tag is used to give line break

```html
<br />
```

### HTML Entities

- &nbsp; => non-breaking space
- &lt; => less than
- &gt; => greater than
- &amp; => ampersand
- &quot; => double quotation mark
- &apos; => single quotation mark
- &cent; => cent
- &pound; => pound
- &yen; => yen
- &euro; => euro
- &copy; => copyright
- &reg; => trademark

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>HTML Entity Example</h1>

    <h2>A space character: &nbsp;</h2>
    <h2>A less than character: &lt;</h2>
    <h2>A greater than character: &gt;</h2>
    <h2>A ampersand character: &amp;</h2>
    <h2>A double quotation mark: &quot;</h2>
    <h2>A single quotation mark: &apos;</h2>
    <h2>A cent character: &cent;</h2>
    <h2>A pound character: &pound;</h2>
    <h2>A yen character: &yen;</h2>
    <h2>A euro character: &euro;</h2>
    <h2>A copyright character: &copy;</h2>
    <h2>A trademark character: &reg;</h2>
  </body>
</html>
```

### Semantic Tags

Semantic Tags: In HTML, there are some semantic elements that can be used to define different parts of a web page

- `article` => The `article` element specifies independent, self-contained content.

- `aside` => The `aside` element defines some content aside from the content it is placed in (like a sidebar).
  The `aside` content should be indirectly related to the surrounding content.

- `details` => The `details` element defines additional details that the user can view or hide.

- `figcaption` => Th `figcaption` tag defines a captino for a `figure` element. The `figcaption` element can be placed as the first or as the last child of a `figure` element.

- `figure` => The figure tag specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.

- `footer` => The `footer` element defines a footer for a documnet or section.
  
  A `footer` element typically contains:
  - authorship information
  - copyright information
  - contact information
  - sitemap
  - back to top links
  - related documents

- `header` => The `header` element represents a container for indtroductory content or a set of navigational links.
  
  A `header` element typically contains:
  - one or more heading elements (h1 - h6)
  - logo or icon
  - authorship information

- `main` => The `main` element specifies the main content of a document.

- `mark` => The `mark` element defines marked/highlighted text.

- `nav` => The `nav` element defines a set of navigation links.

- `section` => The `section` element defines a section in a document

- `summary` => The `summary` element defines a visible heading for a details element.

- `time` => The `time` element defines a date/time.

- `em` => The `em` element emphasizes some text.

- `strong` => The `strong` element defines some important text in the document.

### Attributes

- All HTML elements can have attributes.
- Attributes provide additional information about elements.
- Attributes are always specified in the start tag.
- Attributes ususally come in name/value pairs like: name = "value".
- The Global attributes are attributes that can be used with all HTML elements:

|     Attribute     | Description                                                                          |
| :---------------: | :----------------------------------------------------------------------------------- |
|    `accesskey`    | Specifies a shortcut key to activate/focus an element                                |
|      `class`      | Specifies one or more classnames for an element (refers to a class in a style sheet) |
| `contenteditable` | Specifies whether the content of an element is editable or not                       |
|     `data-*`      | Used to store custom data private to the page or application                         |
|       `dir`       | Specifies the text direction for the content in an element                           |
|    `draggable`    | Specifies whether an element is draggable or not                                     |
|  `enterkeyhint`   | Specifies the text of the enter-key on a virtual keyboard                            |
|     `hidden`      | Specifies that an element is not yet, or is no longer, relevant                      |
|       `id`        | Specifies a unique id for an element                                                 |
|      `inert`      | Specifies that the browser should ignore this section                                |
|    `inputmode`    | Specifies the mode of a virtual keyboard                                             |
|      `lang`       | Specifies the language of the element's content                                      |
|     `popover`     | Specifies a popover element                                                          |
|   `spellcheck`    | Specifies whether the element is to have its spelling and grammer checked or not     |
|      `style`      | Specifies an inline CSS style for an element                                         |
|    `tabindex`     | Specifies the tabbing order of an element                                            |
|      `title`      | Specifies extra information about an element                                         |
|    `translate`    | Specifies whether the content of an element should be translated or not              |


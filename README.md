# HTML Tags with Examples

## Document Structure

### `<!DOCTYPE html>`
```html
<!DOCTYPE html>
```

- Defines the document type and version of HTML.

### `<html>`
```html
<html lang="en">
<!-- Document content goes here -->
</html>
```

- Represents the root element of an HTML document.
- `lang` Defines the document language.
  `bn` for Bangla language.
  `en` for English language.
  `hi` for Hindi language.
  etc.

### `<head>`
```html
<head>
<!-- Meta tags, title, and other head elements go here -->
</head>
```

- Contains meta-information about the HTML document.

### `<title>`
```html
<title>Page Title</title>
```

- Sets the title of the HTML document.

### `<body>`
```html
<body>
<!-- Content visible on the webpage goes here -->
</body>
```

- Contains the content displayed on the webpage.

## Text Formatting

### `<p>`
```html
<p>This is a paragraph.</p>
```

- Represents a paragraph.

### `<pre>`
```html
<pre>
  This is preformatted text.
  It preserves both spaces and line breaks.
</pre>
```

- `<pre>` Represents preformatted text, preserving both spaces and line breaks.

### `<b>` and `<strong>`
```html
<b>Bold Text</b>
<strong>Strong Text</strong>
```

- `<b>` Represents bold text.
- `<strong>` Represents strong importance (often bold).

### `<i>` and `<em>`
```html
<i>Italic Text</i>
<em>Emphasized Text</em>
```

- `<i>` Represents italic text.
- `<em>` Represents emphasized text.

### `<u>`
```html
<u>Underlined Text</u>
```

- Represents underlined text. Note Styling underlined text is discouraged.

### `<s>` and `<del>`
```html
<s>Strikethrough Text</s>
<del>Deleted Text</del>
```

- `<s>` Represents strikethrough text.
- `<del>` Represents deleted or removed text.

### `<sub>` and `<sup>`
```html
H<sub>2</sub>O (Subscript)
E=mc<sup>2</sup> (Superscript)
```

- `<sub>` Represents subscript text.
- `<sup>` Represents superscript text.

### `<code>` and `<pre>`
```html
<code>Inline Code</code>
<pre>Block of Code</pre>
```

- `<code>` Represents inline code.
- `<pre>` Represents preformatted text, often used for code blocks.

### `<small>`
```html
<small>Smaller Text</small>
```

- Represents smaller text.

### `<mark>`
```html
<mark>Highlighted Text</mark>
```

- Represents marked or highlighted text.

### `<blockquote>`
```html
<blockquote>
  This is a blockquote. It is used to emphasize extended quotations.
</blockquote>
```

- `<blockquote>` Represents a section that is a quotation from another source.

### `<abbr>`
```html
<abbr title="Hypertext Markup Language">HTML</abbr>
```

- `<abbr>` Represents an abbreviation or acronym with an optional title.

### `<cite>`
```html
<cite>Author Name</cite>
```

- `<cite>` Represents the title of a creative work (e.g., a book, a song).

### `<q>`
```html
<q>This is a short inline quotation.</q>
```

- `<q>` Represents a short inline quotation.

## List

HTML provides different types of lists, each with its own style. You can create lists using the `<ul>`, `<ol>`, and `<li>` tags.

## Unordered List (`<ul>`):

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

- Default style: Bulleted list.

## Ordered List (`<ol>`):

```html
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```

- Default style: Numbered list.

## Customizing Ordered List Styles:

### Roman Numerals (`type="I"`, `type="i"`, `type="A"`, `type="a"`):

```html
<ol type="I">
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```

- `type="I"`: Capital Roman numerals (I, II, III).
- `type="i"`: Small Roman numerals (i, ii, iii).
- `type="A"`: Capital letters (A, B, C).
- `type="a"`: Small letters (a, b, c).

### Custom Start Value:

```html
<ol start="5">
  <li>Fifth item</li>
  <li>Sixth item</li>
  <li>Seventh item</li>
</ol>
```

- Starts the list numbering from a custom value (5 in this example).

## Definition List (`<dl>`, `<dt>`, `<dd>`):

```html
<dl>
  <dt>Term 1</dt>
  <dd>Definition 1</dd>
  <dt>Term 2</dt>
  <dd>Definition 2</dd>
</dl>
```

- Used for creating definition lists.

## Links and Images

### `<a>`
```html
<a href="https//example.com">Link Text</a>
```

- Represents a hyperlink.

### `<img>`
```html
<img src="image.jpg" alt="Image Description">
```

- Represents an image.

### `<figure>` and `<figcaption>`
```html
<figure>
<img src="image.jpg" alt="Image Description">
<figcaption>Caption for the image</figcaption>
</figure>
```

- `<figure>` Contains any content that is referenced from the main content.
- `<figcaption>` Represents a caption or legend for a `<figure>`.

## Tables

### `<table>`
```html
<table>
<tr>
<th>Header 1</th>
<th>Header 2</th>
</tr>
<tr>
<td>Data 1</td>
<td>Data 2</td>
</tr>
</table>
```

- Represents a table.

### `<tr>`, `<th>`, and `<td>`
```html
<tr>
<th>Header 1</th>
<th>Header 2</th>
</tr>
<tr>
<td>Data 1</td>
<td>Data 2</td>
</tr>
```

- `<tr>` Represents a table row.
- `<th>` Represents a table header cell.
- `<td>` Represents a table data cell.

### Table Attributes
```html
<table border="1" cellpadding="10">
<!-- Table content -->
</table>
```

- `border` Adds a border to the table.
- `cellpadding` Specifies padding within each table cell.

## Forms

### `<form>`, `<input>`, and `<button>` (Continued)

```html
<label for="username">Username</label>
<input type="text" id="username" name="username" required>

<label for="password">Password</label>
<input type="password" id="password" name="password" required>

<button type="submit">Submit</button>
</form>
```

- `<form>` Represents an HTML form.
    Attributes used
   - `action` Specifies the URL to which the form data will be sent.
   - `method` Defines the HTTP method (e.g., `post` or `get`) used for form submission.
   - [See more](form_tag_property.md)

## Button

  `<button>`

- `<button>` Represents a clickable button within a form.
 - `id` and `class` Identifiers for form elements, often used in scripting.

## Label

 `<label>`

- `for` Associates a label with a form element.

## Input
  `input`
- `<input>` Represents an input field within a form.
- `type` Specifies the type of the input field (e.g., `text`, `password`).
- Here is some Common & Less Common or Specialized HTML Input Types
  [Click me](input_type.md)
- `id` and `name` Identifiers for form elements, often used in scripting.
- `required` Specifies that the input must be filled out before submitting the form.
- [See more input tag property](input_tag_property.md)
- `<input>` Represents an input field within a form.

## Meta Tags

### `<meta>`
```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

- `<meta>` Represents metadata that provides additional information about the HTML document.

Attributes used
- `charset` Specifies the character encoding for the HTML document.
- `name` and `content` Used for various metadata purposes.
- [See more](meta_tag_property.md)

## Miscellaneous

### `<hr>`
```html
<hr>
```

- Represents a thematic break or horizontal line.

### `<div>`
```html
<div>
<!-- Content goes here -->
</div>
```

- Represents a division or a container for other HTML elements.

### `<span>`
```html
<span style="color red;">This is red text</span>
```

- Represents an inline container for text.

## Additional Tags

### `<canvas>`
```html
<canvas id="myCanvas" width="200" height="100"></canvas>
```

- `<canvas>` Used for drawing graphics with JavaScript.

### `<marquee>`
```html
<marquee behavior="scroll" direction="left">Scrolling Text</marquee>
```

- `<marquee>` Represents scrolling text or an image.

 ## Updated Tags

Here are some of the most notable HTML tags that have been introduced or updated in recent times, as of January 30, 2024

### `<picture>`

```html
<picture>
  <source srcset="large-image.jpg" media="(min-width 600px)">
  <source srcset="medium-image.jpg" media="(min-width 400px)">
  <img src="small-image.jpg" alt="Image description">
</picture>
```

- Purpose Provides a more flexible way to manage images for responsive design.
- Allows Specifying different image sources for different screen sizes and viewport conditions.
- Browser Support Excellent in modern browsers.

### `<srcset>`

```html
<img src="image.jpg" srcset="image-small.jpg 320w, image-medium.jpg 640w, image-large.jpg 1024w">
```

- Purpose Declares multiple image sources, allowing the browser to choose the most appropriate one based on screen size or device pixel ratio.
- Works In conjunction with the `<picture>` element or the `src` attribute of an `<img>` element.
- Browser Support Widely supported in modern browsers.

### `<figure>` and `<figcaption>`

```html
<figure>
  <img src="image.jpg" alt="Image description">
  <figcaption>Figure caption</figcaption>
</figure>
```

- `<figure>` Groups related content, such as an image and its caption, into a self-contained unit.
- `<figcaption>` Provides a caption or a legend for a `<figure>` element, typically used to describe images or visual content.

- Purpose Define self-contained content like images, diagrams, code blocks, etc., with captions.
- Improve Semantic structure and accessibility of content.
- Browser Support Excellent in modern browsers.

### `<video>` and `<audio>`

```html
<video width="300" height="150" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```
```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

```

- Purpose Embed video and audio content directly into web pages.
- Support Multiple formats and playback controls.
- Browser Support Widely supported in modern browsers.

### `<details>` and `<summary>`

```html
<details>
  <summary>Click for more details</summary>
  <p>Additional details here.</p>
</details>
```

- `<details>` Creates a disclosure widget, allowing content to be hidden or shown based on user interaction with the `<summary>` element.
- `<summary>` Specifies the visible heading for a `<details>` element, serving as the clickable trigger to toggle the content's visibility.

- Purpose Create expandable and collapsible content sections.
- Allow Users to toggle additional information on demand.
- Browser Support Excellent in modern browsers.

### `<main>`

```html
<main>
  </main>
```

- Purpose Identifies the primary content of a web page.
- Improve Semantic structure and accessibility.
- Browser Support Excellent in modern browsers.

### `<dialog>`

```html
<dialog open>
  <p>This is a modal dialog box.</p>
  <button>Close</button>
</dialog>
```

- `<dialog>` Creates a dialog box or a modal window, allowing for focused user interaction or information display.

### `<slot>`

```html
<template>
  <h2>My Web Component</h2>
  <slot></slot>
</template>
```

- `<slot>` Acts as a placeholder within web components, defining where content from outside the component should be inserted. It's a key feature for building reusable and customizable components.


### `<header>`, `<footer>`, `<nav>`, `<section>`, `<article>`, and `<aside>`

- Purpose Define different sections of a web page, enhancing semantic structure and accessibility.
- Browser Support Excellent in modern browsers.

These examples cover a range of HTML tags commonly used for structuring content, applying styles, creating lists, adding links and images, designing tables, building forms, and including meta-information.

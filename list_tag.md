# List Types

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

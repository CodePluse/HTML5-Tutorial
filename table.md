# HTML `<table>` Tag

The `<table>` tag in HTML is used to create tables to organize and present data. Tables consist of rows (`<tr>`), columns (`<td>` for data cells, `<th>` for header cells), and can include various attributes for customization.

## Basic Table Structure:

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

- `<tr>`: Table row.
- `<th>`: Table header cell.
- `<td>`: Table data cell.

## Table Attributes:

### Border Attribute:

```html
<table border="1">
  <!-- Table content -->
</table>
```

- Adds a border to the table.

### Cellpadding and Cellspacing Attributes:

```html
<table cellpadding="10" cellspacing="5">
  <!-- Table content -->
</table>
```

- `cellpadding`: Specifies the padding within each table cell.
- `cellspacing`: Specifies the spacing between table cells.

### Width Attribute:

```html
<table width="100%">
  <!-- Table content -->
</table>
```

- Sets the width of the table. Can be a percentage or a specific value.

### Colspan and Rowspan Attributes:

```html
<tr>
  <td colspan="2">Spanning two columns</td>
</tr>
<tr>
  <td rowspan="2">Spanning two rows</td>
  <td>Data</td>
</tr>
```

- `colspan`: Specifies the number of columns a cell should span.
- `rowspan`: Specifies the number of rows a cell should span.

## Example:

```html
<table border="1" cellpadding="10">
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
  <tr>
    <td colspan="2">Spanning two columns</td>
  </tr>
</table>
```

These attributes allow you to customize the appearance and structure of your HTML tables.
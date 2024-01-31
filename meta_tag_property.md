# HTML `<meta>` Tag Properties

The `<meta>` tag in HTML is used to provide metadata about the document. It includes information such as character set, viewport settings, and more. Here are commonly used properties:

## Essential Attributes:

1. **`charset` Attribute:**
   - Specifies the character encoding for the HTML document. Example: `charset="UTF-8"`.

2. **`name` and `content` Attributes:**
   - Used together to define metadata content. Common values include:
     - `viewport`: Configures the viewport for responsive design. Example: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`.
     - `description`: Provides a short description of the document's content. Example: `<meta name="description" content="Page description">`.

3. **`http-equiv` Attribute:**
   - Provides an HTTP header for the information defined in the `content` attribute. Example: `<meta http-equiv="refresh" content="5;url=https://example.com/">`.

## Character Set and Language:

4. **`charset` Attribute:**
   - Specifies the character encoding for the HTML document. Example: `charset="UTF-8"`.

5. **`lang` Attribute:**
   - Specifies the primary language for the document. Example: `lang="en"`.

## Search Engine Optimization (SEO):

6. **`robots` Attribute:**
   - Controls search engine indexing behavior. Example: `<meta name="robots" content="index, follow">`.

7. **`keywords` Attribute:**
   - Specifies a comma-separated list of keywords relevant to the page. Example: `<meta name="keywords" content="HTML, CSS, JavaScript">`.

## Other Attributes:

8. **`viewport` Attribute:**
   - Configures the viewport for responsive design. Example: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`.

9. **`http-equiv` Attribute:**
   - Provides an HTTP header for the information defined in the `content` attribute. Example: `<meta http-equiv="refresh" content="5;url=https://example.com/">`.

## Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Page description">
  <meta name="robots" content="index, follow">
</head>
<body>
  <!-- Your HTML content here -->
</body>
</html>
# HTML `<link>` Tag Properties

The `<link>` tag in HTML is used to link external resources, such as stylesheets or icons, to an HTML document. Here are the commonly used properties:

## Essential Attributes:

1. **`rel` Attribute:**
- Defines the relationship between the current document and the linked resource. Common values include:
- `stylesheet`: Links to an external stylesheet.
- `icon`: Specifies a favicon or app icon.

2. **`href` Attribute:**
- Specifies the URL of the linked resource.

## Conditional Attributes:

3. **`media` Attribute:**
- Specifies the media type for which the linked stylesheet is intended. Example: `media="screen"`.

4. **`type` Attribute:**
- Defines the type of the linked resource. For stylesheets, it is typically `text/css`.

5. **`sizes` Attribute:**
- Specifies the sizes of the linked icon for different display densities. Example: `sizes="16x16 32x32"`.

## Cross-Origin Attributes:

6. **`crossorigin` Attribute:**
- Controls how the browser handles cross-origin requests. Common values include:
- `anonymous`: No credentials are sent.
- `use-credentials`: Credentials are sent if the requesting origin is a same-origin.

## Additional Attributes:

7. **`integrity` Attribute:**
- Provides a subresource integrity (SRI) value, ensuring the resource hasn't been tampered with.

8. **`as` Attribute:**
- Specifies the type of the resource. For example, `as="font"` or `as="image"`.

9. **`charset` Attribute:**
- Specifies the character encoding for the linked resource.

10. **`title` Attribute:**
- Describes the linked resource. Useful for accessibility.

11. **`disabled` Attribute:**
- Disables the link, preventing the linked resource from being applied.

## Example:

```html
<!-- Linking an external stylesheet -->
<link rel="stylesheet" type="text/css" href="styles.css">

<!-- Linking a favicon -->
<link rel="icon" type="image/png" href="favicon.png">
# HTML Form Tag Properties

The `<form>` tag in HTML is used to create a form for user input. It contains various attributes that control its behavior and appearance. Below are some common attributes along with their explanations:

## action

- **Description:** Specifies the URL where the form data should be submitted.
- **Example:** `<form action="/submit_form.php" method="post">`

## method

- **Description:** Defines the HTTP method used when submitting the form data.
- **Values:** `get` or `post`.
- **Example:** `<form action="/submit_form.php" method="post">`

## target

- **Description:** Specifies where to display the response received after submitting the form.
- **Values:** `_self`, `_blank`, `_parent`, `_top`, or custom frame/window name.
- **Example:** `<form action="/submit_form.php" method="post" target="_blank">`

## enctype

- **Description:** Defines how the form data should be encoded before submitting it to the server.
- **Values:** `application/x-www-form-urlencoded`, `multipart/form-data`, or `text/plain`.
- **Example:** `<form action="/submit_form.php" method="post" enctype="multipart/form-data">`

## name

- **Description:** Assigns a name to the form.
- **Example:** `<form action="/submit_form.php" method="post" name="user_form">`

## autocomplete

- **Description:** Indicates whether the browser should autocomplete form values.
- **Values:** `on` or `off`.
- **Example:** `<form action="/submit_form.php" method="post" autocomplete="off">`

## novalidate

- **Description:** Prevents the browser from validating the form before submitting.
- **Example:** `<form action="/submit_form.php" method="post" novalidate>`

## accept-charset

- **Description:** Specifies the character encodings that are to be used for form submission.
- **Example:** `<form action="/submit_form.php" method="post" accept-charset="UTF-8">`

## onsubmit

- **Description:** Specifies a script to execute when the form is submitted.
- **Example:** `<form action="/submit_form.php" method="post" onsubmit="return validateForm()">`

## enctype

- **Description:** Specifies how form data should be encoded before sending it to the server.
- **Example:** `<form action="/submit_form.php" method="post" enctype="multipart/form-data">`

## accept

- **Description:** Specifies the types of files that the server accepts.
- **Example:** `<input type="file" name="file_upload" accept=".jpg, .png">`

## Other Attributes

- **Required:** Specifies that an input field must be filled out before submitting the form.
- **Disabled:** Disables the form control so that it cannot be used.
- **Placeholder:** Provides a hint to the user about what should be entered in the input field.
- **Multiple:** Allows the user to select multiple files for upload.

These are some of the most commonly used attributes of the `<form>` tag in HTML. Experimenting with these attributes will give you a better understanding of how forms work in web development.

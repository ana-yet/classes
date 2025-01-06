# HTML Form Creation Notes

## HTML Structure

### Basic Document Setup

- Use `<!DOCTYPE html>` for HTML5 declaration.
- The `<html>` tag should include the `lang` attribute (e.g., `lang="en"`).
- Include `<head>` for metadata and styles.
  - Use `<meta charset="UTF-8">` to specify character encoding.
  - Use `<meta name="viewport" content="width=device-width, initial-scale=1.0">` for responsive design.
  - Include a `<title>` to specify the page title.
- Use `<body>` for the main content of the page.

### Styling

- Add inline CSS using the `<style>` tag inside `<head>`.
- Example: Style labels with `display: block` and `margin-bottom: 10px` for better spacing.

## Form Design

### Form Basics

- Use `<form>` to create a form.
- Group form inputs using `<label>` for accessibility and better organization.
- Example of a text input:
  ```html
  <label for="name"
    >Your Name: <input id="name" type="text" placeholder="Your Name"
  /></label>
  ```

### Input Types

1. **Text Input:**

   - `type="text"`: Basic text input.
   - Add `placeholder` for hints (e.g., `placeholder="Your Name"`).

2. **Email Input:**

   - `type="email"`: For email addresses.
   - Example:
     ```html
     <label for="email"
       >Your Email: <input id="email" type="email" placeholder="Your Email"
     /></label>
     ```

3. **Number Input:**
   - `type="number"`: For numeric values.
   - Use `min` and `max` attributes to set a range.
   - Note: The `maxlength` attribute doesn't work with `type="number"`.
   - Example:
     ```html
     <label for="phone"
       >Your Phone: <input id="phone" type="number" placeholder="Your Phone"
     /></label>
     ```

### Radio Buttons

- Use `<input type="radio">` for single-choice options.
- Group related radio buttons with the same `name` attribute.
- Example:
  ```html
  <fieldset>
    <legend>Pick Something</legend>
    <label for="pubg"><input type="radio" name="game" id="pubg" /> Pubg</label>
    <label for="ff"><input type="radio" name="game" id="ff" /> Free Fire</label>
  </fieldset>
  ```

### Checkboxes

- Use `<input type="checkbox">` for multiple-choice options.
- Example:
  ```html
  <fieldset>
    <legend>Checkbox</legend>
    <label for="shutki"
      ><input type="checkbox" name="food" id="shutki" /> Shutki</label
    >
    <label for="bhorta"
      ><input type="checkbox" name="food" id="bhorta" /> Bhorta</label
    >
  </fieldset>
  ```

### Textarea

- Use `<textarea>` for multiline text input.
- Attributes:
  - `cols`: Width of the text area (number of columns).
  - `rows`: Height of the text area (number of rows).
  - Example:
    ```html
    <legend>Special Instruction</legend>
    <textarea
      id="instructions"
      cols="30"
      rows="2"
      placeholder="Enter your instructions here"
    ></textarea>
    ```

### Buttons

- `type="reset"`: Resets the form fields to their default values.
- `type="submit"`: Submits the form data.
- Example:
  ```html
  <input type="reset" value="Reset" /> <input type="submit" value="Submit" />
  ```

## Additional Notes

- Always pair `<label>` with `for` attributes matching the `id` of the corresponding input.
- Use `<fieldset>` and `<legend>` to group related form controls.
- Add meaningful placeholders to guide users.
- Use consistent naming conventions for `name` attributes to group radio buttons or checkboxes logically.

---

By following these notes, you can create clean, accessible, and user-friendly forms.

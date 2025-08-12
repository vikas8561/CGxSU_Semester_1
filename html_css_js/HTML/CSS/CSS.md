# CSS Properties and Types of CSS

CSS (Cascading Style Sheets) is used to style HTML elements, controlling their appearance and layout on a webpage. CSS can be applied in three primary ways: inline, internal, and external. This document explains common CSS properties, inspired by W3Schools' documentation, and details the types of CSS, with examples tailored to Coding Gita and SwamiNarayan University.

## Types of CSS
CSS can be applied to HTML in three ways, each with its own use case and advantages:

1. **Inline CSS**:
   - **Description**: Uses the `style` attribute directly within an HTML element to apply styles. It has the highest specificity but is hard to maintain for large projects.
   - **Use Case**: Quick, one-off styling for specific elements.
   - **Example**:
     ```html
     <p style="color: blue;">Join Coding Gita for web development!</p>
     ```
     The text is styled blue directly in the HTML.

2. **Internal CSS**:
   - **Description**: Defined within a `<style>` tag in the `<head>` section of an HTML document. It applies to the entire page and is more maintainable than inline CSS.
   - **Use Case**: Styling a single webpage without needing a separate file.
   - **Example**:
     ```html
     <head>
       <style>
         p { color: green; }
       </style>
     </head>
     <body>
       <p>SwamiNarayan University offers tech degrees.</p>
     </body>
     ```
     All `<p>` elements on the page have green text.

3. **External CSS**:
   - **Description**: Defined in a separate `.css` file, linked to the HTML document using the `<link>` tag. It offers the best maintainability for large projects.
   - **Use Case**: Consistent styling across multiple webpages.
   - **Example**:
     ```html
     <!-- index.html -->
     <head>
       <link rel="stylesheet" href="styles.css">
     </head>
     <body>
       <p>Coding Gita: Learn to code!</p>
     </body>
     ```
     ```css
     /* styles.css */
     p {
       color: purple;
     }
     ```
     The `<p>` element is styled purple via the external stylesheet.

## Common CSS Properties
Below are commonly used CSS properties, as referenced from W3Schools, applied using internal CSS within a `<style>` tag for consistency with the previous request.

1. **color**: Sets the text color.
2. **background-color**: Sets the background color of an element.
3. **font-family**: Specifies the font for the text.
4. **font-size**: Sets the size of the text.
5. **text-align**: Aligns the text (e.g., left, center, right).
6. **padding**: Adds space inside the element’s borders.
7. **margin**: Adds space outside the element’s borders.
8. **border**: Defines the border around an element.

### Examples with Coding Gita and SwamiNarayan University

#### 1. Text Color (`color`)
```html
<style>
  .welcome-text {
    color: blue;
  }
</style>
<p class="welcome-text">Join Coding Gita to learn web development!</p>
```
The text is displayed in blue.

#### 2. Background Color (`background-color`)
```html
<style>
  .university-heading {
    background-color: #f0f0f0;
  }
</style>
<h2 class="university-heading">SwamiNarayan University: Innovate, Learn, Succeed</h2>
```
The heading has a light grey background.

#### 3. Font Family (`font-family`)
```html
<style>
  .workshop-text {
    font-family: Arial, sans-serif;
  }
</style>
<p class="workshop-text">Coding Gita offers hands-on Python workshops.</p>
```
The text uses the Arial font, with sans-serif as a fallback.

#### 4. Font Size (`font-size`)
```html
<style>
  .lab-heading {
    font-size: 24px;
  }
</style>
<h3 class="lab-heading">SwamiNarayan University’s AI Research Lab</h3>
```
The heading is displayed with a font size of 24 pixels.

#### 5. Text Alignment (`text-align`)
```html
<style>
  .bootcamp-heading {
    text-align: center;
  }
</style>
<h4 class="bootcamp-heading">Register now for Coding Gita’s 2025 coding bootcamp!</h4>
```
The text is centered within the `<h4>` element.

#### 6. Padding (`padding`)
```html
<style>
  .degree-text {
    padding: 15px;
  }
</style>
<p class="degree-text">SwamiNarayan University offers cutting-edge tech degrees.</p>
```
The text has 15 pixels of padding on all sides.

#### 7. Margin (`margin`)
```html
<style>
  .path-heading {
    margin: 20px;
  }
</style>
<h4 class="path-heading">Coding Gita: Your path to mastering programming.</h4>
```
The heading has 20 pixels of margin on all sides.

#### 8. Border (`border`)
```html
<style>
  .enroll-text {
    border: 2px solid green;
  }
</style>
<p class="enroll-text">Enroll in SwamiNarayan University’s Data Science program today!</p>
```
The `<p>` has a 2-pixel-wide, solid green border.

### Combined Example (Using Internal CSS)
```html
<head>
  <style>
    .main-heading {
      color: #0066cc;
      text-align: center;
      font-family: Verdana, sans-serif;
    }
    .collaboration-text {
      font-size: 16px;
      background-color: #e6f3ff;
      padding: 10px;
      margin: 20px;
    }
    .highlight {
      color: purple;
      font-family: Georgia, serif;
    }
    .session-heading {
      border: 1px dashed #333;
      text-align: center;
      padding: 15px;
    }
  </style>
</head>
<body>
  <h1 class="main-heading">Welcome to Coding Gita</h1>
  <p class="collaboration-text">
    Coding Gita and <span class="highlight">SwamiNarayan University</span> collaborate to offer innovative tech education.
  </p>
  <h3 class="session-heading">Join our practical sessions to build real-world projects!</h3>
</body>
```
This example combines multiple CSS properties:
- The `<h1>` has blue text, centered, in Verdana font.
- The `<p>` has a 16-pixel font size, light blue background, 10-pixel padding, and 20-pixel margin, with a `<span>` for "SwamiNarayan University" in purple Georgia font.
- The `<h3>` has a dashed black border, centered text, and 15-pixel padding.

## Summary
CSS can be applied via inline, internal, or external methods, each suited to different use cases. Inline CSS is quick but less maintainable, internal CSS is page-specific, and external CSS is ideal for large projects. Common properties like `color`, `background-color`, `font-family`, `font-size`, `text-align`, `padding`, `margin`, and `border` allow for flexible styling, as shown in the examples for Coding Gita and SwamiNarayan University. For scalability, external CSS is recommended.

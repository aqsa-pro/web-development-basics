
# Homework: Introduction to CSS

## Instructions

Complete the following tasks to practice using CSS with HTML. Submit your work as a single HTML file named `homework_lesson6.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: Including CSS in HTML

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Demonstrate the use of all three methods of including CSS in HTML:
    - **Inline CSS**: Apply a style directly within an HTML element.
    - **Internal CSS**: Apply styles using a `<style>` tag within the `<head>` section.
    - **External CSS**: Link to an external CSS file.

### Task 2: CSS Syntax

1. In your HTML file, create multiple HTML elements (e.g., paragraphs, headings, divs).
2. Apply CSS styles to these elements using the correct syntax: `selector { property: value; }`.

### Task 3: Selectors

1. Demonstrate the use of the following CSS selectors in your HTML and CSS:
    - **Element Selector**: Target all instances of a specific element.
    - **Class Selector**: Target elements with a specific class attribute.
    - **ID Selector**: Target an element with a specific id attribute.
    - **Group Selector**: Apply the same style to multiple elements.

### Task 4: Properties and Values

1. Use a variety of CSS properties and values to style your HTML elements. Include at least the following properties:
    - **Color**
    - **Font Size**
    - **Background Color**
    - **Margin**
    - **Padding**
    - **Border**

### Task 5: Creating a Simple Webpage

1. Create a complete HTML document that includes:
    - A header with a title.
    - A main content area with various HTML elements (e.g., paragraphs, headings).
    - Proper CSS styles applied using all three methods of including CSS.

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Introduction to CSS</title>
    <style>
        /* Internal CSS */
        p {
            color: blue;
        }
    </style>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <h1 style="color: red;">Welcome to CSS</h1> <!-- Inline CSS -->
    <p class="intro">This is an introduction to CSS.</p>
    <p id="main">CSS makes the web beautiful!</p>
</body>
</html>
```

**CSS (styles.css)**:

```
/* External CSS */

/* Class Selector */
.intro {
    font-size: 20px;
    color: darkgreen;
}

/* ID Selector */
#main {
    background-color: lightgray;
    padding: 10px;
    border: 1px solid black;
}
```

## Submission

Submit your `homework_lesson6.html` file and optional `styles.css` file via the designated submission platform.


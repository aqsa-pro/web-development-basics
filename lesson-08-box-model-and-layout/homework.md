
# Homework: Box Model and Layout in CSS

## Instructions

Complete the following tasks to practice using the CSS Box Model and layout properties. Submit your work as a single HTML file named `homework_lesson8.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: The CSS Box Model

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Create an element and apply styles to demonstrate each part of the CSS Box Model:
    - **Content**: Define the content area.
    - **Padding**: Add padding around the content.
    - **Border**: Add a border around the padding.
    - **Margin**: Add a margin outside the border.

### Task 2: Margins, Borders, Padding, and Content

1. Create multiple elements and apply different margins, borders, padding, and content areas. Use individual and shorthand properties for each.
    - Example: `margin`, `margin-top`, `margin-right`, `margin-bottom`, `margin-left`
    - Example: `padding`, `padding-top`, `padding-right`, `padding-bottom`, `padding-left`
    - Example: `border`, `border-width`, `border-style`, `border-color`

### Task 3: Understanding Layout with CSS

1. Demonstrate the use of various layout properties such as `display`, `position`, `float`, and `clear`.
    - Create elements with different display properties: block, inline, inline-block, and none.
    - Use positioning properties: static, relative, absolute, fixed.
    - Apply float and clear properties to elements.

### Task 4: Display Properties

1. Create examples of block elements, inline elements, and inline-block elements. Style them to highlight the differences in their behaviors.

### Task 5: Creating a Simple Layout

1. Create a complete HTML document that includes:
    - A header with a title.
    - A main content area with sections and aside elements.
    - A footer.
    - Proper CSS styles applied using all methods (inline, internal, external) to demonstrate the CSS Box Model and layout properties.

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Box Model and Layout</title>
    <style>
        /* Internal CSS */
        .content-box {
            padding: 20px;
            border: 2px solid black;
            margin: 10px;
            background-color: lightgrey;
        }
    </style>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to the Box Model</h1>
    </header>
    <main>
        <section class="content-box">
            <h2>Content Box</h2>
            <p>This box demonstrates the CSS Box Model.</p>
        </section>
        <aside class="content-box">
            <h2>Side Box</h2>
            <p>This is a side box with a different style.</p>
        </aside>
    </main>
    <footer>
        <p>Footer Content</p>
    </footer>
</body>
</html>
```

**CSS (styles.css)**:

```
/* External CSS */

/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

/* Header */
header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 0;
    text-align: center;
}

/* Main Content */
main {
    display: flex;
    justify-content: space-around;
    padding: 20px;
}

.content-box {
    background-color: #f9f9f9;
    border: 1px solid #ddd;
    padding: 20px;
    width: 30%;
}

/* Footer */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}
```


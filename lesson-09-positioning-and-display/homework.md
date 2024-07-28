
# Homework: Positioning and Display in CSS

## Instructions

Complete the following tasks to practice using CSS positioning and display properties. Submit your work as a single HTML file named `homework_lesson9.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: CSS Position Property

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Demonstrate the use of different values for the `position` property:
    - **Static Positioning**: Create an element with static positioning.
    - **Relative Positioning**: Create an element with relative positioning.
    - **Absolute Positioning**: Create an element with absolute positioning.
    - **Fixed Positioning**: Create an element with fixed positioning.
    - **Sticky Positioning**: Create an element with sticky positioning.

### Task 2: CSS Display Property

1. Demonstrate the use of different values for the `display` property:
    - **Block**: Create a block-level element.
    - **Inline**: Create an inline element.
    - **Inline-Block**: Create an inline-block element.
    - **None**: Create an element that is hidden.
    - **Flex**: Create a flex container.
    - **Grid**: Create a grid container.

### Task 3: Combining Positioning and Display

1. Create a complete HTML document that includes:
    - A header with a title.
    - A main content area with sections demonstrating different positioning and display properties.
    - A footer.
    - Proper CSS styles applied using all methods (inline, internal, external) to demonstrate the positioning and display properties.

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Positioning and Display</title>
    <style>
        /* Internal CSS */
        .relative {
            position: relative;
            top: 20px;
            left: 20px;
        }
    </style>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <header>
        <h1>Positioning and Display</h1>
    </header>
    <main>
        <section class="static">
            <h2>Static Positioning</h2>
            <p>This box uses static positioning.</p>
        </section>
        <section class="relative">
            <h2>Relative Positioning</h2>
            <p>This box uses relative positioning.</p>
        </section>
        <section class="absolute">
            <h2>Absolute Positioning</h2>
            <p>This box uses absolute positioning.</p>
        </section>
        <section class="fixed">
            <h2>Fixed Positioning</h2>
            <p>This box uses fixed positioning.</p>
        </section>
        <section class="sticky">
            <h2>Sticky Positioning</h2>
            <p>This box uses sticky positioning.</p>
        </section>
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

header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 0;
    text-align: center;
}

main {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
}

section {
    border: 1px solid #ddd;
    margin: 10px;
    padding: 20px;
    width: 80%;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}

/* Static Positioning */
.static {
    position: static;
}

/* Relative Positioning */
.relative {
    position: relative;
    top: 20px;
    left: 20px;
}

/* Absolute Positioning */
.absolute {
    position: absolute;
    top: 100px;
    left: 50%;
    transform: translateX(-50%);
}

/* Fixed Positioning */
.fixed {
    position: fixed;
    bottom: 10px;
    right: 10px;
    background-color: rgba(255, 255, 255, 0.8);
    border: 1px solid #000;
}

/* Sticky Positioning */
.sticky {
    position: sticky;
    top: 0;
    background-color: #f9f9f9;
    z-index: 1;
}
```

## Submission

Submit your `homework_lesson9.html` file and optional `styles.css` file via the designated submission platform.



# Homework: Page Layout with CSS

## Instructions

Complete the following tasks to practice using CSS layout techniques. Submit your work as a single HTML file named `homework_lesson12.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: Using Flexbox for Layout

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Create a flex container with multiple flex items:
    - **Flex Container**: An element with `display: flex`.
    - **Flex Items**: Child elements of the flex container.
    - **Apply Flexbox properties**: Use properties like `flex-direction`, `justify-content`, and `align-items`.

### Task 2: Using CSS Grid for Layout

1. Create a grid container with multiple grid items:
    - **Grid Container**: An element with `display: grid`.
    - **Grid Items**: Child elements of the grid container.
    - **Apply Grid properties**: Use properties like `grid-template-columns`, `grid-gap`, and `grid-template-rows`.

### Task 3: Creating a Basic Webpage Layout

1. Create a complete HTML document that includes:
    - A header with a title.
    - A navigation bar with links.
    - A main content area with sections for main content and a sidebar.
    - A footer.
    - Use either Flexbox or Grid to layout the page.

### Task 4: Responsive Design

1. Apply responsive design principles to your webpage layout:
    - Use media queries to adjust the layout for different screen sizes.
    - Ensure that the webpage is usable and looks good on both desktop and mobile devices.

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Page Layout with CSS</title>
    <style>
        /* Internal CSS */
        .flex-container {
            display: flex;
            flex-direction: row;
            justify-content: space-around;
            align-items: center;
        }
    </style>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <header>
        <h1>My Website</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
    <main>
        <section class="content">
            <h2>Main Content</h2>
            <p>This is the main content area.</p>
        </section>
        <aside class="sidebar">
            <h2>Sidebar</h2>
            <p>This is the sidebar content.</p>
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

header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 0;
    text-align: center;
}

nav {
    background-color: #333;
    color: white;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 20px;
}

.content {
    flex: 3;
    background-color: #f9f9f9;
    padding: 20px;
    margin-right: 20px;
}

.sidebar {
    flex: 1;
    background-color: #f4f4f4;
    padding: 20px;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

/* Responsive Design */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
        align-items: center;
    }

    main {
        flex-direction: column;
    }

    .content {
        margin-right: 0;
    }
}
```

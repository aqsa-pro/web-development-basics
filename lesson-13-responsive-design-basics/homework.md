
# Homework: Responsive Design Basics

## Instructions

Complete the following tasks to practice implementing responsive design using flexible grids, images, and media queries. Submit your work as a single HTML file named `homework_lesson13.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: Flexible Grid Layouts

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Create a flexible grid layout using relative units (like percentages) to define the width of grid items:
    - **Grid Container**: An element with `display: flex` and `flex-wrap: wrap`.
    - **Grid Items**: Child elements of the grid container with flexible widths based on screen size.

### Task 2: Responsive Images

1. Add images to your HTML file and make them responsive:
    - **Responsive Images**: Use CSS properties to ensure images scale appropriately within their containing elements.

### Task 3: Media Queries

1. Implement media queries to apply different styles based on screen size, resolution, or orientation:
    - **Basic Media Queries**: Apply different styles for different screen sizes.
    - **Combined Media Queries**: Apply styles for specific ranges of screen sizes.
    - **Layout Adjustments**: Use media queries to hide or show elements based on screen size.

### Task 4: Creating a Simple Responsive Webpage

1. Create a complete HTML document that includes:
    - A header with a title.
    - A navigation bar with links.
    - A main content area with sections for main content and a sidebar.
    - A footer.
    - Use flexible grids and media queries to make the layout responsive.

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Responsive Design Basics</title>
    <style>
        /* Internal CSS */
        .container {
            display: flex;
            flex-wrap: wrap;
        }

        .item {
            flex: 1 1 100%; /* Default to full width */
        }

        @media (min-width: 600px) {
            .item {
                flex: 1 1 50%; /* 2 columns on medium screens */
            }
        }

        @media (min-width: 900px) {
            .item {
                flex: 1 1 33.33%; /* 3 columns on large screens */
            }
        }
    </style>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <header>
        <h1>Responsive Design Basics</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
    <main class="container">
        <section class="item">
            <h2>Section 1</h2>
            <p>This is the first section of the responsive design example.</p>
            <img src="https://via.placeholder.com/400" alt="Placeholder Image">
        </section>
        <section class="item">
            <h2>Section 2</h2>
            <p>This is the second section of the responsive design example.</p>
            <img src="https://via.placeholder.com/400" alt="Placeholder Image">
        </section>
        <aside class="sidebar item">
            <h2>Sidebar</h2>
            <p>This is the sidebar content, visible on larger screens.</p>
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

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    background-color: #333;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    padding: 10px;
    display: block;
}

main {
    display: flex;
    flex-wrap: wrap;
    padding: 20px;
}

.item {
    flex: 1 1 100%;
    padding: 20px;
    box-sizing: border-box;
}

.sidebar {
    display: none;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}

/* Responsive Styles */
@media (min-width: 600px) {
    .item {
        flex: 1 1 50%; /* 2 columns on medium screens */
    }
}

@media (min-width: 900px) {
    .item {
        flex: 1 1 33.33%; /* 3 columns on large screens */
    }

    .sidebar {
        display: block;
        flex: 1 1 100%;
    }
}

img {
    max-width: 100%;
    height: auto;
}
```

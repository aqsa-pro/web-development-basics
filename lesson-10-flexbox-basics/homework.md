
# Homework: Flexbox Basics

## Instructions

Complete the following tasks to practice using CSS Flexbox properties. Submit your work as a single HTML file named `homework_lesson10.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: Flex Containers and Flex Items

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Create a flex container with multiple flex items:
    - **Flex Container**: An element with `display: flex`.
    - **Flex Items**: Child elements of the flex container.

### Task 2: Flex Direction

1. Demonstrate the use of different values for the `flex-direction` property:
    - **Row**: Create a flex container with flex items arranged in a row.
    - **Row-Reverse**: Create a flex container with flex items arranged in a reversed row.
    - **Column**: Create a flex container with flex items arranged in a column.
    - **Column-Reverse**: Create a flex container with flex items arranged in a reversed column.

### Task 3: Justify Content

1. Demonstrate the use of different values for the `justify-content` property:
    - **Flex Start**: Align items to the start of the container.
    - **Flex End**: Align items to the end of the container.
    - **Center**: Center the items along the main axis.
    - **Space Between**: Distribute items with space between them.
    - **Space Around**: Distribute items with space around them.
    - **Space Evenly**: Distribute items with equal space around them.

### Task 4: Align Items and Align Self

1. Demonstrate the use of the `align-items` property:
    - **Stretch**: Stretch items to fill the container.
    - **Flex Start**: Align items to the start of the cross axis.
    - **Flex End**: Align items to the end of the cross axis.
    - **Center**: Center items along the cross axis.
    - **Baseline**: Align items along their baseline.

2. Demonstrate the use of the `align-self` property for individual flex items.

### Task 5: Flex Wrap

1. Demonstrate the use of different values for the `flex-wrap` property:
    - **No Wrap**: Do not wrap items.
    - **Wrap**: Wrap items to the next line.
    - **Wrap-Reverse**: Wrap items to the next line in reverse order.

### Task 6: Flex Grow, Flex Shrink, and Flex Basis

1. Demonstrate the use of the `flex-grow`, `flex-shrink`, and `flex-basis` properties:
    - **Flex Grow**: Create a flex item that can grow.
    - **Flex Shrink**: Create a flex item that can shrink.
    - **Flex Basis**: Set the initial size of a flex item.

### Task 7: Creating a Responsive Layout with Flexbox

1. Create a complete HTML document that includes:
    - A header with a title.
    - A main content area with a flex container and flex items demonstrating the various Flexbox properties.
    - A footer.
    - Proper CSS styles applied using all methods (inline, internal, external) to demonstrate Flexbox properties.

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Flexbox Basics</title>
    <style>
        /* Internal CSS */
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            padding: 20px;
            background-color: #f9f9f9;
        }
    </style>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <header>
        <h1>Flexbox Basics</h1>
    </header>
    <main>
        <div class="container">
            <div class="item">Item 1</div>
            <div class="item">Item 2</div>
            <div class="item">Item 3</div>
        </div>
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

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

/* Flex Container */
.container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-wrap: wrap;
    padding: 20px;
    background-color: #f9f9f9;
}

/* Flex Items */
.item {
    background-color: #ddd;
    border: 1px solid #ccc;
    padding: 20px;
    flex: 1;
    margin: 10px;
    text-align: center;
    font-size: 1.2em;
}
```

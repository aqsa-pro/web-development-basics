
# Homework: Styling Text and Links

## Instructions

Complete the following tasks to practice using CSS to style text and links. Submit your work as a single HTML file named `homework_lesson11.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: Basic Text Styling

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Demonstrate the use of different text styling properties:
    - **Font Size**: Set the font size of a paragraph.
    - **Font Family**: Set the font family of a paragraph.
    - **Font Weight**: Set the font weight of a paragraph.
    - **Font Style**: Set the font style of a paragraph.
    - **Text Color**: Set the color of a paragraph.

### Task 2: Text Alignment and Transformation

1. Demonstrate the use of text alignment and transformation properties:
    - **Text Alignment**: Align text to the center, left, and right.
    - **Text Transformation**: Transform text to uppercase, lowercase, and capitalize.

### Task 3: Text Decoration

1. Demonstrate the use of text decoration properties:
    - **Text Decoration**: Add underline, line-through, and remove text decorations.
    - **Text Shadow**: Apply a shadow to text.

### Task 4: Styling Links

1. Create styled links with different properties:
    - **Basic Link Styling**: Style a link with color and text decoration.
    - **Link Pseudo-Classes**: Style links for different states (link, visited, hover, active).

### Task 5: Combining Text and Link Styling

1. Create a complete HTML document that includes:
    - A header with a title.
    - A main content area with sections demonstrating various text and link styling techniques.
    - A footer.
    - Proper CSS styles applied using all methods (inline, internal, external) to demonstrate text and link styling.

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Styling Text and Links</title>
    <style>
        /* Internal CSS */
        p.uppercase {
            text-transform: uppercase;
        }
    </style>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <header>
        <h1>Styling Text and Links</h1>
    </header>
    <main>
        <section>
            <h2>Basic Text Styling</h2>
            <p class="intro">This paragraph demonstrates basic text styling with font size, family, weight, style, and color.</p>
        </section>
        <section>
            <h2>Text Alignment and Transformation</h2>
            <p class="uppercase">This text is uppercase.</p>
            <p class="lowercase">This text is lowercase.</p>
            <p class="capitalize">this text is capitalized.</p>
        </section>
        <section>
            <h2>Text Decoration</h2>
            <p class="underline">This text is underlined.</p>
            <p class="line-through">This text is line-through.</p>
            <h2 class="shadow">This heading has a shadow.</h2>
        </section>
        <section>
            <h2>Styling Links</h2>
            <a href="https://www.example.com" class="link">This is a styled link</a>
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

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

/* Basic Text Styling */
p.intro {
    font-size: 16px;
    font-family: 'Arial', sans-serif;
    font-weight: bold;
    font-style: italic;
    color: #333;
}

/* Text Alignment and Transformation */
.uppercase {
    text-transform: uppercase;
}

.lowercase {
    text-transform: lowercase;
}

.capitalize {
    text-transform: capitalize;
}

/* Text Decoration */
.underline {
    text-decoration: underline;
}

.line-through {
    text-decoration: line-through;
}

.shadow {
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
}

/* Styling Links */
a.link {
    color: #0066cc;
    text-decoration: none;
}

a.link:hover {
    text-decoration: underline;
}

/* Link Pseudo-Classes */
a:link {
    color: blue; /* Unvisited link */
}

a:visited {
    color: purple; /* Visited link */
}

a:hover {
    color: red; /* Mouse over link */
}

a:active {
    color: orange; /* Selected link */
}
```

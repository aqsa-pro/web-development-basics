
# Homework: Color and Typography in CSS

## Instructions

Complete the following tasks to practice using CSS to set colors and typography. Submit your work as a single HTML file named `homework_lesson7.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: Setting Colors in CSS

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Demonstrate the use of different color values in CSS:
    - **Color Names**: Apply a color using a color name.
    - **HEX Values**: Apply a color using a HEX value.
    - **RGB Values**: Apply a color using an RGB value.
    - **RGBA Values**: Apply a color using an RGBA value (include opacity).
    - **HSL Values**: Apply a color using an HSL value.
    - **Setting Background Colors**: Apply a background color to an element.

### Task 2: Typography Basics

1. In your HTML file, create multiple HTML elements (e.g., paragraphs, headings, divs).
2. Apply basic typography styles to these elements:
    - **Font Family**: Set a font family for the body or specific elements.
    - **Font Size**: Set the font size for different elements.
    - **Font Weight**: Set the font weight for some text.
    - **Font Style**: Apply italic or oblique styles to some text.

### Task 3: Font Properties

1. Demonstrate the use of various font properties in your HTML and CSS:
    - **Font Family**: Use different font families.
    - **Font Size**: Apply different font sizes using various units (e.g., px, em).
    - **Font Weight**: Apply different font weights.
    - **Font Style**: Apply different font styles.
    - **Font Variant**: Use small-caps for some text.

### Task 4: Text Properties

1. Apply various text properties to your HTML elements:
    - **Text Color**: Set the color of the text.
    - **Text Alignment**: Align the text within its container.
    - **Line Height**: Set the space between lines of text.
    - **Letter Spacing**: Adjust the space between letters.
    - **Text Decoration**: Add or remove text decorations (e.g., underline).
    - **Text Transform**: Control the capitalization of text.

### Task 5: Creating a Simple Webpage

1. Create a complete HTML document that includes:
    - A header with a title.
    - A main content area with various HTML elements styled with colors and typography.
    - Proper CSS styles applied using all methods (inline, internal, external).

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Color and Typography</title>
    <style>
        /* Internal CSS */
        p {
            color: blue;
        }
    </style>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <h1 style="color: red;">Welcome to Color and Typography</h1> <!-- Inline CSS -->
    <p class="intro">This is an introduction to color and typography in CSS.</p>
    <p class="highlight">CSS allows you to control the appearance of text and the use of colors.</p>
    <p class="uppercase">This text is uppercase.</p>
    <p class="small-caps">This text is in small caps.</p>
    <a href="#" class="link">This is a link with no underline.</a>
</body>
</html>
```

**CSS (styles.css)**:

```
/* External CSS */

/* Basic Color and Background Color */
body {
    background-color: #f0f0f0;
    color: #333;
    font-family: Arial, sans-serif;
}

/* Headings */
h1 {
    color: #2c3e50;
    font-size: 2.5em;
    text-align: center;
}

/* Paragraphs */
p {
    font-size: 16px;
    line-height: 1.5;
}

/* Intro Paragraph */
.intro {
    color: #2980b9;
    font-size: 1.2em;
    font-style: italic;
}

/* Highlight Paragraph */
.highlight {
    background-color: #ffeb3b;
    font-weight: bold;
}

/* Uppercase Text */
.uppercase {
    text-transform: uppercase;
}

/* Small Caps Text */
.small-caps {
    font-variant: small-caps;
}

/* Link */
.link {
    color: #e74c3c;
    text-decoration: none;
    font-weight: bold;
    letter-spacing: 1px;
}
```

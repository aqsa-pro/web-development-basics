
# Homework: Building a Simple Web Page

## Instructions

Complete the following tasks to build a complete web page using HTML and CSS. Submit your work as a single HTML file named `homework_lesson14.html` and an optional CSS file named `styles.css` if you use external CSS.

## Tasks

### Task 1: Planning the Web Page

1. Plan the structure and content of your web page. The web page should include the following sections:
    - Header with navigation
    - Hero section with an introduction
    - About section
    - Portfolio section
    - Contact section
    - Footer

### Task 2: Creating the HTML Structure

1. Create a new HTML file and add the standard `<!DOCTYPE html>` declaration and basic HTML structure with `<html>`, `<head>`, and `<body>` tags.
2. Create the HTML structure for the planned web page sections.

### Task 3: Adding Styles with CSS

1. Create a new CSS file (if using external CSS) and link it to your HTML file.
2. Add styles to your web page to make it visually appealing.

### Task 4: Making the Web Page Responsive

1. Use media queries to ensure the web page looks good on different screen sizes.

### Task 5: Final Touches and Testing

1. Ensure all links work correctly.
2. Validate HTML and CSS for errors.
3. Test the web page on different devices and screen sizes to ensure responsiveness.
4. Add any additional content or styles to improve the web page.

### Example Structure

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>My Portfolio</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    <section id="home" class="hero">
        <h1>Welcome to My Portfolio</h1>
        <p>Hi, I'm [Your Name], a web developer.</p>
    </section>
    <section id="about" class="about">
        <h2>About Me</h2>
        <p>This is the about section where you can introduce yourself.</p>
    </section>
    <section id="portfolio" class="portfolio">
        <h2>My Work</h2>
        <div class="portfolio-item">
            <h3>Project 1</h3>
            <p>Description of project 1.</p>
        </div>
        <div class="portfolio-item">
            <h3>Project 2</h3>
            <p>Description of project 2.</p>
        </div>
        <div class="portfolio-item">
            <h3>Project 3</h3>
            <p>Description of project 3.</p>
        </div>
    </section>
    <section id="contact" class="contact">
        <h2>Contact Me</h2>
        <form>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            <input type="submit" value="Send">
        </form>
    </section>
    <footer>
        <p>&copy; 2024 My Portfolio</p>
    </footer>
</body>
</html>
```

**CSS (styles.css)**:

```
/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
}

header {
    background: #333;
    color: #fff;
    padding: 10px 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

.hero {
    background: #f4f4f4;
    padding: 60px 20px;
    text-align: center;
}

.hero h1 {
    margin: 0;
    font-size: 2.5em;
}

.about, .portfolio, .contact {
    padding: 40px 20px;
    text-align: center;
}

.portfolio-item {
    background: #f4f4f4;
    margin: 20px 0;
    padding: 20px;
}

form {
    max-width: 600px;
    margin: 0 auto;
    text-align: left;
}

form label {
    display: block;
    margin: 10px 0 5px;
}

form input, form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
}

form input[type="submit"] {
    background: #333;
    color: #fff;
    border: 0;
    padding: 15px 20px;
    cursor: pointer;
}

footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

/* Responsive Styles */
@media (max-width: 768px) {
    nav ul li {
        display: block;
        margin: 10px 0;
    }

    .hero h1 {
        font-size: 2em;
    }

    form input, form textarea {
        width: 100%;
    }
}

@media (max-width: 480px) {
    .hero {
        padding: 40px 10px;
    }

    .about, .portfolio, .contact {
        padding: 20px 10px;
    }
}
```

## Submission

Submit your `homework_lesson14.html` file and optional `styles.css` file via the designated submission platform.


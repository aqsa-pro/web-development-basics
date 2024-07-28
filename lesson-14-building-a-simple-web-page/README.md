### Lesson 14: Building a Simple Web Page

#### Objectives:

* Apply the knowledge gained from previous lessons to build a complete web page
* Combine HTML and CSS skills to create a structured, styled, and responsive web page
* Understand the process of developing a web page from start to finish

#### Lesson Outline:

1.  **Planning the Web Page**
2.  **Creating the HTML Structure**
3.  **Adding Styles with CSS**
4.  **Making the Web Page Responsive**
5.  **Final Touches and Testing**

* * *

#### 1\. Planning the Web Page

Before building a web page, it’s important to plan its structure and content. For this lesson, we’ll create a simple personal portfolio web page with the following sections:

* Header with navigation
* Hero section with an introduction
* About section
* Portfolio section
* Contact section
* Footer

#### 2\. Creating the HTML Structure

We’ll start by creating the HTML structure for the web page.

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

#### 3\. Adding Styles with CSS

Next, we’ll add CSS to style the web page and make it visually appealing.

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
``` 

#### 4\. Making the Web Page Responsive

We’ll use media queries to ensure the web page looks good on different screen sizes.

**CSS (styles.css)**:

```
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

#### 5\. Final Touches and Testing

* Ensure all links work correctly.
* Validate HTML and CSS for errors.
* Test the web page on different devices and screen sizes to ensure responsiveness.
* Add any additional content or styles to improve the web page.

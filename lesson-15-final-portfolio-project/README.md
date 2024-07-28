### Lesson 15: Final Project and Review

#### Objectives:

* Apply all the concepts learned in previous lessons to create a comprehensive final project
* Review key HTML and CSS concepts
* Practice problem-solving and debugging skills
* Prepare for real-world web development tasks

#### Lesson Outline:

1.  **Final Project Overview**
2.  **Project Requirements**
3.  **Creating the Project**
4.  **Reviewing Key Concepts**
5.  **Testing and Debugging**
6.  **Submission and Presentation**

* * *

#### 1\. Final Project Overview

For the final project, you will create a multi-page personal portfolio website. This project will incorporate all the HTML and CSS skills you have learned throughout the course. The portfolio website should be responsive and include the following pages:

* Home
* About
* Portfolio
* Contact

Each page will have its own unique content, but the overall design should be cohesive and consistent.

#### 2\. Project Requirements

* **Home Page**:
    
    * Introduction with a brief bio
    * Links to other sections (About, Portfolio, Contact)
* **About Page**:
    
    * Detailed information about yourself
    * Your background, skills, and interests
* **Portfolio Page**:
    
    * Showcase your projects
    * Each project should have a title, description, and image
* **Contact Page**:
    
    * Contact form with fields for name, email, and message
    * Contact information (email, phone number, social media links)
* **General Requirements**:
    
    * Consistent navigation menu on all pages
    * Responsive design for various screen sizes
    * Use of Flexbox or Grid for layout
    * Proper use of semantic HTML elements
    * Clean and well-organized CSS

#### 3\. Creating the Project

**Step-by-Step Guide**:

1.  **Set Up the Project Structure**:
    
    * Create a new directory for the project.
    * Inside the directory, create subdirectories for each page (`home`, `about`, `portfolio`, `contact`).
    * Create an `index.html` file in the root directory and individual HTML files for each page.
2.  **HTML Structure**:
    
    * Create the basic HTML structure for each page.
    * Include the navigation menu in each HTML file.
3.  **CSS Styling**:
    
    * Create a `styles.css` file in a `css` directory.
    * Link the `styles.css` file to all HTML pages.
    * Add styling for the navigation menu, headers, paragraphs, images, forms, etc.
4.  **Responsive Design**:
    
    * Use media queries to ensure the website is responsive.
    * Test the website on different devices and screen sizes.

**Example Project Structure**:

arduino

Copy code

```
my-portfolio/
├── css/
│   └── styles.css
├── home/
│   └── index.html
├── about/
│   └── index.html
├── portfolio/
│   └── index.html
├── contact/
│   └── index.html
└── index.html
``` 

#### 4\. Reviewing Key Concepts

**HTML Concepts**:

* Semantic elements (`<header>`, `<nav>`, `<section>`, `<article>`, `<footer>`)
* Forms and input fields
* Links and images
* Lists and tables

**CSS Concepts**:

* Box model (margin, border, padding, content)
* Flexbox and Grid layouts
* Responsive design with media queries
* Text and link styling
* Color and typography

#### 5\. Testing and Debugging

* **Validation**:
    
    * Validate your HTML and CSS using the W3C validators.
    * Ensure there are no errors or warnings.
* **Cross-Browser Testing**:
    
    * Test your website on different browsers (Chrome, Firefox, Safari, Edge).
    * Ensure consistent behavior and appearance across all browsers.
* **Responsiveness**:
    
    * Test your website on different devices (desktops, tablets, mobile phones).
    * Ensure the layout adapts properly to different screen sizes.
* **Debugging**:
    
    * Use browser developer tools to inspect elements and debug CSS issues.
    * Fix any layout or styling issues that arise.

#### 6\. Submission and Presentation

* **Submission**:
    
    * Upload your project to GitHub.
    * Ensure your repository is well-organized with clear commit messages.
* **Presentation**:
    
    * Prepare a brief presentation of your project.
    * Explain the design choices you made and the challenges you faced.
    * Demonstrate the responsiveness and functionality of your website.

**GitHub Repository Instructions**:

1.  **Create a Repository**:
    
    * Create a new repository on GitHub named `final-portfolio-project`.
2.  **Clone the Repository**:
    
    * Clone the repository to your local machine:
        
        ```
        git clone https://github.com/your-username/final-portfolio-project.git
        cd final-portfolio-project
        ``` 
        
3.  **Add Project Files**:
    
    * Add your project files to the repository.
4.  **Commit and Push**:
    
    * Add, commit, and push your changes to GitHub:
        
        ```
        git add .
        git commit -m "Add final portfolio project"
        git push origin main
        ```
        
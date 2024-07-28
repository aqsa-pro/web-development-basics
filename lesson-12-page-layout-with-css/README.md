### Lesson 12: Page Layout with CSS

#### Objectives:

* Understand different CSS layout techniques
* Learn how to use Flexbox and Grid for layout
* Create a basic webpage layout with a header, navigation, main content, and footer
* Apply responsive design principles

#### Lesson Outline:

1.  **Introduction to CSS Layout Techniques**
2.  **Using Flexbox for Layout**
3.  **Using CSS Grid for Layout**
4.  **Creating a Basic Webpage Layout**
5.  **Responsive Design**

* * *

#### 1\. Introduction to CSS Layout Techniques

CSS provides several layout techniques to control the arrangement of elements on a webpage. The most common techniques include:

* **Float Layout**: Uses the `float` property to create multi-column layouts.
* **Flexbox**: A one-dimensional layout method for arranging items in rows or columns.
* **CSS Grid**: A two-dimensional layout method for creating complex grid-based layouts.

#### 2\. Using Flexbox for Layout

Flexbox is ideal for creating flexible and responsive layouts. It simplifies the process of aligning and distributing space among items in a container.

* **Flex Container**:
    
    ```
    .flex-container {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
    }
    ``` 
    
* **Flex Items**:
    
    ```
    .flex-item {
        flex: 1;
        padding: 10px;
    }
    ``` 
    

#### 3\. Using CSS Grid for Layout

CSS Grid is a powerful tool for creating complex and responsive grid-based layouts. It allows you to define rows and columns and place items within the grid.

* **Grid Container**:
    
    ```
    .grid-container {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-gap: 10px;
    }
    ``` 
    
* **Grid Items**:
    
    ```
    .grid-item {
        padding: 20px;
        background-color: #f4f4f4;
    }
    ``` 
    

#### 4\. Creating a Basic Webpage Layout

Let's create a basic webpage layout with a header, navigation, main content, and footer using Flexbox and Grid.

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Page Layout with CSS</title>
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
``` 

#### 5\. Responsive Design

Responsive design ensures that your webpage looks good on all devices, from desktops to mobile phones. You can achieve this using media queries.

**Media Queries Example**:

```
/* General styles for larger screens */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header, footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}

nav ul {
    display: flex;
    justify-content: center;
}

main {
    display: flex;
    flex-direction: row;
    padding: 20px;
}

.content {
    flex: 3;
    margin-right: 20px;
}

.sidebar {
    flex: 1;
}

/* Media query for smaller screens */
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

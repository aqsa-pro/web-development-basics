### Lesson 13: Responsive Design Basics

#### Objectives:

* Understand the principles of responsive design
* Learn about media queries and how to use them
* Implement responsive design techniques using flexible grids, images, and media queries
* Create a simple responsive webpage layout

#### Lesson Outline:

1.  **Introduction to Responsive Design**
2.  **Flexible Grid Layouts**
3.  **Responsive Images**
4.  **Media Queries**
5.  **Creating a Simple Responsive Webpage**

* * *

#### 1\. Introduction to Responsive Design

Responsive design is an approach to web development that makes web pages render well on various devices and window sizes. It ensures that the user experience is optimized across desktops, tablets, and mobile devices.

* **Key Principles**:
    * Fluid Grid Layouts: Using relative units like percentages instead of fixed units like pixels.
    * Flexible Images: Ensuring images scale appropriately within their containing elements.
    * Media Queries: Applying different styles based on the screen size and orientation.

#### 2\. Flexible Grid Layouts

A flexible grid layout uses relative units (like percentages) to create a grid that adapts to different screen sizes.

* **Example**:

    ```
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
    ``` 
    

#### 3\. Responsive Images

Responsive images adjust their size to fit within their containing element, ensuring they look good on all screen sizes.

* **Example**:

    ```
    img {
        max-width: 100%;
        height: auto;
    }
    ``` 
    
* **HTML**:

    ```
    <img src="image.jpg" alt="Responsive Image">
    ``` 
    

#### 4\. Media Queries

Media queries are used to apply different CSS rules based on the screen size, resolution, or orientation.

* **Basic Media Query**:

    ```
    @media (max-width: 600px) {
        body {
            background-color: lightblue;
        }
    }
    ``` 
    
* **Combining Media Queries**:

    ```
    @media (min-width: 600px) and (max-width: 900px) {
        body {
            background-color: lightgreen;
        }
    }
    ``` 
    
* **Using Media Queries for Layout**:

    ```
    .sidebar {
        display: none;
    }
    
    @media (min-width: 800px) {
        .sidebar {
            display: block;
        }
    }
    ``` 
    

#### 5\. Creating a Simple Responsive Webpage

Let's create an HTML document that demonstrates responsive design principles:

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Responsive Design Basics</title>
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
``` 

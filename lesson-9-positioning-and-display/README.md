### Lesson 9: Positioning and Display

#### Objectives:

* Understand different CSS positioning methods
* Learn about the `position` property and its values
* Explore the `display` property and its values
* Combine positioning and display properties to create complex layouts

#### Lesson Outline:

1.  **CSS Position Property**
2.  **Static Positioning**
3.  **Relative Positioning**
4.  **Absolute Positioning**
5.  **Fixed Positioning**
6.  **Sticky Positioning**
7.  **CSS Display Property**
8.  **Combining Positioning and Display**

* * *

#### 1\. CSS Position Property

The `position` property in CSS allows you to control the layout and positioning of elements. The main values for the `position` property are `static`, `relative`, `absolute`, `fixed`, and `sticky`.

#### 2\. Static Positioning

* **Static** is the default positioning for HTML elements. Elements are positioned according to the normal document flow.

```
div {
    position: static;
}
``` 

#### 3\. Relative Positioning

* **Relative** positioning allows you to position an element relative to its normal position. Other elements are not affected by this positioning.

```
div {
    position: relative;
    top: 20px; /* Moves the element 20px down from its original position */
    left: 10px; /* Moves the element 10px to the right from its original position */
}
``` 

#### 4\. Absolute Positioning

* **Absolute** positioning allows you to position an element relative to its nearest positioned ancestor (not `static`). If no such ancestor exists, it is positioned relative to the initial containing block (the viewport).

```
div {
    position: absolute;
    top: 50px;
    left: 100px;
}
``` 

#### 5\. Fixed Positioning

* **Fixed** positioning allows you to position an element relative to the viewport. The element stays in the same position even when the page is scrolled.

```
div {
    position: fixed;
    top: 0;
    right: 0;
}
``` 

#### 6\. Sticky Positioning

* **Sticky** positioning allows an element to switch between relative and fixed positioning depending on the scroll position. It is positioned relative until a given offset position is met in the viewport, then it becomes fixed.

```
div {
    position: sticky;
    top: 0; /* The element becomes fixed when its top is at 0px from the viewport */
}
``` 

#### 7\. CSS Display Property

The `display` property specifies the display behavior of an element. Common values include `block`, `inline`, `inline-block`, `none`, `flex`, and `grid`.

* **Block**: The element takes up the full width available and starts on a new line.
    
    ```
    div {
        display: block;
    }
    ``` 
    
* **Inline**: The element takes up only as much width as necessary and does not start on a new line.
    
    ```
    span {
        display: inline;
    }
    ``` 
    
* **Inline-Block**: The element behaves like an inline element but can have width and height set.
    
    ```
    img {
        display: inline-block;
    }
    ``` 
    
* **None**: The element is not displayed at all.
    
    ```
    .hidden {
        display: none;
    }
    ``` 
    
* **Flex**: The element becomes a flex container.
    
    ```
    .container {
        display: flex;
    }
    ``` 
    
* **Grid**: The element becomes a grid container.
    
    ```
    .container {
        display: grid;
    }
    ``` 
    

#### 8\. Combining Positioning and Display

Let's create an HTML document that demonstrates different positioning and display properties:

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Positioning and Display</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <header>
        <h1>Positioning and Display</h1>
    </header>
    <main>
        <section class="static">
            <h2>Static Positioning</h2>
            <p>This box uses static positioning.</p>
        </section>
        <section class="relative">
            <h2>Relative Positioning</h2>
            <p>This box uses relative positioning.</p>
        </section>
        <section class="absolute">
            <h2>Absolute Positioning</h2>
            <p>This box uses absolute positioning.</p>
        </section>
        <section class="fixed">
            <h2>Fixed Positioning</h2>
            <p>This box uses fixed positioning.</p>
        </section>
        <section class="sticky">
            <h2>Sticky Positioning</h2>
            <p>This box uses sticky positioning.</p>
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

main {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
}

section {
    border: 1px solid #ddd;
    margin: 10px;
    padding: 20px;
    width: 80%;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}

/* Static Positioning */
.static {
    position: static;
}

/* Relative Positioning */
.relative {
    position: relative;
    top: 20px;
    left: 20px;
}

/* Absolute Positioning */
.absolute {
    position: absolute;
    top: 100px;
    left: 50%;
    transform: translateX(-50%);
}

/* Fixed Positioning */
.fixed {
    position: fixed;
    bottom: 10px;
    right: 10px;
    background-color: rgba(255, 255, 255, 0.8);
    border: 1px solid #000;
}

/* Sticky Positioning */
.sticky {
    position: sticky;
    top: 0;
    background-color: #f9f9f9;
    z-index: 1;
}
``` 

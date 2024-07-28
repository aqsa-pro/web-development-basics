### Lesson 10: Flexbox Basics

#### Objectives:

* Understand the basics of the CSS Flexbox layout model
* Learn how to use Flexbox properties to create responsive layouts
* Understand the concepts of flex containers and flex items
* Apply Flexbox properties to control the alignment, direction, and order of elements

#### Lesson Outline:

1.  **Introduction to Flexbox**
2.  **Flex Containers and Flex Items**
3.  **Flex Direction**
4.  **Justify Content**
5.  **Align Items and Align Self**
6.  **Flex Wrap**
7.  **Flex Grow, Flex Shrink, and Flex Basis**
8.  **Creating a Responsive Layout with Flexbox**

* * *

#### 1\. Introduction to Flexbox

Flexbox is a CSS layout model that allows you to create complex and flexible layouts with ease. It is designed to distribute space along a single axis (horizontal or vertical) and align items within a container.

* **Advantages of Flexbox**:
    * Simplifies the process of creating flexible and responsive layouts
    * Provides more control over alignment and spacing of items
    * Reduces the need for float and positioning hacks

#### 2\. Flex Containers and Flex Items

* **Flex Container**: An element that has `display: flex` or `display: inline-flex`. It serves as the parent element for flex items.

    ```
    .container {
        display: flex;
    }
    ``` 
    
* **Flex Items**: The child elements of a flex container. They can be controlled and aligned using various flexbox properties.

    ```
    <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
    </div>
    ``` 
    

#### 3\. Flex Direction

The `flex-direction` property defines the direction in which the flex items are placed in the flex container.

* **Row (default)**: Items are placed horizontally.

    ```
    .container {
        flex-direction: row;
    }
    ``` 
    
* **Row-Reverse**: Items are placed horizontally in reverse order.

    ```
    .container {
        flex-direction: row-reverse;
    }
    ``` 
    
* **Column**: Items are placed vertically.

    ```
    .container {
        flex-direction: column;
    }
    ``` 
    
* **Column-Reverse**: Items are placed vertically in reverse order.

    ```
    .container {
        flex-direction: column-reverse;
    }
    ``` 
    

#### 4\. Justify Content

The `justify-content` property aligns flex items along the main axis (horizontal by default).

* **Flex Start (default)**: Items are aligned to the start of the container.

    ```
    .container {
        justify-content: flex-start;
    }
    ``` 
    
* **Flex End**: Items are aligned to the end of the container.

    ```
    .container {
        justify-content: flex-end;
    }
    ``` 
    
* **Center**: Items are centered along the main axis.

    ```
    .container {
        justify-content: center;
    }
    ``` 
    
* **Space Between**: Items are evenly distributed with space between them.

    ```
    .container {
        justify-content: space-between;
    }
    ``` 
    
* **Space Around**: Items are evenly distributed with space around them.

    ```
    .container {
        justify-content: space-around;
    }
    ``` 
    
* **Space Evenly**: Items are evenly distributed with equal space around them.

    ```
    .container {
        justify-content: space-evenly;
    }
    ``` 
    

#### 5\. Align Items and Align Self

The `align-items` property aligns flex items along the cross axis (vertical by default).

* **Stretch (default)**: Items are stretched to fill the container.

    ```
    .container {
        align-items: stretch;
    }
    ``` 
    
* **Flex Start**: Items are aligned to the start of the cross axis.

    ```
    .container {
        align-items: flex-start;
    }
    ``` 
    
* **Flex End**: Items are aligned to the end of the cross axis.

    ```
    .container {
        align-items: flex-end;
    }
    ``` 
    
* **Center**: Items are centered along the cross axis.

    ```
    .container {
        align-items: center;
    }
    ``` 
    
* **Baseline**: Items are aligned along their baseline.

    ```
    .container {
        align-items: baseline;
    }
    ``` 
    

The `align-self` property allows individual flex items to be aligned independently of the other items.

* **Align Self Example**:

    ```
    .item {
        align-self: flex-start;
    }
    ``` 
    

#### 6\. Flex Wrap

The `flex-wrap` property specifies whether the flex items should wrap or not when they overflow the container.

* **No Wrap (default)**: Items do not wrap.

    ```
    .container {
        flex-wrap: nowrap;
    }
    ``` 
    
* **Wrap**: Items wrap to the next line.

    ```
    .container {
        flex-wrap: wrap;
    }
    ``` 
    
* **Wrap-Reverse**: Items wrap to the next line in reverse order.

    ```
    .container {
        flex-wrap: wrap-reverse;
    }
    ``` 
    

#### 7\. Flex Grow, Flex Shrink, and Flex Basis

* **Flex Grow**: Defines the ability for a flex item to grow if necessary.

    ```
    .item {
        flex-grow: 1;
    }
    ``` 
    
* **Flex Shrink**: Defines the ability for a flex item to shrink if necessary.

    ```
    .item {
        flex-shrink: 1;
    }
    ``` 
    
* **Flex Basis**: Defines the default size of an element before the remaining space is distributed.

    ```
    .item {
        flex-basis: 100px;
    }
    ``` 
    

#### 8\. Creating a Responsive Layout with Flexbox

Let's create an HTML document that demonstrates the use of Flexbox properties to create a responsive layout:

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Flexbox Basics</title>
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

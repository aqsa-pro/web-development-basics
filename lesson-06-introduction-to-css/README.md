### Lesson 6: Introduction to CSS

#### Objectives:

* Understand the basics of CSS
* Learn how to include CSS in HTML documents
* Understand the concept of selectors, properties, and values
* Apply basic styles to HTML elements

#### Lesson Outline:

1.  **What is CSS?**
2.  **Including CSS in HTML**
3.  **CSS Syntax**
4.  **Selectors**
5.  **Properties and Values**
6.  **Applying Basic Styles**

* * *

#### 1\. What is CSS?

CSS (Cascading Style Sheets) is a language used to describe the presentation of a document written in HTML or XML. CSS controls the layout, colors, fonts, and overall visual appearance of a webpage.

* **Advantages of CSS**:
    * Separation of content and presentation
    * Reusability of styles
    * Easier maintenance
    * Improved accessibility

#### 2\. Including CSS in HTML

There are three ways to include CSS in an HTML document:

* **Inline CSS**:
    
    * CSS is written directly within an HTML element's `style` attribute.
    
    ```
    <p style="color: red;">This is a red paragraph.</p>
    ``` 
    
* **Internal CSS**:
    
    * CSS is written within a `<style>` tag inside the `<head>` section of the HTML document.
    
    ```
    <head>
        <style>
            p {
                color: blue;
            }
        </style>
    </head>
    ``` 
    
* **External CSS**:
    
    * CSS is written in a separate `.css` file, and linked to the HTML document using the `<link>` tag.
    
    ```
    <head>
        <link rel="stylesheet" type="text/css" href="styles.css">
    </head>
    ``` 
    

#### 3\. CSS Syntax

CSS syntax consists of selectors, properties, and values:

```
selector {
    property: value;
}
```

* **Selector**: Specifies the HTML element(s) to be styled.
* **Property**: Specifies the style attribute to be applied.
* **Value**: Specifies the value of the style attribute.

#### 4\. Selectors

Selectors are used to target HTML elements for styling.

* **Element Selector**:
    
    * Targets all instances of a specific element.
    
    ```
    p {
        color: green;
    }
    ``` 
    
* **Class Selector**:
    
    * Targets elements with a specific class attribute. Class names are prefixed with a dot (`.`).
    
    ```
    .intro {
        font-size: 20px;
    }
    ``` 
    
    ```
    <p class="intro">This is an introductory paragraph.</p>
    ``` 
    
* **ID Selector**:
    
    * Targets an element with a specific id attribute. ID names are prefixed with a hash (`#`).
    
    ```
    #main {
        background-color: lightgray;
    }
    ``` 
    
    ```
    <div id="main">This is the main section.</div>
    ``` 
    
* **Group Selector**:
    
    * Applies the same style to multiple elements.
    
    ```
    h1, h2, h3 {
        color: navy;
    }
    ``` 
    

#### 5\. Properties and Values

CSS properties are used to define the styles for the selected elements. Here are some common properties and their values:

* **Color**:
    
    ```
    color: red;
    ``` 
    
* **Font Size**:
    
    ```
    font-size: 16px;
    ``` 
    
* **Background Color**:
    
    ```
    background-color: yellow;
    ``` 
    
* **Margin**:
    
    ```
    margin: 20px;
    ``` 
    
* **Padding**:
    
    ```
    padding: 10px;
    ``` 
    
* **Border**:
    
    ```
    border: 1px solid black;
    ``` 
    

#### 6\. Applying Basic Styles

Let's create a simple HTML document and apply some basic CSS styles to it:

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Introduction to CSS</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <h1>Welcome to CSS</h1>
    <p class="intro">This is an introduction to CSS.</p>
    <p id="main">CSS makes the web beautiful!</p>
</body>
</html>
``` 

**CSS (styles.css)**:

```
/* Element Selector */
h1 {
    color: navy;
    font-size: 36px;
}

/* Class Selector */
.intro {
    font-size: 20px;
    color: darkgreen;
}

/* ID Selector */
#main {
    background-color: lightgray;
    padding: 10px;
    border: 1px solid black;
}
``` 

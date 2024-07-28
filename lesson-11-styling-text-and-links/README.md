### Lesson 11: Styling Text and Links

#### Objectives:

* Learn how to style text in various ways using CSS
* Understand how to style links and their different states (hover, active, visited)
* Apply CSS properties to control text appearance
* Combine text and link styling to enhance webpage aesthetics

#### Lesson Outline:

1.  **Basic Text Styling**
2.  **Text Alignment and Transformation**
3.  **Text Decoration**
4.  **Styling Links**
5.  **Link Pseudo-Classes**
6.  **Combining Text and Link Styling**

* * *

#### 1\. Basic Text Styling

CSS offers various properties to style text, such as setting font size, color, and font family.

* **Font Size**:
    
    ```
    p {
        font-size: 16px;
    }
    ``` 
    
* **Font Family**:
    
    ```
    p {
        font-family: 'Arial', sans-serif;
    }
    ``` 
    
* **Font Weight**:
    
    ```
    p {
        font-weight: bold;
    }
    ``` 
    
* **Font Style**:
    
    ```
    p {
        font-style: italic;
    }
    ``` 
    
* **Text Color**:
    
    ```
    p {
        color: #333;
    }
    ``` 
    

#### 2\. Text Alignment and Transformation

Text alignment and transformation help control the layout and presentation of text.

* **Text Alignment**:
    
    ```
    h1 {
        text-align: center;
    }
    ``` 
    
* **Text Transformation**:
    
    ```
    p.uppercase {
        text-transform: uppercase;
    }
    
    p.lowercase {
        text-transform: lowercase;
    }
    
    p.capitalize {
        text-transform: capitalize;
    }
    ``` 
    

#### 3\. Text Decoration

Text decoration properties add or remove decorations from text, such as underlines, overlines, and line-throughs.

* **Text Decoration**:
    
    ```
    a {
        text-decoration: none;
    }
    
    .underline {
        text-decoration: underline;
    }
    
    .line-through {
        text-decoration: line-through;
    }
    ``` 
    
* **Text Shadow**:
    
    ```
    h2 {
        text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
    }
    ``` 
    

#### 4\. Styling Links

Links can be styled to improve their appearance and provide visual feedback during interaction.

* **Basic Link Styling**:
    
    ```
    a {
        color: #0066cc;
        text-decoration: none;
    }
    
    a:hover {
        text-decoration: underline;
    }
    ``` 
    

#### 5\. Link Pseudo-Classes

Pseudo-classes are used to define the special states of an element.

* **Pseudo-Classes for Links**:
    
    ```
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
    

#### 6\. Combining Text and Link Styling

Let's create an HTML document that demonstrates various text and link styling techniques:

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Styling Text and Links</title>
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

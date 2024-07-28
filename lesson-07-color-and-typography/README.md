### Lesson 7: Color and Typography

#### Objectives:

* Learn how to use CSS to set colors and backgrounds
* Understand the use of color values (names, HEX, RGB, RGBA, HSL)
* Learn how to control typography in CSS (fonts, sizes, weights, styles)
* Understand line height, letter spacing, and text alignment

#### Lesson Outline:

1.  **Setting Colors in CSS**
2.  **Typography Basics**
3.  **Font Properties**
4.  **Text Properties**

* * *

#### 1\. Setting Colors in CSS

CSS allows you to specify colors using various formats. You can apply colors to text, backgrounds, borders, and other elements.

* **Color Names**:
    
    ```
    p {
        color: red;
    }
    ``` 
    
* **HEX Values**:
    
    ```
    p {
        color: #ff0000;
    }
    ``` 
    
* **RGB Values**:
    
    ```
    p {
        color: rgb(255, 0, 0);
    }
    ``` 
    
* **RGBA Values** (includes opacity):
    
    ```
    p {
        color: rgba(255, 0, 0, 0.5);
    }
    ``` 
    
* **HSL Values**:
    
    ```
    p {
        color: hsl(0, 100%, 50%);
    }
    ``` 
    
* **Setting Background Colors**:
    
    ```
    body {
        background-color: lightblue;
    }
    ``` 
    

#### 2\. Typography Basics

Typography in web design refers to the styling of text to make it readable and visually appealing.

* **Font Family**:
    
    ```
    body {
        font-family: Arial, sans-serif;
    }
    ``` 
    
* **Font Size**:
    
    ```
    p {
        font-size: 16px;
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
    

#### 3\. Font Properties

* **Font Family**: Specifies the typeface to be used.
    
    ```
    body {
        font-family: 'Times New Roman', Times, serif;
    }
    ``` 
    
* **Font Size**: Controls the size of the text.
    
    ```
    h1 {
        font-size: 2em;
    }
    ``` 
    
* **Font Weight**: Sets the thickness of the font.
    
    ```
    strong {
        font-weight: 700;
    }
    ``` 
    
* **Font Style**: Sets the style of the font (normal, italic, oblique).
    
    ```
    em {
        font-style: italic;
    }
    ``` 
    
* **Font Variant**: Controls the use of small-caps.
    
    ```
    p {
        font-variant: small-caps;
    }
    ``` 
    

#### 4\. Text Properties

* **Text Color**: Sets the color of the text.
    
    ```
    p {
        color: #333;
    }
    ``` 
    
* **Text Alignment**: Aligns the text within its container (left, right, center, justify).
    
    ```
    h1 {
        text-align: center;
    }
    ``` 
    
* **Line Height**: Controls the space between lines of text.
    
    ```
    p {
        line-height: 1.5;
    }
    ``` 
    
* **Letter Spacing**: Controls the space between letters.
    
    ```
    h2 {
        letter-spacing: 2px;
    }
    ``` 
    
* **Text Decoration**: Adds decoration to text (underline, overline, line-through, none).
    
    ```
    a {
        text-decoration: none;
    }
    ``` 
    
* **Text Transform**: Controls the capitalization of text.
    
    ```
    p.uppercase {
        text-transform: uppercase;
    }
    ``` 
    

#### Creating a Simple Webpage with Color and Typography

Let's create an HTML document that demonstrates the use of color and typography:

**HTML (index.html)**:

```
<!DOCTYPE html>
<html>
<head>
    <title>Color and Typography</title>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <h1>Welcome to Color and Typography</h1>
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

### Lesson 2: Text Formatting and Semantics

#### Objectives:

* Learn about text formatting tags in HTML
* Understand the importance of semantic HTML
* Use semantic elements to improve the structure and accessibility of web content

#### Lesson Outline:

1.  **Basic Text Formatting**
2.  **Semantic HTML Elements**
3.  **Creating a Document with Semantic HTML**

* * *

#### 1\. Basic Text Formatting

HTML provides a variety of tags to format text. Here are some commonly used ones:

* **Bold Text**: `<b>` or `<strong>`
    ```
    <b>This text is bold</b>
    <strong>This text is strong</strong>
    ```
    
* **Italic Text**: `<i>` or `<em>`
    ```
    <i>This text is italic</i>
    <em>This text is emphasized</em>
    ```
    
* **Underlined Text**: `<u>`
    ```
    <u>This text is underlined</u>
    ```
    
* **Strikethrough Text**: `<s>`
    ```
    <s>This text is strikethrough</s>
    ```
    
* **Subscript and Superscript**: `<sub>` and `<sup>`
    ```
    H<sub>2</sub>O
    E = mc<sup>2</sup>
    ```
    
* **Quotations**: `<blockquote>` and `<q>`
    ```
    <blockquote>This is a blockquote.</blockquote>
    <q>This is an inline quotation.</q>
    ```
    
* **Preformatted Text**: `<pre>`
    ```
    <pre>
    This text
    preserves    whitespace
    and line breaks.
    </pre>
    ``` 
    

#### 2\. Semantic HTML Elements

Semantic HTML elements clearly describe their meaning in a way that both the browser and the developer can understand. Using semantic elements improves accessibility and SEO.

* **Headings**: `<h1>` to `<h6>`
    ```
    <h1>Main Heading</h1>
    <h2>Subheading</h2>
    ```
    
* **Article**: `<article>`
    ```
    <article>
        <h2>Article Title</h2>
        <p>Article content goes here.</p>
    </article>
    ```
    
* **Section**: `<section>`
    ```
    <section>
        <h2>Section Title</h2>
        <p>Section content goes here.</p>
    </section>
    ``` 
    
* **Nav**: `<nav>`
    ```
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
        </ul>
    </nav>
    ``` 
    
* **Aside**: `<aside>`
    ```
    <aside>
        <p>This is an aside.</p>
    </aside>
    ``` 
    
* **Footer**: `<footer>`
    ```
    <footer>
        <p>Footer content goes here.</p>
    </footer>
    ``` 
    
* **Header**: `<header>`
    ```
    <header>
        <h1>Website Header</h1>
    </header>
    ``` 
    

#### 3\. Creating a Document with Semantic HTML

Let's create an HTML document using semantic elements:
```
<!DOCTYPE html>
<html>
<head>
    <title>Semantic HTML Example</title>
</head>
<body>
    <header>
        <h1>My Website</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <article>
            <h2>Welcome to My Website</h2>
            <p>This is an example of a website using semantic HTML elements.</p>
        </article>

        <section>
            <h2>About</h2>
            <p>Information about the website goes here.</p>
        </section>

        <aside>
            <h3>Related Links</h3>
            <ul>
                <li><a href="#link1">Link 1</a></li>
                <li><a href="#link2">Link 2</a></li>
            </ul>
        </aside>
    </main>

    <footer>
        <p>&copy; 2024 My Website</p>
    </footer>
</body>
</html>
```

### Lesson 3: Links and Images

#### Objectives:

* Understand how to create hyperlinks in HTML
* Learn how to add and format images in HTML
* Differentiate between absolute and relative paths

#### Lesson Outline:

1.  **Creating Hyperlinks**
2.  **Adding and Formatting Images**
3.  **Absolute vs. Relative Paths**

* * *

#### 1\. Creating Hyperlinks

Hyperlinks, or links, are created using the `<a>` tag. Links can navigate to other pages, sections within the same page, or even different websites.

* **Basic Link**:
    ```
    <a href="https://www.example.com">Visit Example</a>
    ``` 
    
* **Opening Links in a New Tab**:
    ```
    <a href="https://www.example.com" target="_blank">Visit Example in a New Tab</a>
    ``` 
    
* **Linking to an Email Address**:
    ```
    <a href="mailto:someone@example.com">Send Email</a>
    ``` 
    
* **Linking to a Section within the Same Page**:
    ```
    <a href="#section1">Go to Section 1</a>
    
    <!-- Later in the document -->
    <h2 id="section1">Section 1</h2>
    <p>Content of Section 1</p>
    ```
    

#### 2\. Adding and Formatting Images

Images are added using the `<img>` tag, which is a self-closing tag.

* **Basic Image**:
    ```
    <img src="image.jpg" alt="Description of image">
    ``` 
    
    * `src`: Specifies the path to the image file.
    * `alt`: Provides alternative text for the image if it cannot be displayed.
* **Adjusting Image Size**:
    ```
    <img src="image.jpg" alt="Description of image" width="300" height="200">
    ``` 
    
* **Using External Images**:
    ```
    <img src="https://www.example.com/image.jpg" alt="Description of image">
    ``` 
    
* **Adding a Link to an Image**:
    ```
    <a href="https://www.example.com">
        <img src="image.jpg" alt="Description of image">
    </a>` 
    ```
    

#### 3\. Absolute vs. Relative Paths

* **Absolute Path**: A full URL that points to a specific location on the web.
    ```
    <a href="https://www.example.com/page.html">Visit Example</a>
    <img src="https://www.example.com/image.jpg" alt="Description of image">` 
    ```

* **Relative Path**: A path relative to the current document's location.
    ```
    <!-- Link to another page in the same directory -->
    <a href="page.html">Go to Page</a>
    
    <!-- Link to an image in the same directory -->
    <img src="image.jpg" alt="Description of image">
    
    <!-- Link to a page in a subdirectory -->
    <a href="subdirectory/page.html">Go to Page in Subdirectory</a>
    
    <!-- Link to an image in a subdirectory -->
    <img src="subdirectory/image.jpg" alt="Description of image">
    ```
    

#### Creating a Simple Webpage with Links and Images

Let's create a simple HTML document that includes both links and images:

```
`<!DOCTYPE html>
<html>
<head>
    <title>Links and Images</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a sample webpage demonstrating links and images.</p>

    <h2>Links</h2>
    <ul>
        <li><a href="https://www.example.com" target="_blank">External Link</a></li>
        <li><a href="#section1">Internal Link</a></li>
        <li><a href="mailto:someone@example.com">Email Link</a></li>
    </ul>

    <h2>Images</h2>
    <img src="image.jpg" alt="Sample Image" width="300">

    <h2 id="section1">Section 1</h2>
    <p>This is an example of an internal link target.</p>

    <h2>Image Link</h2>
    <a href="https://www.example.com">
        <img src="image.jpg" alt="Sample Image Link" width="300">
    </a>
</body>
</html>
```

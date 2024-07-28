### Lesson 4: Lists and Tables

#### Objectives:

* Learn how to create and format different types of lists in HTML
* Understand how to create and format tables in HTML
* Get familiar with the attributes and elements used in lists and tables

#### Lesson Outline:

1.  **Creating Lists**
2.  **Formatting Lists**
3.  **Creating Tables**
4.  **Formatting Tables**

* * *

#### 1\. Creating Lists

HTML supports several types of lists, including ordered lists, unordered lists, and definition lists.

* **Unordered Lists**:
    
    * Use the `<ul>` tag to create an unordered list.
    * Use the `<li>` tag for each list item.
    
    ```
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
    </ul>
    ``` 
    
* **Ordered Lists**:
    
    * Use the `<ol>` tag to create an ordered list.
    * Use the `<li>` tag for each list item.
    
    ```
    <ol>
        <li>First item</li>
        <li>Second item</li>
        <li>Third item</li>
    </ol>
    ``` 
    
* **Definition Lists**:
    
    * Use the `<dl>` tag to create a definition list.
    * Use the `<dt>` tag for each term.
    * Use the `<dd>` tag for each description.
    
    ```
    <dl>
        <dt>HTML</dt>
        <dd>HyperText Markup Language</dd>
        <dt>CSS</dt>
        <dd>Cascading Style Sheets</dd>
    </dl>
    ``` 
    

#### 2\. Formatting Lists

Lists can be styled using CSS to enhance their appearance and usability.

* **Customizing List Markers**:
    
    ```
    <ul style="list-style-type: square;">
        <li>Square item</li>
        <li>Square item</li>
    </ul>
    
    <ol style="list-style-type: upper-roman;">
        <li>Item I</li>
        <li>Item II</li>
    </ol>
    ``` 
    
* **Nested Lists**:
    
    ```
    <ul>
        <li>Item 1
            <ul>
                <li>Sub-item 1</li>
                <li>Sub-item 2</li>
            </ul>
        </li>
        <li>Item 2</li>
    </ul>
    ``` 
    

#### 3\. Creating Tables

Tables are created using the `<table>` tag, with rows defined by `<tr>`, headers by `<th>`, and cells by `<td>`.

* **Basic Table**:
    
    ```
    <table>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
        <tr>
            <td>Data 3</td>
            <td>Data 4</td>
        </tr>
    </table>
    ``` 
    
* **Table with Caption**:
    
    ```
    <table>
        <caption>Table Caption</caption>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
    </table>
    ``` 
    

#### 4\. Formatting Tables

Tables can be styled using CSS to improve readability and aesthetics.

* **Adding Borders and Padding**:
    
    ```
    <style>
        table, th, td {
            border: 1px solid black;
            border-collapse: collapse;
            padding: 10px;
        } 
    </style>
    ``` 
    
* **Adding a Background Color**:
    
    ```
    <style>
        th {
            background-color: #f2f2f2;
        }
        td {
            background-color: #f9f9f9;
        }
    </style>
    ``` 
    
* **Adjusting Table Width and Alignment**:
    
    ```
    <style>
        table {
            width: 100%;
        }
        th, td {
            text-align: left;
        }
    </style>
    ``` 
    

#### Creating a Simple Webpage with Lists and Tables

Let's create an HTML document that includes both lists and tables:

```
<!DOCTYPE html>
<html>
<head>
    <title>Lists and Tables</title>
    <style> table, th, td {
            border: 1px solid black;
            border-collapse: collapse;
            padding: 10px;
        }
        th {
            background-color: #f2f2f2;
        }
        td {
            background-color: #f9f9f9;
        }
        ul {
            list-style-type: square;
        }
        ol {
            list-style-type: upper-roman;
        } </style>
</head>
<body>
    <h1>Lists and Tables</h1>

    <h2>Unordered List</h2>
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
    </ul>

    <h2>Ordered List</h2>
    <ol>
        <li>First item</li>
        <li>Second item</li>
        <li>Third item</li>
    </ol>

    <h2>Definition List</h2>
    <dl>
        <dt>HTML</dt>
        <dd>HyperText Markup Language</dd>
        <dt>CSS</dt>
        <dd>Cascading Style Sheets</dd>
    </dl>

    <h2>Table</h2>
    <table>
        <caption>Sample Table</caption>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
        <tr>
            <td>Data 3</td>
            <td>Data 4</td>
        </tr>
    </table>
</body>
</html>
```

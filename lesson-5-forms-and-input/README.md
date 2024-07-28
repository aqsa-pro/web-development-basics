### Lesson 5: Forms and Input

#### Objectives:

* Understand the basic structure of HTML forms
* Learn about different input types and form elements
* Explore basic form validation

#### Lesson Outline:

1.  **Basic Structure of a Form**
2.  **Input Types and Form Elements**
3.  **Form Attributes and Methods**
4.  **Basic Form Validation**

* * *

#### 1\. Basic Structure of a Form

HTML forms are used to collect user input. The `<form>` element encapsulates form elements such as text fields, checkboxes, radio buttons, and submit buttons.

* **Basic Form**:
    
    ```
    <form action="submit_form.php" method="post">
        <!-- Form elements go here -->
    </form>
    ``` 
    
* **Action Attribute**: Specifies the URL to which the form data will be sent.
    
* **Method Attribute**: Specifies the HTTP method (`GET` or `POST`) to be used when sending form data.
    

#### 2\. Input Types and Form Elements

HTML provides various input types and form elements to collect different types of data from users.

* **Text Input**:
    
    ```
    <label for="name">Name:</label>
    <input type="text" id="name" name="name">
    ``` 
    
* **Password Input**:
    
    ```
    <label for="password">Password:</label>
    <input type="password" id="password" name="password">
    ``` 
    
* **Email Input**:
    
    ```
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">
    ``` 
    
* **Number Input**:
    
    ```
    <label for="age">Age:</label>
    <input type="number" id="age" name="age" min="0" max="100">
    ``` 
    
* **Date Input**:
    
    ```
    <label for="birthday">Birthday:</label>
    <input type="date" id="birthday" name="birthday">
    ``` 
    
* **Radio Buttons**:
    
    ```
    <p>Gender:</p>
    <input type="radio" id="male" name="gender" value="male">
    <label for="male">Male</label><br>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female">Female</label><br>
    ``` 
    
* **Checkboxes**:
    
    ```
    <p>Interests:</p>
    <input type="checkbox" id="coding" name="interests" value="coding">
    <label for="coding">Coding</label><br>
    <input type="checkbox" id="sports" name="interests" value="sports">
    <label for="sports">Sports</label><br>
    ``` 
    
* **Select Dropdown**:
    
    ```
    <label for="country">Country:</label>
    <select id="country" name="country">
        <option value="usa">USA</option>
        <option value="canada">Canada</option>
        <option value="uk">UK</option>
    </select>
    ``` 
    
* **Textarea**:
    
    ```
    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4" cols="50"></textarea>
    ``` 
    
* **Submit Button**:
    
    ```
    <input type="submit" value="Submit">
    ``` 
    

#### 3\. Form Attributes and Methods

Forms can be customized and controlled using various attributes and methods.

* **Form Attributes**:
    
    * `action`: Specifies the URL to send the form data.
    * `method`: Specifies the HTTP method (`GET` or `POST`).
    * `target`: Specifies where to display the response (e.g., `_blank`, `_self`).
* **Example Form with Attributes**:
    
    ```
    <form action="submit_form.php" method="post" target="_blank">
        <!-- Form elements go here -->
    </form>
    ``` 
    
* **GET vs. POST Methods**:
    
    * `GET`: Appends form data to the URL, suitable for non-sensitive data.
    * `POST`: Sends form data in the HTTP request body, suitable for sensitive data.

#### 4\. Basic Form Validation

HTML5 provides built-in form validation features to ensure data integrity.

* **Required Field**:
    
    ```
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" required>
    ``` 
    
* **Pattern Validation**:
    
    ```
    <label for="phone">Phone:</label>
    <input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" placeholder="123-456-7890">
    ``` 
    
* **Email Validation**:
    
    ```
    <label for="useremail">Email:</label>
    <input type="email" id="useremail" name="useremail" required>
    ``` 
    

#### Creating a Simple Webpage with Forms and Input

Let's create an HTML document that includes a basic form with various input types:

```
<!DOCTYPE html>
<html>
<head>
    <title>Forms and Input</title>
</head>
<body>
    <h1>Contact Us</h1>
    <form action="submit_form.php" method="post">
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name" required><br><br>
        
        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email" required><br><br>
        
        <label for="age">Age:</label><br>
        <input type="number" id="age" name="age" min="0" max="100"><br><br>
        
        <p>Gender:</p>
        <input type="radio" id="male" name="gender" value="male">
        <label for="male">Male</label><br>
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label><br><br>
        
        <p>Interests:</p>
        <input type="checkbox" id="coding" name="interests" value="coding">
        <label for="coding">Coding</label><br>
        <input type="checkbox" id="sports" name="interests" value="sports">
        <label for="sports">Sports</label><br><br>
        
        <label for="country">Country:</label><br>
        <select id="country" name="country">
            <option value="usa">USA</option>
            <option value="canada">Canada</option>
            <option value="uk">UK</option>
        </select><br><br>
        
        <label for="message">Message:</label><br>
        <textarea id="message" name="message" rows="4" cols="50"></textarea><br><br>
        
        <input type="submit" value="Submit">
    </form>
</body>
</html>
``` 

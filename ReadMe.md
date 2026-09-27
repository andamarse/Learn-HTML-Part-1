# Let's Get Started with Learning HTML

## What is HTML?

HTML stands for **HyperText Markup Language**.

You might have already heard about websites, which we normally navigate through using web browsers. Websites are built using different technologies, including HTML.

HTML is a **markup language** used to structure the content of web pages. It can work together with other technologies such as **CSS** and **JavaScript**, which we will learn about later.

CSS is used mainly to **style and design** web pages, while JavaScript is used to add **functionality and behavior** to web pages.

Together, HTML, CSS, and JavaScript form the foundation of most websites.

## ~~HTML Files~~

When you are coding in HTML, you would normally do it in a file with the `.html` extension. For example, `index.html`:

When you open that file with a web browser, the browser interprets the HTML and displays the content according to the HTML elements and their structure.

## ~~Basic HTML Template~~

An HTML document would normally start with a basic template ~~such as~~:

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>

    </body>
</html>
```

In VS Code, you can generate this template inside an HTML file by typing an exclamation mark (`!`) and pressing **Enter**.

## ~~Understanding the Template~~

Let's explain the template.

```html
<!DOCTYPE html>
```

`DOCTYPE html` tells the browser that the document is an HTML document and instructs it to use **HTML5 standards mode**.

~~Next we have:~~

```html
<html>

</html>
```

The second line is an opening ~~`<html>`~~ HTML tag, and the last line is a closing ~~`</html>`~~ HTML tag.

The ~~`<html>`~~ HTML element is the **root element** of the HTML document. Other HTML elements are placed inside it.

### ~~HTML Tags~~

An HTML tag will normally start with a **less-than sign** ~~(`<`)~~, followed by the tag name, and then a **greater-than sign** ~~(`>`)~~.

~~For example:~~

```html
<tagName>
```

This is called an **opening tag**.

A closing tag contains a forward slash ~~(`/`)~~ before the tag name:

```html
</tagName>
```

An HTML element normally consists of an opening tag, content, and a closing tag:

```html
<openingTag>
    Content
</closingTag>
```

For example:

```html
<p>Hello World</p>
```

Here:

~~`<p>`~~ `p` is the opening tag.

`Hello World` is the content.

~~`</p>`~~ forward slash `p` is the closing tag.

Together, they form the ~~`<p>`~~ paragraph element.

### ~~Elements Without Closing Tags~~

Some HTML elements do not have a closing tag. These are called **void elements**.

For example:

```html
<input>
```

The ~~`<input>`~~ input element is a void element, so it does not need a closing tag:

```html
</input>
```

Other examples include the image element ~~`<img>`~~, line break element ~~`<br>`~~, and metadata element ~~`<meta>`~~.

## ~~The `<html>`, `<head>`, and `<body>` Elements~~

The HTML document starts with the ~~`<html>`~~ `html` element, which is the root element.

Inside the ~~`<html>`~~ `html` element, we normally have two main elements:

```html
<html>
    <head>

    </head>
    <body>

    </body>
</html>
```

```html
<head>

</head>
```

The ~~`<head>`~~ head element contains information **about the document**, such as metadata, the page title, links to stylesheets, and other resources or information used by the browser.

```html
<body>

</body>
```

The ~~`<body>`~~ body element contains the **main content of the web page** that is displayed to the user.

For example, in this tutorial we will create two headings,

```html
<h1>MyCompany</h1>
<h2>Login</h2>
```

two labels,

```html
<label>Username</label>
<label>Password</label>
```

two input fields,

```html
<input>
<input>
```

and a button

```html
<button>Login</button>
```

inside a ~~`<form>`~~ form element

```html
<form>
    <h1>MyCompany</h1>
    <h2>Login</h2>
    <label>Username</label>
    <input>
    <label>Password</label>
    <input>
    <button>Login</button>
</form>
```

and inside the ~~`<body>`~~ body element.

```html
<body>
    <form>
        <h1>MyCompany</h1>
        <h2>Login</h2>
        <label>Username</label>
        <input>
        <label>Password</label>
        <input>
        <button>Login</button>
    </form>
</body>
```

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Login</title>
    </head>
    <body>
        <form>
            <h1>MyCompany</h1>
            <h2>Login</h2>
            <label>Username</label>
            <input>
            <label>Password</label>
            <input>
            <button>Login</button>
        </form>
    </body>
</html>
```

## ~~HTML Attributes~~

HTML elements can also contain **attributes**.

Attributes provide additional information about an element or control aspects of how the element behaves.

~~For example:~~

```html
<input class="input-outline" name="username" id="username">
```

In this example:

* `class` is an attribute.
* `name` is an attribute.
* `id` is an attribute.
* `input-outline`, `username`, and `username` are their respective attribute values.

Some common attributes include:

* id
* class
* name
* placeholder
* type
* href
* src

### ~~`id`~~

An `id` gives an element a unique identifier within the HTML document.

~~For example:~~

```html
<input id="username">
```

An element should have only one `id` attribute, and the same `id` should not normally be used on multiple elements in the same document.

### ~~`class`~~

The `class` attribute is commonly used to group elements that should share styling or behavior.

For example:

```html
<h1 class="heading">MyCompany</h1>
<h2 class="heading">Login</h2>
```

Both heading elements have the `heading` class.

An element can have multiple classes:

```html
<input class="input-outline password-field">
```

Here, the input element has two classes: `input-outline` and `password-field`.

### ~~`name`~~

The `name` attribute is particularly important when working with forms.

~~For example:~~

```html
<input name="username">
```

Unlike `id`, the `name` value does not have to be unique across the entire document. Multiple form controls can have the same `name`, depending on how they are being used.

### ~~`placeholder`~~

The `placeholder` attribute is commonly used with input fields to display example or guidance text inside an empty input.

~~For example:~~

```html
<input placeholder="Enter your username">
```

The placeholder is **not the actual value** entered into the input. It disappears when the user enters a value.

## ~~HTML Forms~~

A **form** is used to collect information or input from a user.

HTML provides a ~~`<form>`~~ form element that can contain different **form controls**, such as input fields, checkboxes, radio buttons, and buttons.

For example:

```html
<form>
    <label>Username</label>
    <input>
    <label>Password</label>
    <input>
    <button>Login</button>
</form>
```

Here, the ~~`<form>`~~ form element contains the elements that make up our login form.

The ~~`<label>`~~ label elements describe what information the user should enter, the ~~`<input>`~~ input elements allow the user to enter information, and the ~~`<button>`~~ button element allows the user to perform an action.

### ~~Form `action` and `method`~~

A ~~`<form>`~~ form element can also have attributes that control what happens when the form is submitted.

For example:

```html
<form action="/login" method="post">
    <label>Username</label>
    <input name="username">
    <label>Password</label>
    <input name="password" type="password">
    <button type="submit">Login</button>
</form>
```

The `action` attribute specifies **where the form data should be sent** when the form is submitted.

The `method` attribute specifies **how the data should be sent**.

Common methods include:

* `GET` — commonly used when retrieving data or when the submitted information can be included in the URL.
* `POST` — commonly used when sending data to a server, such as when submitting a login form.

The `name` attribute on form controls is important because it identifies the fields when their values are submitted.

For example:

```html
<input name="username">
<input name="password">
```

If the user enters: `username: John` and `password: 123456`, the form submission can contain data associated with the names: `username = John` and `password = 123456`.

We will learn more about forms, form controls, and submitting data to a server later.

## ~~Putting Everything Together~~

~~Here is our login example using some of the attributes we have learned:~~

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Login</title>
    </head>
    <body>
        <form class="login-form" action="/login" method="post">
            <h1 class="heading">MyCompany</h1>
            <h2 class="heading">Login</h2>
            <label>Username</label>
            <input class="input-outline" name="username" id="username" placeholder="Enter your username">
            <label>Password</label>
            <input class="input-outline password-field" name="password" id="password" type="password" placeholder="Enter your password">
            <button type="submit">Login</button>
        </form>
    </body>
</html>
```

Now we will create a project folder, open it with VS Code, and start typing this code in a file named `login.html` and then open the file with a web browser to see how the HTML is rendered.

**Take special note:** You can use the browser's **Developer Tools/Inspector** to inspect the HTML elements generated on the page by right-clicking on the web page and selecting **Inspect**.

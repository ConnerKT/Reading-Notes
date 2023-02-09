# **Dynamic Web pages with JavaScript**

## References

<https://developer.mozilla.org/en-US/docs/Web/JavaScript>

<https://code-maven.com/introduction-to-javascript>

<https://code-maven.com/javascript-input-with-prompt-and-confirm>

## Why Does This Topic Matter to **Me!**

This topic matters to me because I want to learn how to add functions to my classes and be able to make things function in a technical way.

# JavaScript

**Java Script** is a lightweight language, web page scripting language.

JavaScript can be simplified to three things, the language, DOM API, and the server API.

It can be embeded inline a HTML file or you can create a seperate file.

Input Output...

## Input

**alert** is one way to speak to the user using a pop up browser window.
(Remember these examples are inlined, not external)

    <script language="javascript">

        alert("Hello World");

    </script>

**document.write** is used to change what is shown, can be inputed in.

    First line
    <script>

    document.write("<h1>Hello World</h1>");

    </script>
    Last line

**console.log** is used to print out debugging info.

    <script>

    console.log("Hello World");

    </script>

## Output

**prompt** is used to pop up a window from the user to get the input. In this example it has a variable set to store the input, and a document write to write the variable.

    <script>

    var name = prompt("Your name:", "");
    document.write("Hello ", name);

    </script>

**confirm** is not an input, but recieves a true or false from the user.

    <script>

    if (confirm("Shall I print Hello World?")) {
    document.write("Hello World");
    } else {
    document.write("OK, I won't print it.");
    }

    </script>

## Variables 

A variable is a container for storing data.

**Var, let, const**

Var (variable) - is the oldest form of storing, to run on older browsers var is needed.

let - is like var but newer (variable that can be changed)

const - stores data but that value can't be changed

**Variables are given a unique name**

= means assignment

== is the sign for equal to

## Things I Want to know more about

How to apply JavaScript to my site.
How do I make buttons work with animation?

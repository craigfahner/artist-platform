# Building Blocks of Web Apps

### HTML

* Stands for Hypertext Markup Language
* *Hypertext* refers to text with embedded links that let you "jump" to another file or location
* Markup: a language used to describe formatting and layout
* **[HTML reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)**

### CSS

* Cascading Style Sheets aka The Style
* HTML is your content - CSS is the appearance
* Determines font sizes, positions of elements on the page, etc.
* **[CSS reference](https://cssreference.io/)**

### Javascript

* Handles interactions, events, etc.
* Javascript is built into all modern browsers and lets you do things like animate elements, process user interactions and create dynamic experiences in the browser
* Syntax: semicolons, curly brackets, parentheses, indentations, dots!
* Rather than being a *markup language*, like HTML or CSS, it’s a *programming language* used to create algorithms
* **[Javascript reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)**
* Two kinds of JS scripting: client-side and server-side

### Basic Javascript Concepts
#### Comments
Comments are used to make notes in your code that are ignored by the JavaScript compiler. Any text that follows a double forward slash (//) is considered a comment.

```js
// this is a comment
```

#### Values and variables
Variables are used to store data in JavaScript. They are *declared* using the **var** keyword. A special name is given for a variable, which can be referred to in your program to recall and manipulate the stored data.

Variables can be numbers, "strings" (text), objects (sets of data), booleans (true or false) and other types of information.

```js
var length = 16; // the variable "length" is storing the number 16
var lastName = "Fahner" // the variable "lastName" is storing the String "Fahner"
// note that strings are placed within quotation marks
```

#### Control structures
JavaScript programs are given behaviours using control structures, which test and manipulate variables.

A **conditional** structure tests to see if a condition is met by comparing a variable to another value. These are written in an "if... else" format. Instructions that are written within the "if" block only run if the condition is met. Instructions in the "else" block only run when the condition is not met.

```js
if(theSky=="blue"){
  //go outside
} else {
  //go inside
}
```

A **loop** is a control structure that repeats instructions for a certain amount of times, or until a certain condition is met. In a **for loop**, a variable is declared which is incremented until it reaches a stated condition:

```js
// increment variable i, which starts at 0, until it reaches list.length
for(var i = 0; i < list.length; i++){ 
  console.log(list[i]); // print to the javascript console each element in the array "list"
}
```

#### Functions and methods

JavaScript has a number of built-in functions and methods, which automate certain operations (math functions, formatting, etc). The ```toUpperCase()``` method, for instance, converts text to uppercase:

```js
var text = "hello";
var x = text.toUpperCase();
```

The above code results in the following value for x:

```HELLO```

Functions and methods are followed by a set of parentheses, which sometimes are used to pass a variable to the function as a **parameter**. 

You can declare your own function by using the keyword **function**, which allows you to bundle a set of instructions under a given function name:

```js
function add(param1, param2){
  return param1 + param2;
}

var four = add(2,2);
```

In the above function, the **return** keyword is used to "send back" a value from the function.

#### Client-side vs Server-side scripting

All modern web browsers can interpret JavaScript programs. Websites often have scripts embedded in them, which are executed on the "client" side. It is also possible, through frameworks like **[node.js](https://www.nodejs.org)**, to run JavaScript on the server side. This means that the webserver runs a script that decides what content is served to the client when they access a service. Further server-side functionality is added through the use of libraries and packages such as Express and socket.io. These add-ons allow synchronous communication to be established between client and server, so that the scripts on either end can "talk to each other."

#### Further Reading

[Mozilla's "A re-introduction to JavaScript"](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript)

[Lee Tusman's guide to HTML/CSS/JS and the DOM](http://leetusman.com/intermediate-programming/posts/html-css-js-dom/)
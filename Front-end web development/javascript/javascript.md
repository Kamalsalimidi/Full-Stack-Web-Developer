# JavaScript

## Introduction

JavaScript Can Change HTML Content
One of many JavaScript HTML methods is getElementById().

The example below "finds" an HTML element (with id="demo"), and changes the element content (innerHTML) to "Hello JavaScript":

```
<!DOCTYPE html>
<html>
<body>

<h2>What Can JavaScript Do?</h2>

<p id="demo">JavaScript can change HTML content.</p>
<img id="myImage" src="pic_bulboff.gif" style="width:100px">

<button type="button" onclick='document.getElementById("demo").innerHTML = "Hello JavaScript!"'>Click Me!</button>
<button onclick="document.getElementById('myImage').src='pic_bulbon.gif'">Turn on the light</button>
</body>
</html>
```

## JavaScript Where To

In HTML, JavaScript code is inserted between <script> and </script> tags.
JavaScript in <head> or <body> or call from external file [ <script src="myScript.js"></script>]

## JavaScript Display Possibilities

JavaScript can "display" data in different ways:

Writing into an HTML element, using innerHTML.
Writing into the HTML output using document.write().
Writing into an alert box, using window.alert().
Writing into the browser console, using console.log().

## JavaScript Keywords

| Keyword	| Description |
|---------| -----------  |
| var	| Declares a variable |
| let	| Declares a block variable |
| const	| Declares a block constant |
| if	| Marks a block of statements to be executed on a condition |
| switch |	Marks a block of statements to be executed in different cases |
| for	| Marks a block of statements to be executed in a loop |
| function |	Declares a function |
| return |	Exits a function |
| try	| Implements error handling to a block of statements |

Note:
A variable declared without a value will have the value undefined.
You cannot re-declare a variable declared with let or const.
If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated. [ "5" + 2 + 3 = 523, 2 + 3 + "5" = 55 ]
[ var carName = "Volvo"; var carName; The variable carName will still have the value "Volvo" after the execution of these statements: ]

## JavaScript Arithmetic

| Operator |	Description |
| --------- | -------------- |
| +	| Addition |
| -	| Subtraction |
| *	| Multiplication |
| ** |	Exponentiation (ES2016) |
| /	| Division |
| %	| Modulus (Remainder) |
| ++ |	Increment |
| -- |	Decrement |

## JavaScript Functions

```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Functions</h2>

<p>This example calls a function which performs a calculation, and returns the result:</p>

<p id="demo"></p>

<script>
function myFunction(p1, p2) {
  return p1 * p2;
}
document.getElementById("demo").innerHTML = myFunction(4, 3);
</script>

</body>
</html>
```

## JavaScript Objects

```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Objects</h2>

<p>There are two different ways to access an object property.</p>

<p>You can use person.property or person["property"].</p>

<p id="demo"></p>

<script>
// Create an object:
const person = {
  firstName: "John",
  lastName : "Doe",
  id     :  5566
};

// Display some data from the object:
document.getElementById("demo").innerHTML =
person["firstName"] + " " + person["lastName"];
</script>

</body>
</html>
```
## HTML Events

An HTML event can be something the browser does, or something a user does.

Here are some examples of HTML events:

- An HTML web page has finished loading
- An HTML input field was changed
- An HTML button was clicked

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

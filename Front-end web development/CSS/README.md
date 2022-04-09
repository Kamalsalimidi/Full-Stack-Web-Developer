CSS 
---

**CSS selectors**

CSS selectors are used to "find" (or select) the HTML elements you want to style.

We can divide CSS selectors into five categories:

* Simple selectors (select elements based on name, id, class)

```
<html>
<head>
<style>
p,h1 {
  text-align: center;
  color: red;
}
</style>
</head>
<body>
<pHello World!</p>
</body>
</html>
```

```
<html>
<head>
<style>
#para1 {
  text-align: center;
  color: red;
}
</style>
</head>
<body>
<p id="para1">Hello World!</p>
</body>
</html>
```

```
<html>
<head>
<style>
h1.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>
<h1 class="center">Red and center-aligned heading</h1>
</body>
</html>
```

**CSS Universal Selector**

```
* {
  text-align: center;
  color: blue;
}
```

- Combinator selectors (select elements based on a specific relationship between them)
- Pseudo-class selectors (select elements based on a certain state)
- Pseudo-elements selectors (select and style a part of an element)
- Attribute selectors (select elements based on an attribute or attribute value)


**Add CSS**

- Three Ways to Insert CSS

  - External CSS - external file is used for css

  ```
  <!DOCTYPE html>
  <html>
  <head>
  <link rel="stylesheet" href="mystyle.css">
  </head>
  <body>
  ```

  - Internal CSS - It is defined inside the <style> element, inside the head section.
  - Inline CSS - An inline style may be used to apply a unique style for a single element.

  ```
  <h1 style="color:blue;text-align:center;">This is a heading</h1>
  <p style="color:red;">This is a paragraph.</p>
  ```

- Cascading Order - What style will be used when there is more than one style specified for an HTML element, number one has the highest priority.

- Inline style (inside an HTML element)
- External and internal style sheets (in the head section)
- Browser default

**CSS Comments**

```
/* This is
a multi-line
comment */
```

**CSS Styles** - 


- Colour 

  `colour, RGB, HEX, HSL`

- Background  

  `background-color: Blue; background-image: url("paper.gif"); background-repeat: repeat/no-repeat; background-attachment: fixed/scroll; background-     position: right top`

  i.e can be used in single line, follows same order as in above sequence 

      `background: #ffffff url("img_tree.png") no-repeat right top`

- text

  `color: blue; text-align: center/justify/others; text-align-last: right; vertical-align: text-bottom; text-decoration-line: ~overline~; text-decoration-color: blue; text-transform: uppercase; text-indent: 50px; letter-spacing: 5px; line-height: 0.8; word-spacing: 10px; white-space: nowrap; text-shadow: 2px 2px;`

- Borders 

  `border-width: 5px; border-style: solid; border-color: red`

   i.e can be used in single line, follows same order as in above sequence 

         border: 5px solid red

         border-top-style,border-right-style,border-bottom-style,border-left-style i.e `border-style: dotted solid double dashed`

  `border-radius: 5px` - property is used to add rounded borders to an element

- Margins - Outside of any defined borders.

  `margin-top: 100px; margin-right: 100px; margin-bottom: 100px; margin-left: 100px`

  i.e can be used in single line, follows same order as in above sequence 

        margin: 25px 50px 75px 100px

- Padding - Inside of any defined borders
  
  `padding-top: 100px; padding-right: 100px; padding-bottom: 100px; padding-left: 100px`

  i.e can be used in single line, follows same order as in above sequence 

        padding: 25px 50px 75px 100px

- Height/Width

  `height: 200px; width: 50%; max-width: 500px`

- Outline - OUTSIDE the borders

  `outline-width: solid; outline-style: red; outline-color: 20px`

   i.e can be used in single line, follows same order as in above sequence 

        outline: 25px 50px 75px

   `outline-offset: 70px` - property adds space between an outline and the edge/border of an element.

- Fonts

  `font-style: italic/normal/oblique; font-variant: small-caps; font-weight: bold; font-size: 30px; font-family: "Lucida Console", "Courier New", monospace`

  i.e can be used in single line, follows same order as in above sequence 

        font: italic small-caps bold 12px/30px Georgia, serif

  ```
  <head>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide">
  <style>
  body {
    font-family: "Audiowide", sans-serif;
  }
  </style>
  </head>
  ```

- Icons

  ```
  <!DOCTYPE html>
  <html>
  <head>
  <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
  </head>
  <body>
  
  <i class="material-icons">cloud</i>
  <i class="material-icons">favorite</i>
  <i class="material-icons">attachment</i>
  <i class="material-icons">computer</i>
  <i class="material-icons">traffic</i>
  
  </body>
  </html>
  ```

- Link

  ```
  <!DOCTYPE html>
  <html>
  <head>
  <style>
  /* unvisited link */
  a:link {
    color: red;
  }
  
  /* visited link */
  a:visited {
    color: green;
  }
  
  /* mouse over link */
  a:hover {
    color: hotpink;
  }
  
  /* selected link */
  a:active {
    color: blue;
  }
  </style>
  </head>
  <body>
  
  <h2>Styling a link depending on state</h2>
  
  <p><b><a href="default.asp" target="_blank">This is a link</a></b></p>
  <p><b>Note:</b> a:hover MUST come after a:link and a:visited in the CSS definition in order to be effective.</p>
  <p><b>Note:</b> a:active MUST come after a:hover in the CSS definition in order to be effective.</p>
  
  </body>
  </html>
  ```

- list
  
  `list-style-type: square; list-style-position: inside; list-style-image`

- table
  
  `border: 1px solid; border: 1px solid; width: 100%; text-align: left; padding: 15px; tr:hover {background-color: coral;}`
  
  ```
  <!DOCTYPE html>
  <html>
  <head>
  <style>
  table, th, td {
    border: 1px solid;
  }
  </style>
  </head>
  <body>
  
  <h2>Add a border to a table:</h2>
  
  <table>
    <tr>
      <th>Firstname</th>
      <th>Lastname</th>
    </tr>
    <tr>
      <td>Peter</td>
      <td>Griffin</td>
    </tr>
    <tr>
      <td>Lois</td>
      <td>Griffin</td>
    </tr>
  </table>
  
  </body>
  </html>
  ```
  
   - Responsive 

      ```
      <div style="overflow-x:auto;">

      <table>
      ... table content ...
      </table>
      
      </div>
      ```

- Display

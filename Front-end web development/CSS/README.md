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

  `color: blue; text-align: center/justify/others; text-align-last: right; vertical-align: text-bottom; text-decoration-line: ~overline~;`

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

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

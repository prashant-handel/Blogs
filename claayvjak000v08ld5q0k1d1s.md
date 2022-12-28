# Basics of CSS

The CSS stands for Cascading Style Sheets. The main motive of CSS is to style the sheet according to the requirement and for good appearance. The syntax of CSS includes a selector, then curly braces within which we define the properties and its values according to our requirements. 

eg-
 
```
p {
  color: red;
  text-align: center;
}
```

In the above code the selector is p which defines all p tags. color and text-align are properties. red and center are the values assign to the properties. The above command will give text color as red and align the text as center which comes within the p tag.

There are three ways to define CSS -
1.  External CSS
2.  Internal CSS
3.  Inline CSS

**1. External CSS**

It is defined by adding link of an external file having "file_name".css for eg. style.css. We add a link tag within the head tag of the HTML in which we add our style.css file. We do all the changes in the style.css file and all the changes are done in the output. We can use different types of selectors and assign different css styles to it. 

We can assign the link of the CSS file as shown

```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

**2. Internal CSS**

The internal CSS consists of all the styling codes within the HTML file itself. We have to define the style tag within the head tag of HTML file. All the designing is defined within this style tag as shown 

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: cyan;
}

h1 {
  color: red;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

**3. Inline CSS**

The inline CSS consists of all the designing properties and its values within the class attribute of the tag we want to modify. 

```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue; text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```






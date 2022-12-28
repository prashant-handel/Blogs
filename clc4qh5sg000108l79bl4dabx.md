# Console.log() vs console.dir()

Both methods **console.log()** and **console.dir()** are used to display contents in the console of the browser.

## Console.log()

The console.log() method prints out the object in the console in the form of string to the user. It returns the object in its string representation.

### Syntax

`console.log(value);`

`console.log("string", value, expression);`

### Example

```javascript
console.log(123456); // 123456

console.log("Hello Friends");    // Hello Friends

console.log(10 + 20); // 30
```

## Console.dir()

The console.dir() method output the list of object properties of a specified object in the console to the user. It recognizes the object just as an object and outputs its properties. console.dir shows all properties of a DOM element along with its methods which we can apply on them.

### Syntax

`console.dir(element)`

### Example

HTML

```xml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello All after 3 seconds</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <div id="HelloAll">Hello All
            <span>I am Prashant</span>
        </div>
    </div>
    <script src="app.js"></script>
</body>
</html>
```

JavaScript

```javascript
let HelloAllEl = document.getElementById("HelloAll");
console.dir(HelloAllEl);
```

Output

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672054608355/b3cf95db-0ed4-452c-a696-373e8e29f57b.jpeg align="center")

The above image shows the values displayed in the console using **console.dir()** method shows all the properties and possible methods of the element.

## Conclusion

The main difference between these two methods is that the **console.log()** method displays the element in the form of string.

Whereas, the **console.dir()** method displays an interactive list of the properties of the specified JavaScript object.
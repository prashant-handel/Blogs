# Window setInterval() in JavaScript

The **setInterval()** method in JavaScript is used to call a specific function repeatedly at every given interval of time. It evaluates an expression or calls a function at given intervals. This method continues the calling of function until the window is closed or the **clearInterval()** method is invoked. This method returns a numeric value or a non-zero number that identifies the created timer.

We can write this method with ***window*** prefix or without window prefix.

## Syntax

window.setInterval(function, time interval);

or

setInterval(function, time interval);

## Parameters

This function takes two parameters. The first parameter is the function that we want to execute and the second parameter is the time interval in milliseconds. Thus, according to both parameters the function in the first parameter calls itself at every interval of time which is passed as second parameter.

## Example

### HTML

```javascript
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello All Blinking Effect</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <div id="HelloAll">Hello All</div>
    </div>
    <script src="app.js"></script>
</body>
</html>
```

### CSS

```javascript
body{
    margin: 0;
    display:flex;
    justify-content: center;
    height: 100vh;
    align-items: center;
    background-color:slategray;
}

#HelloAll{
    font-size: 200px;
    display: block;
}
```

### JavaScript

```javascript
let HelloAllEl = document.getElementById("HelloAll");

setInterval(() => {
  HelloAllEl.style.display = 'block';
}, 1000);

setInterval(() => {
  HelloAllEl.style.display = 'none';
}, 2000);
```

In the above example the Hello all text shows and hides at a set interval of time.

## ClearInterval()

To stop the execution of the **setInterval()** function we have to use **clearInterval()** function. The value returned by the **setInterval()** method has to be passed as the argument of **clearInterval()** method to cancel the timeout.
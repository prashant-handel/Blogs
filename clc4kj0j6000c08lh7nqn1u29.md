# Window setTimeout() in JavaScript

The **setTimeout()** function is similar to the **setInterval()** method in JavaScript. The only difference is that this method does not execute repeatedly. This method calls the function after a specific period only once.

We can write this method with *a* **window** prefix or without a window prefix.

## Syntax

window.setTimeout(function, time period);

or

setTimeout(function, time period);

## Parameters

This function takes two parameters. The first parameter is the function that we want to execute and the second parameter is the time interval in milliseconds. Thus, according to both parameters, the function in the first parameter calls itself after a specific time period which is mentioned as second parameter.

## Example

### HTML

```javascript
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
    display: none;
}
```

### JavaScript

```javascript
let HelloAllEl = document.getElementById("HelloAll");

setTimeout(() => {
  HelloAllEl.style.display = 'block';
}, 3000);
```

In the above example the Hello all text shows after 3 seconds i.e. 3000 milliseconds.

Result after 3seconds.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672045101773/b6f033ad-c947-496c-ab07-6d1a6fa648ca.jpeg align="center")

## ClearTimeout()

To stop the execution of the **setTimeout()** function we have to use **clearTimeout()** function. The value returned by the **setTimeout()** method has to be passed as the argument of **clearTimeout()** method to cancel the timeout.
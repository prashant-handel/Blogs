# Difference Between InnerHTML and outerHTML

## What is innerHTML?

The innerHTML is a DOM element method that is used to get the whole content which is inside the element on which this method is applied. It doesn't return the element on which this method is called but only gives out whole text content within it in the form of a string.

Let's take an example-

```xml
<p id="para">Hi! <b> I am Prashant</b></p>
```

We can call innerHTML method on the p tag by using its id in this way.

```javascript
para.innerHTML    // Hi! <b> I am Prashant</b>
```

We not only get the innerHTML but also modify it by assigning the value to it, for example

```javascript
para.innerHTML = `Hi! I am Rohan`;
```

In the above assignment I have changed the name from Prashant to Rohan and also removed the bold tag.

## What is outerHTML?

The outerHTML is much similar to the innerHTML method. It also return value in the form of the string. It returns the values including the element on which this method is called.

Let's take the above example for better understanding.

```xml
<p id="para">Hi! <b> I am Prashant</b></p>
```

Calling outerHTML method on the p tag

```javascript
para.outerHTML    // <p id="para">Hi! <b> I am Prashant</b></p>
```

Similar to the innerHTML method we can also assign values to the elements using outerHTML.

```javascript
para.outerHTML = `<p id="para">Hi! I am Rohan</p>`;
```

Similar to the above innerHTML example I have changed the name from Prashant to Rohan and also removed the bold tag.

## Conclusion

The innerHTML and outerHTML methods are much similar to each other. The innerHTML method excludes the element on which the method is called. But the outerHTML method includes the element on which it is called.

These methods doesn't valid for text or comment nodes. These methods only work on the element nodes.
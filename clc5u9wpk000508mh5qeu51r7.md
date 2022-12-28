# innerText vs innerHTML

## What is innerText?

The innerText method is used to get the text within the text excluding the tag itself. It avoids the tags within it and only return the text values in the form of the string.

For example

```javascript
<div id="HelloAll">Hello All
            <span><b>I am Prashant</b></span>
        </div>
```

Calling innerText method on the div having id HelloAll

```javascript
HelloAll.innerText
```

Output is

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672121422956/aaf46ace-bb2d-47b4-b470-aca33002e3e4.jpeg align="center")

innerText method can also modify text within the elements.

```javascript
HelloAll.innerText = "Hello All I am Prashant";
```

Output

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672121608381/b5fa2b42-44d2-4a86-822f-617518141157.jpeg align="center")

## **What is innerHTML?**

The innerHTML is a DOM element method that is used to get the whole content which is inside the element on which this method is applied. It doesn't return the element on which this method is called but only gives out whole text content within it in the form of a string.

Let's take an example-

```javascript
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

In the above assignment, I changed the name from Prashant to Rohan and also removed the bold tag.

## Conclusion

The innerText and innerHTML methods are much similar to each other. The innerHTML includes the text as well as tags within the element. But the innerText method includes the tags and ignores the tags within it.
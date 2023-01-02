# Introduction to JSX

JSX stands for **JavaScript XML**. JSX allows us to write HTML elements in JavaScript and place them in the DOM without any `document.getElementById()`, `createElement()` or `appendChild()` methods. JSX is faster than normal JavaScript language. JSX is used to convert HTML tags into react elements.

JSX is not mandatory to use there are other languages to develop react applications. But programmers find it easy to use JSX to develop react applications.

JSX allows writing expressions in curly `brackets { }`. The expression can be any JS expression or React variable.

JSX is much closer to JavaScript than to HTML, it uses camelCase notation for naming convention.

For example, `class` becomes `className` in JSX, and `tabindex` becomes `tabIndex`.

JSX elements must be closed using `/`.

We can get Hello World on the screen by writing the code. for example

The index.html file must have a div with id="root" and append by using the following code within index.js file.

```javascript
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
    <p>Hello World</p>
);
```

The output we got

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672637770208/fa3de45a-a4b4-497e-9db5-229357a70313.jpeg align="center")
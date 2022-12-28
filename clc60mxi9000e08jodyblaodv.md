# What is DOM and BOM in JavaScript?

## Window Object

For understanding the concept of BOM and DOM first we need to understand about window object. All objects, functions, and variables are a part of the window object.Both BOM and DOM are window objects.

## BOM

BOM stands for Browser Object Model. The BOM is the window object that represents a window in the browser. We can manipulate the browser window with the `window` object and add various events using BOM properties. The DOM is a subset of BOM object and we can access DOM by using `document` properties and methods. Apart from `document` BOM also have `history`, `screen`, `location` etc.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672132602059/cab37ae6-626d-4f6d-bc1d-566ee3864689.jpeg align="center")

## DOM

It stands for Document Object Model. Document Object Model in JavaScript is used to access the elements inside the document. It maps the entire Document into a hierarchy of parent and child in tree structure along with its properties and methods. The `document` object represents the whole HTML document. When an HTML document is loaded in the browser, it becomes a document object, and you can use `document` object to manipulate the web page.

We can change an element's text, element's color, hide and show elements, add an event listener to the HTML elements etc.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672132648388/a87db111-ea4d-453a-ab8e-dda198a58443.png align="center")
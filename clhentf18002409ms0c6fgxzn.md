---
title: "How to use componentWillUnmount() in React Functional Components"
datePublished: Mon May 08 2023 09:47:55 GMT+0000 (Coordinated Universal Time)
cuid: clhentf18002409ms0c6fgxzn
slug: how-to-use-componentwillunmount-in-react-functional-components
tags: react, reactjs, lifecycle, reacthooks, lifecycle-in-react

---

Functional components are better than class based components in React in terms of working as well as maintaining. There is also less code that is needed to be written to get same results.

The class components have different lifecycle methods that are used to accomplish different functionalities at different times. Some methods are componentDidMount(), componentDidUpdate(), shouldComponentUpdate() and componentWillUnmount().

In functional components all the work of the lifecycle methods is handled by using only one hook i.e. useEffect() hook. We can apply various lifecycle methods by using this single hook.

useEffect() is used to manage API calls that happened on a componentDidMount(), but never componentWillUnmount(). And the interesting thing is that it turns out to be both componentDidMount() and componentWillUnmount(). The logic behind this is very simple.

Everything that is written within first parameter (callback function) act similar to the componentDidMount(). But when we pass a function in the return statement of first parameter of useEffect(), it will act as the componentWillUnmount() function.

```javascript
useEffect(() => {
  // Anything in here is fired on component mount.
  // componentDidMount
  
  return () => {
  // Anything in here is fired on component unmount.
  // componentWillUnmount
  };
  }, []);
```
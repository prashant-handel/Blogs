---
title: "Redux Principles"
datePublished: Fri Mar 31 2023 09:24:12 GMT+0000 (Coordinated Universal Time)
cuid: clfwc8jnm000z09l04w6nf23n
slug: redux-principles
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1680254427362/593613ab-793f-48ef-a315-ce5590c855de.png
tags: reactjs, html5, redux, store, redux-toolkit

---

### First Principle

**"The state of your whole application is stored in an object tree within a single store."**

It means that the state of our application is maintained in a single object which the Redux storage would manage.

**For example-**

If we have a state named `count` and a function for the increase of the count state.

If we click the increase button, the count value updates and is stored in the Redux store.

The count object-

{

count: 0

}

### Second Principle

**"The only way to change the state is to dispatch an action, an object describing what happened."**

It means that to update the state of your app, you need to let Redux know about that with action.

You are not allowed to directly update the state object.

Let us take the previous example, for incrementing the value of the count we have to pass an action to the Redux store before updating the value.

The action is a simple object contains a type property indicating your action.

{

type: increment

}

### Third Principle

**"To specify how the state tree is transformed by actions, you write pure reducers."**

It defines how the state changes. The reducer is like a function that takes previousState and action as parameters and returns newState.

const reducer = (state, action) =&gt;{

switch (action.type){

case increment: return{

count: state.count+1

}

}

}

```javascript
const reducer = (state, action) =>{
    switch (action.type){
        case increment: return{
        count: state.count + 1
        }
    }
}
```

Redux works on these three principles. Let us take a simple JavaScript Application, the state of the application is maintained separately in the Redux Store. The JavaScript App is always subscribed to the Redux Store.

The store cannot directly update the state. Whenever the application wants to update the state, the application has to dispatch an action.

The reducer then handles the action and updates the current state. Thus the app is subscribed to the JavaScript Application, it updates the state in the application too.

We can understand it easily through the image.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680254567142/1a8b524f-12e1-4703-8afd-956b701425ae.jpeg align="center")
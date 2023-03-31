---
title: "Actions, Reducer and Store in Redux"
datePublished: Fri Mar 31 2023 10:56:08 GMT+0000 (Coordinated Universal Time)
cuid: clfwfiruj000109kv0x1m0678
slug: actions-reducer-and-store-in-redux
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1680260133692/423f1e65-3a56-4b5d-a63b-2a96b55586ae.png
tags: javascript, react, reactjs, redux, redux-toolkit

---

### Actions

Action is the only way for the interaction between the store and the application.

It carries some information from the application to the Redux store.

Actions are plain JavaScript objects.

It must have a 'type' property that informs about the type of action to be performed.

The 'type' property is defined as string constants.

### Reducer

Reducer specifies how the app's state changes in response to the actions sent to the store.

It is a function that accepts state and action as arguments and returns the next state of the application i.e.

(previousState, action) =&gt; newState

### Redux Store

There is only one store for the entire application.

There are various responsibilities of the Redux store, such as-

It holds the application's state.

It allows access to the state using `getState()`.

It provides a method `dispatch(action)` that allows updating the state.

It also provides a method called subscribe(listener) which is executed whenever the state in the Redux Store changes.
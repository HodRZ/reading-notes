# State, Props, and the Component Lifecycle

## Prop  -  State
**Props and states** are two ways to handle data inside a React App; *data* and its management data is an important factor in React, this data can be imported from outside your component or created inside it, if it's **imported it's Prop**, and if it's **created -*setted*- inside your component it's called *State***

**Props** are used as an arguments to pass inside the constructor component, where it's rendered to the user. **State** is used to handle data recieved from the user on the current component.

Since **props** are *imported* from other components, they don't affect the current component. **state** on the other hand, is data handled **inside** the component, so updating it causes the component to be rendered again

---

## The Component Lifecycle

the steps that the component goes through from the moment it's created till it's removed from the DOM are called **the Component Lifecycle Events**, and these phases are:

1. Mounting
2. Updating
3. Unmounting


![lifecycle](https://miro.medium.com/max/1400/0*0saPKFiTUk6W3FYp)


*During* these phases we can use some methods as shown in figure to control the component behaviour at an exact stage of execution. Take as an example the `componentDidMount()` method, this method is invoked the moment a component is mounted *or rendered to the DOM* this makes it a good place for the `setState()` method.

the lifecycle of the component begins in the **mounting phase** starting with the constructor, render, componentDidMount, componentWillUnmount, React updates.





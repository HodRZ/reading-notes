# React and Form

- ## Forms

**Form** elements interact with *React* in an interesting way; React focuses on state management for each component, but *HTML Forms* keep some internal state **-Control of own state-** and render data from the DOM not *React state* *ex: user input*, this can work in *React*, but its more convenient to let *React* **Control** the state and make it the **single source of truth**.

an element that controls it's own state is an **Uncontrolled Component**, and one where the state is managed be *React* is a **Controlled Component**. controlling the component can be achieved by having a *watcher* method *(ex:`onChange`)* that watches the change in the element and change the state accordingly.

this also relates to the idea of **one way data binding**, where there is only one place to represent the state of the *App* and UI listens to it and change only if data at this place is changed

![react one-way binding](https://i.stack.imgur.com/JoHqS.jpg)

![react flow](https://i.stack.imgur.com/qDpID.jpg)

---

- ## The Conditional (Ternary) Operator

we use it to shorten *if statements*

`if(x===y){
  console.log(true);
} else {
  console.log(false);
}`

`console.log((x===y)? true: false)`

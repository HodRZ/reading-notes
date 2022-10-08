# React Hooks, useState

## useEffect

The useEffect hook in React allows the developer to produce a **side effect** from a function, this hook as everything else in React is envoked as a function, so it runs when the component function is envoked, React will mount the component and do the initial render, then it will look to see of it there's any side effect needed or a state to be updated, then it will run according to the code.

So, how React would know when to produce the effect? The answer is the **dependency array**, the useEffect hook will watch the dependency array for any changes, and if one found the effect will fire.

The dependency array can be an **empty array, a variable/set of variables, or not provided at all**

The difference between the three options is:

- an empty array will let the effect fire once, since diffing between empty values will return nothing

- an array of dependency will let the effect fire whenever the variable change;like being dependent on a state variable and it will fire when the state change

- not providing an array will the give the function nothing to diff so the function will be invoked as a loop

---

## useState

The useState hook is provided to the developer to subscribe to the global React module; React hooks are coded using the **module pattern**, which relies on **closures**, using the state allows the developer to close over a variable that can persist and passed between components.

useState return a **state** variable and **setState** setter for the variable, and the setter is responsible for only its coupled state variable,these states are closed over in an array in the module scope and the values are accessed using indices.

One of the major confusions in React is the nature of useState, the general way of thinking about because of its behavior is that it's an async function, but the what happens is that tge state is updated in **batches**; the states in a component will be *deferred* after the render of the component, in current version of react, if we have 2 state setters then an async call then a third state setter, the first two will run in a batch, then the third one will be run after the async call, and it's proposed for future versions to update the whole component state in one batch.

Updating the state in batches is due to **reconciliation**, as to have a single source of truth for the state and the props 

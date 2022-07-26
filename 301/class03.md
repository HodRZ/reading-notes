# Passing Functions as Props

## Lists and Keys

- **Map**

In Javascript, `map()` is used to itterate over an array and transform it, and this works almost the same way in React.

`map()` is used in React to create a list of elements and include them as a bulk in *JSX*

Now, an important thing to consider, is that Reacts will throw and error that each elemnt in the list needs a **key**. Keys are a special string attribute that gives every element a unique identity, this helps React identify which element have changed, added, or removed.

---

- **`...` the Spread Operator**

The spread operator is a feature that helps in speeding up the flow of work, it takes an iterable and allows it to be expanded.

the spread can be used in:

- Function Argments
- Array Literlas
- Object literals

and can be used for ex:

- Copying an array.
- Concatenating or combining arrays.
- Using Math functions.
- Using an array as arguments.

---

- **Passing Functions Between Components**

[Passing Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

as shown in the video above, the first thing the developer did is creating the increment function inside the parent where ths *State* is.

the `increment()` function takes the name that needs to be updated, then loops through the array of people (data) to update the counter(state) of that name.

the function is passed the same way the props are passed to the child, and within the child the function is added by `this.props.function` and invoked the same way a function is invoked within the child

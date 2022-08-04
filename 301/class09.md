# Fuctional Programming

**Functional Programming** is a programming paradigm; other paradigms are *OOP* where you have objects and methods, or *imperative* where you give your computer a recpe to do something, in **functional programming**, it's also a style of coding and a mindset!

lets be honest, *OOP* is confusing at best and cry-all-night at worse! inheritance? this? **Functional** programming is simpler.

in **Functional Programming** everything is a function, something that takes in an input and gives an output.

An important concept in *functioal programming* is **avoiding side effects** and use **pure functions**, a *side effect* is anything that a function might do that isn't computing the output from the input, or if the function uses some global variable to compute the output that doesn't depened only on the input thats not a pure function, or if the function is not *deterministic*; meaning it doesn't give the same outpu for the same input. so a **Pure Function** only takes its input, compute it, and returns an output.

Another important concept is **Immutability**, which means that the data inside the function keeps its state to make the function more consistent and predictable.

When a function is **Immutable** and **Pure** we call **referentially transparent** and this helps when working with **Higher Order Functions**

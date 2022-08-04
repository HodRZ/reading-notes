
# The Call Stack

The *JavaScript Interpreter* has two types of memory; the **Heap** *(Long-lived)* and the **Call Stack** *(Short-Lived)*, the *Call stack* is used to store and organise functions invocations *(Calls)*.

since JS interpretation is *Single-threaded* it runs functions *to-completion*, and that means *the stack* data structure, as its name implies, is **Last In First Out**, so when a function is called, its pushed to the call stack to form a *stack frame*, the call stack will keep track of this frame, and if another function was invoked inside the first one, or the function itself was recursive, another frame will be push to the call stack.

![callstack](https://miro.medium.com/max/1838/1*NHvc4BArOnXfo7Afg6LFMg.png)

sometimes a **Stack overflow** error will occur; since the call stack is a place in memory, it has its own size, and usually its small (in chrome the stack is 60,000 call), so when that number is exceeded, the stack will overflow and throw an error.

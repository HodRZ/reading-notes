# Node.JS

JavaScript when its first created was used to run on the browser, and it was imposible to run it on the servers that used languages like Java or PHP, so when Node.JS was intrudecued in 2009 it revolutionazed web development because it allowed the developer to write a full-stack app with one languague!
Node.JS is not a programming laguage, but a runtime that allows the user to run Javascript on a server.

>Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

The above is called *implementaion details* of JavaScript , and the JavaScript engine must handle these details. **Google’s V8 Engine** is one of the most popular implementaions, it uses **JIT compilation** and this make it faster that a regular interpreter.

JS is **event-based** means that everything in node is a reaction to an event, ex: a click will happen that will invoke a function, then JS will run a function **to completion** before moving on to the next function, but this might cause a problem  if a function took too long in the stack, it will **block** the loop from continuing, thats why there're multiple task queues in JS runtime, *if a function needs time to resolve it can be pushed to the (micro/macro) queue and clear the call stack for other functions,

![event loop](https://uploads-ssl.webflow.com/62c6fbddb12bb54622241c3d/62c6fbddb12bb523df242285_event_loop_animation-gif.gif)

---
you can install Node.JS directly by grabing a binary for your system from the oficcial web-site, or by using a version manager ex:brew, and what s great is that NodeJS comes with a package manager **npm** *Node.JS Package Manager* to install modules from the thousands of modules available by the huge eco system of this runtime

i run the LTS version 16.15.1 of Node and 8.13.2 of npm

using npm is simple you just type ex: `npm install jshint` and it will install the module for you, and you decide if you want it globally or locally using option like `npm -g moduleName`

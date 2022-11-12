# Chakra UI

## What is Chakra UI ?

>Chakra UI is a simple, modular and accessible component library that gives you the building blocks you need to build your React applications.

**Chakra UI** is a UI components library that contains styled ready-to-use components for frontend applications.

___

## Comparsion with other libraries / frameworks

Although using a component library may speed up development, but using a framework *(ex:TailWindCSS)* maybe better as its not opinionated and provides more customization.

## Getting started with ChakraUI

to use Chakra UI in your application, you first need to install it using

`npm i @chakra-ui/react @emotion/react @emotion/styled framer-motion`

or crate a react app with the Chakra UI template:

`npx create-react-app my-app --template @chakra-ui`

then wrap the whole app tree in Chakra provider component

``` jsx
import * as React from 'react'`

import { ChakraProvider } from '@chakra-ui/react'

function App() {
  return (
    <ChakraProvider>
      <App />
    </ChakraProvider>
  )
}
```

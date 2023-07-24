# REACT 3

1. What is React Context, and how does it help in managing state and data sharing in a React application?

   - React Context is a way to share data between components in a React application without having to pass props down manually at every level. It is a built-in feature of React, and it is a great way to manage state and data sharing in your applications.
   - Context is primarily used when some data needs to be accessible by many components at different nesting levels.
   - Context is similar to props, but it is designed to pass data through the component tree without having to pass props down manually at every level.
  

2. Explain the useContext Hook and how it can be used to access data from a React Context within a functional component.

   - The useContext hook is a React hook that allows you to access data from a React Context within a functional component.

   - To use the useContext hook, you first need to create a context using the createContext() method. This method takes two arguments: the name of the context and a default value.
   - The useContext() hook returns an object with the data from the context

3. Describe the purpose of Next.js, and provide an example from the Vercel Next.js Examples reading on how it can be used to build a scalable web application.

    - Next.js is a React framework that allows you to build server-side rendered (SSR) React applications. It is a great way to build scalable web applications because it allows you to build a React application that is rendered on the server and then sent to the client.
    - It provides a number of features that make it ideal for building scalable web applications, including:

       - Server-side rendering (SSR): Next.js renders your pages on the server before sending them to the client. This can improve the performance of your application by reducing the amount of work that the client's browser has to do.
       - Automatic code splitting: Next.js automatically splits your code into smaller chunks that can be loaded on demand. This can improve the performance of your application by reducing the amount of code that needs to be loaded on the client's browser.


  
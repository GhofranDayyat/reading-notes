# Context API

* Context API is a (kind of) new feature added in version 16.3 of React that allows one to share state across the entire app (or part of it) lightly and with ease
*  Context API is a way for a React app to effectively produce global variables that can be passed around, it's   alternative to "prop drilling" or moving props from grandparent to child to parent, and so on.
* Context is primarily used when some data needs to be accessible by many components at different nesting levels. 
*  don't pass down the Avatar component itself so that the intermediate components don’t need to know about the  props=====>  only the top-most Page component need to know 
* **Benefit**
 1. make your code cleaner in many cases by reducing the amount of props you need to pass through your application 
 2. giving more control to the root components

* **Creates a Context object** ``const MyContext = React.createContext(defaultValue)`
* When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.
* The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. 
 1. ``Context.Provider`` ===> ``<MyContext.Provider value={/* some value */}>``
 2. ``Class.contextType``
 3. ``Context.Consumer``
 4. Context.displayName

 # Q
1. Describe use cases for ``useMemo()`` and ``useReducer()``?
- **useMemo** is a React hook that memorizes the output of a function
- **useReducer** is usually preferable to useState when you have complex state  logic that involves multiple sub-values or when the next state depends on the previous one

2. Why do custom hooks need the use prefix?
- Should start with use so that you can tell at a glance that the rules of Hooks apply to it.

3. What do custom hooks usually do?
- Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks


4. Using any list of custom hooks, research and name one that you think will be useful in your applications
- **use-location hook**
The name says it all, this hook is used for getting the location of the browser.

5. Describe how a hook that fetches API data might work
- useEffect can make a network requeset on component render, when the fetch resolves, it can set the response from the server to the local state using the setState function, which will cause the component to render to update the DOM with the data.
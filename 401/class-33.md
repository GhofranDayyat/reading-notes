# Context API

* Context API is a (kind of) new feature added in version 16.3 of React that allows one to share state across the entire app (or part of it) lightly and with ease
*  Context API is a way for a React app to effectively produce global variables that can be passed around, it's   alternative to "prop drilling" or moving props from grandparent to child to parent, and so on.
* Context is primarily used when some data needs to be accessible by many components at different nesting levels. 
*  don't pass down the Avatar component itself so that the intermediate components don’t need to know about the  props=====>  only the top-most Page component need to know 
* **Peneft**
 1. make your code cleaner in many cases by reducing the amount of props you need to pass through your application 
 2. giving more control to the root components

* **Creates a Context object** ``const MyContext = React.createContext(defaultValue)`
* When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.
* The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. 
 1. ``Context.Provider`` ===> ``<MyContext.Provider value={/* some value */}>``
 2. ``Class.contextType``
 3. ``Context.Consumer``
 4. Context.displayName
Context API --> Context provides a way to pass data through the component tree without having to pass props down manually at every level.
  1. In a typical React application, data is passed top-down (parent to child) via props, but this can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.
  2. Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.
  3. Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.
  4. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.
    4.a. https://reactjs.org/docs/composition-vs-inheritance.html
  5. Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes.
  6. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree.
  7. The contextType property on a class can be assigned a Context object created by React.createContext(). This lets you consume the nearest current value of that Context type using this.context. You can reference this in any of the lifecycle methods including the render function.
  8. Context object accepts a displayName string property. React DevTools uses this string to determine what to display for the context.
  9. Because context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders.
  

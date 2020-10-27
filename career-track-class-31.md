React Custom Hooks --> Building your own Hooks lets you extract component logic into reusable functions.
  1. When we want to share logic between two JavaScript functions, we extract it to a third function. Both components and Hooks are functions, so this works for them too!
  2. A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.
  3. Just like in a component, make sure to only call other Hooks unconditionally at the top level of your custom Hook.
  4. Unlike a React component, a custom Hook doesn’t need to have a specific signature. We can decide what it takes as arguments, and what, if anything, it should return. In other words, it’s just like a normal function. Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.
  5. Custom Hooks are a convention that naturally follows from the design of Hooks, rather than a React feature.
  6. Custom Hooks are a mechanism to reuse stateful logic (such as setting up a subscription and remembering the current value), but every time you use a custom Hook, all state and effects inside of it are fully isolated.

Rules of Hooks
  1. Only Call Hooks at the Top Level --> Don’t call Hooks inside loops, conditions, or nested functions. Instead, always use Hooks at the top level of your React function. By following this rule, you ensure that Hooks are called in the same order each time a component renders.
  2. Only Call Hooks from React Functions. Don’t call Hooks from regular JavaScript functions. Instead, you can:
    2.a. Call Hooks from React function components.
    2.b. Call Hooks from custom Hooks.
    2.c. We released an ESLint plugin called eslint-plugin-react-hooks that enforces these two rules.
      2.c.1. npm install eslint-plugin-react-hooks --save-dev
      

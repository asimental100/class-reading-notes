setState() --- the only legitimate way to update state after the initial state setup.
  1. React components can, and often do, have state. State can be anything, but think of things like whether a user is logged in or not and displaying the correct username based on which account is active. Or an array of blog posts. Or if a modal is open or not and which tab within it is active. React components with state render UI based on that state. When the state of components changes, so does the component UI.
  2. React Reconciliation
    2.a. This is basically kicking off a process that React calls reconciliation. The reconciliation process is the way React updates the DOM, by making changes to the component based on the change in state. When the request to setState() is triggered, React creates a new tree containing the reactive elements in the component (along with the updated state). This tree is used to figure out how the Search component’s UI should change in response to the state change by comparing it with the elements of the previous tree. React knows which changes to implement and will only update the parts of the DOM where necessary. This is why React is fast.
    
Handling Events in React
  1. Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:
    1.a. React events are named using camelCase, rather than lowercase.
    1.b. With JSX you pass a function as the event handler, rather than a string.
    1.c. You cannot return false to prevent default behavior in React. You must call preventDefault explicitly.
    
Snapshot Testing with Jest
  1. Snapshot tests are a very useful tool whenever you want to make sure your UI does not change unexpectedly. A typical snapshot test case renders a UI component, takes a snapshot, then compares it to a reference snapshot file stored alongside the test. The test will fail if the two snapshots do not match: either the change is unexpected, or the reference snapshot needs to be updated to the new version of the UI component.
  2. A similar approach can be taken when it comes to testing your React components. Instead of rendering the graphical UI, which would require building the entire app, you can use a test renderer to quickly generate a serializable value for your React tree.
  
React Testing Library
  1. The react-testing-library is a very light-weight solution for testing React components. It provides light utility functions on top of react-dom and react-dom/test-utils, in a way that encourages better testing practices. Its primary guiding principle is: "The more your tests resemble the way your software is used, the more confidence they can give you." - Kent C. Dobbs
  2. This library is a replacement for enzyme. While you can follow these guidelines using enzyme itself, enforcing this is harder because of all the extra utilities that enzyme provides (utilities which facilitate testing implementation details).
  

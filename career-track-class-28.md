Architectural Styles & Architectural Patterns
  1. Architectural Pattern - is a general and reusable solution to an occurring problem in a particular context. It is a recurring solution to a recurring problem. The purpose of Architectural Patterns is to understand how the major parts of the system fit together and how messages and data flow through the system. We can have multiple patterns in a single system to optimize each section of our code.
    1.a. Architectural Patterns are similar to Design Patterns, but they have a different scope. In a few words, while Design Patterns impact a specific section of the code base, Architectural Patterns are high-level strategies that concern large-scale components, the global properties and mechanisms of a system.
  2. Architectural Style - is a name given to a recurrent Architectural Design. It doesn’t exist to solve a problem.
    2.a. A single architecture can contain several Architectural Styles, and each Architectural Style can make use of several Architectural Patterns. An Architecture Patterns can be a subset of an Architectural Styles targeting a specific scope.
    2.b. We can use the same words used by the Building Architecture domain, where an Architectural Style is characterized by the features that make a building notable and historically identifiable. A style may include such elements as form, a method of construction or building materials.
  3. Idiom is also a term that we can regularly meet. An Idiom is a low-level pattern specific to a programming language. It describes how to implement particular aspects of the components or the relationships between them using the features of a given language.

Container and Presentation Pattern
  1. The container and presentation pattern splits code into two distinct places:
    1.a. Containers - are stateful components that contain your business login.
      1.a.1. Container components “[a]re concerned with how things work”1. In this role they manage state, fetch data from APIs, setup event handlers, and pass information to other components via props.
      1.a.2. Container components are responsible for specifying how a section of our application works. They manage state, fetch data from apis, and setup event handlers.
      1.a.3. When the Container/Presentation pattern first became popular all containers were class based components. At that time state and lifecycle methods were only available within class components. Since containers are responsible for managing state and fetching data (lifecycle methods) they were exclusively written as class components. This helped highlight the dichotomy between container components (classes) and presentational components (functions). Class container components are created by extending the react Component class.
    1.b. Presentations - are stateless components that present your data.
      1.b.1. Presentation components “[a]re concerned with how things look” In this role they receive props and use those props to render and style DOM.
      1.b.2. Presentation components are responsible for specifying how a section of our page looks. They create DOM and styles.
      1.b.3. Presentational components are written as functional components. They return the markup that is going to get rendered to the DOM.
      1.b.4. When we pass props into our component we should use the prop-types package to specify the props our component receives. This gives us convenient warning messages if we forget to pass a prop or pass a prop with the wrong type.
      
Functional vs Class-Components in React
  1. A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.
    1.a. Because a functional component is just a plain JavaScript function, you cannot use setState() in your component. That’s the reason why they also get called functional stateless components. So everytime you see a functional component you can be sure that this particular component doesn’t have its own state.
    1.b. Functional component are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks.
  2. A class component requires you to extend from React.Component and create a render function which returns a React element.
    2.a. If you need a state in your component you will either need to create a class component or you lift the state up to the parent component and pass it down the functional component via props.
    2.b. Another feature which you cannot use in functional components are lifecycle hooks. The reason is the same like for state, all lifecycle hooks are coming from the React.Component which you extend from in class components. So if you need lifecycle hooks you should probably use a class component.
  
Conditional Rendering
  1. In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.
  2. Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.  
  

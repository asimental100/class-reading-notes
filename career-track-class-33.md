Composition vs Inheritance --> React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.
  1. Containment
    1.a. Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”. We recommend that such components use the special children prop to pass children elements directly into their output. This lets other components pass arbitrary children to them by nesting the JSX
  2. Specialization
    2.a. Sometimes we think about components as being “special cases” of other components. For example, we might say that a WelcomeDialog is a special case of Dialog. In React, this is also achieved by composition, where a more “specific” component renders a more “generic” one and configures it with props. Composition works equally well for components defined as classes.
  3. Props and composition give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way. Remember that components may accept arbitrary props, including primitive values, React elements, or functions.
  4. If you want to reuse non-UI functionality between components, we suggest extracting it into a separate JavaScript module. The components may import it and use that function, object, or a class, without extending it.
  

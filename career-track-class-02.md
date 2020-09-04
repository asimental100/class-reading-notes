MVC (Model View Controller)
  1. Request: the user sends request to Controller which handles the "request flow".
  2. Get Data: the controller will ask the model for information based on the request.
    a. The model interacts with the database and then handles the data logic before passing the data back to the controller.
  3. Get Presentation: the controller now interacts with the view in order to dynamically render the data it has recieved before sending the presentation back to the controller.
  4. Response: the controller now returns the presentation to the user.

Array Methods
  1. forEach(): This method can help you to loop over array's items.
  2. includes(): This method check if array includes the item passed in the method.
  3. filter(): This method create new array with only elements passed condition inside the provided function.
  4. map(): This method create new array by calling the provided function in every element.
  5. reduce(): The reduce() method applies a function against an accumulator and each element in the array (from left to right) to reduce it to a single value - MDN
  6. some(): This method check if at least one of array's item passed the condition. If passed, it return 'true' otherwise 'false'.
  7. every(): This method check if all array's item passed the condition. If passed, it return 'true' otherwise 'false'.
  8. sort(): This method used to arrange/sort array's item either ascending or descending order.
  9. Array.from(): This change all thing that are array-like or iterable into true array especially when working with DOM, so that you can use other array methods like reduce, map, filter and so on.
  10. Array.of(): This create array from every arguments passed into it.
  
Classes - a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 classalike semantics.

MVC definitions
  Model: The Model component corresponds to all the data-related logic that the user works with. This can represent either the data that is being transferred between the View and Controller components or any other business logic-related data. For example, a Customer object will retrieve the customer information from the database, manipulate it and update it data back to the database or use it to render data.
  View: The View component is used for all the UI logic of the application. For example, the Customer view will include all the UI components such as text boxes, dropdowns, etc. that the final user interacts with.
  Controller: Controllers act as an interface between Model and View components to process all the business logic and incoming requests, manipulate data using the Model component and interact with the Views to render the final output. For example, the Customer controller will handle all the interactions and inputs from the Customer View and update the database using the Customer Model. The same controller will be used to view the Customer data.
  

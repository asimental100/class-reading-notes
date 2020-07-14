Make sure I fully understand the "problem domain" before I start to code because it fill save me a lot of time and frustration.

Objects: groups together a set of variables and functions to create a model of a something you would recognize from the real world.
  1. If a variable is part of an object, it is called a property. Properties tells us about the object, such as the name of a hotel or the number of rooms it has.
  2. If a function if part of an object, it is called a method. Methods represent tasks that are associated with the object.
    2.a. For example: you can check how many hotel rooms are available by subtracting the number of booked rooms from the total number of rooms.
  3. Variables and their values are called key-value pairs and are formatted like this = key:value, key:value, key:value
  4. Named functions are also thought of as key-value pairs, with the function name serving asa the key and the code block serving as the value.
    4.a. The format for methods (functions within objects) looks like this: functionName: function() { code to execute; }
    
NodeList: a collection of element nodes. Each node is given an index number (a number that starts at zero, just like arrays).
  1. The order in which the element nodes are stored in a NodeList is the same order that they appear in the HTML page.
  2. Live NodeLists: when your script updates the page, the NodeList updates at the same time.
    2.a. Methods beginning with "getElementBy..." return live NodeLits. These are typically faster to generate than static NodeLists.
  3. Static NodeLists: when your script updates the page, the NodeList is not updates to reflect the changes made by the script.
    3.a. the new methods that begin with "querySelector..." return static NodeLists. They relect the document when the query was made and do not update with script changes.
  4. The "item() method" which will return an individual node from the NodeList in a similar fashion to how you select an specific element in an array.
    4.a. Despite their similarities using Array syntax (simply using [] brackets) is preffered over the item() method because it faster.

createElement() method: allows you to create new elements.

appendChild() method: allows you to specify which element you want this node added to, as a child of it.

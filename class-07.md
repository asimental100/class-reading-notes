Basic Table Structure
  1. The table element is used to create a table. The contents of the table are written out row by row.
  2. The tr element indicates the start and end of each table row. Table rows are filled with table data.
  3. The td element is where we store the table data.
  4. The th element is used just like the td element but its purpose is to represent the heading for either a column or a row.
    4.a. Can use empty td and th elements to ensure that the table renders correctly.
    4.b. Can use colspan="number" to have a td or th element span any number of columns.
    4.c. Can use rowspan="number" to have a ted or th element span any number of rows.
  5.The thead element is where the header of the table should be stored.
  6. The tbody element is where the main table elements should be stored.
  7. The tfoot element is where the footer of the table should be stored.

Three Groups of Built-In Objects
  1. Browser Object Model: creates a model of the browser tab or window. The topmost object is the window object, which represents the current browser window or tab.
    1.a. The Window Object's child objects represent other browser features such as:
      1.a.1. Document: Current Webpage
      1.a.2. History: Pages in browser history
      1.a.3. Location: Url of current page
      1.a.4. Navigator: Information about Browser
      1.a.5. Screen: Device's display information
  2. Document Object Model: creates a model of the current web page.
    2.a.The topmost object is the document object, which represents the page as a whole, its child objects represent other items on the page.
      2.a.1. Examples include html, head, body, title, div, p, text, etc.
  3. Global Javascript Objects: the global objects do not form a single model. they are a group of individual objects that relate to different parts of the JavaScript language.
    3.a. The names of the global objects usually start with a Capital letter (ex. String and Date objects).

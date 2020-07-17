How Forms Work: A user fills in a form and then presses a button to submit the information to the server. The name of each form control is sent to the server along with the value the user enters or selects. Then the server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database. Lastly, the server creates a new page to send back to the browser based on the information recieved. 

Fieldset element allows you to group related form controls together inside of it.
  1. a legend element can come directly after the opening fieldset tag and contains a caption which helps identify the purpose of that group of form controls.

Background-image adds a background image to the input box (useful alternative to placeholder in text inputs to differentiate between say a name input and email input).

list-style-position: using the value of either "outside" or 'inside' you can change where the bullets/numbers of a list appear.

Different Event Types: Any of these events can be used to trigger a function in your Javascript code.
  1. UI Events: Occurs when a user interacts with the browser's user interface (UI) rather than the web page.
    1.a. load - web page has finished loading
    1.b. unload - web page is unloading (usually because a new page was requested)
    1.c. error - browser encounters a JavaScript error ot an asset doesn't exist
    1.d. resize - browser window has been resized
    1.e. scroll - user has scrolled up or down the page
  2. Keyboard Events; Occur when a user interacts with the keyboard (see also input event)
    2.a. keydown - user first presses a key (repeats while key is depressed)
    2.b. keyup - user releases key
    2.c. keypress - character is being inserted (repeats while key is depressed)
  3. Form Events: Occur when a user interacts with a form element
    3.a. input - value in any input or textarea element has chnaged or any element with the contenteditable attribute
    3.b. change - value in select box, checkbox, or radio button changes
    3.c. submit - user submits a form (using a button or a key)
    3.d. reset - user clicks on a form's reset button (rarely used these days)
    3.e. cut - user cuts content from a form field
    3.f. copy - user copies content from a form field
    3.g. paste - user pastes content into a form field
    3.h. select - user selects some text in a form field

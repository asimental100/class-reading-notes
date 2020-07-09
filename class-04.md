Email Links
  1. To create a link that starts up the user's email program and addresses and email to a specific email address you use teh <a> element. However this time the value of the href attribute starts with "mailto:" and is followed by the specific email address where the email should be sent.
Opening Links in A New Window
   1. To open a link in a new window you use the "target" attribute with a value of "_blank" in the opening <a> element after the href attribute.
Linking to a Specific Part Page
   1. You can link to specific parts of the same page by using the href attribute inside the opening <a> element tag by using double quotation marks and the # sign followed by the section you wish to link to's id.
   2. You can also link to specific parts of other pages by using the # symbol followed by the specific part's id directly follwing the url link
    2.a. Example: <a href="https:/www.htmlandcssbook.com/#bottom"> will take you to that page and the bottom section of it.
Block-level Elements: Start on a new line
   1. Examples include: <h1> <p> <ul> <li>
Inline Elements: flow in between surrounding text
   1. Examples include: <img> <b> <i>
Positioning Schemes
   1. Normal Flow (position:static;)
     1.a. The default behavior that causes every block=level element to appear on a new line.
   2. Relative Flow (position:relative;)
     2.a. Moves an element in relation to where it would have been in Normal Flow. (example you can move it 20% or 20px to right from where it would have been).
   3. Absolute Flow (position:absolute;)
     3.a. This moves an element out of normal flow and it no longer effects the elements surrounding it. These elements also move as the user scrolls up and down.
   4. Fixed Flow (position:fixed;)
     4.a. This is a form of absolute positioning that positions the element in relation to the browser window, as oppossed to the containing element.
     4.b. Elements with fixed positioning do not affect the position of the surrounding elements and they do not move as the user scrolls up and down.
   5. Floating Elements
     5.a. Floating an element allows you to take that element out of normal flow and position it to the far right or left of a containing box.
     5.b. the floated element becomes a block-level element around which other content can flow.
  
Pair Programming: the practice of two developers sharing a single workstation to interactively tackle a coding task together.
   1. Commonly involves two roles: the Driver and the Navigator. 
     1.a. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code.
     1.b. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.
   2. Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging.
 

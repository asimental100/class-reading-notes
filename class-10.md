The Seven Types of Built-In Error Objects in JavaScript
  1. Error - Generic error, the other errors are all based upon this error
  2. SyntaxError - Syntax has not been followed
  3. ReferenceError - Tried to reference a variable that is not delcared/within scope
  4. TypeError - An unexpected data type that cannot be coerced
  5. RangeError - Numbers not in acceptable range
  6. URIError - encodeURI(), decodeURI(), and similar methods used incorrectly
  7. EvalError - eval() function used incorrectly
NaN = Not a Number which is not considered a type error but instead simply means that you tried to preform a math operation using a value that is not a number.

Debugger - Using the 'debugger' keyword allows you to create a breakpoint in your code, thereby pausing the code when the developer tools are open.
  1. You can also place the debugger keywords in conditional statements to find out where the code is going
  2. Remove these keywords/conditionals before the code goes live.
  
Try, Catch and Finally - is a conditional form of code used in debugging. Try, Catch and Finally all get their own code block. With the try code block coming first then the catch codeblock which runs when there is an exception to try code block and then the code block for finally always get executed.
  1. Ex: try { try to execute this code } catch (exception) { If there is an exception, run this code } finally { this code always get executed }

Remember to try multiple browsers when testing code.

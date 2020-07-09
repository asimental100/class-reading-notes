Superscript & Subscript
  1. The <sup> element should be placed around characters to turn them into superscript.
  2. The <sub> element should be placed around characters to turn them into subscript.
  
External CSS
  1. The <link> element can be used in an HTML document to tell the browser where to find the CSS file.
    1.a. It lives inside the <head> element and should use 3 attributes:
      1.a.1. href: this specifies the path to the CSS file..
      1.a.2. type: this specifies the type of document document being linked to and it's value should be "text/css".
      1.a.3. rel: this specifies the relationship between the file being linked and the HTML file and when linknig to a CSS file it's value should be "stylesheet".
    1.b. It is an empty element, meaning that it does not need a closing tag.
Internal CSS
    1. You can also usee CSS rules within an HTML file by placing them inside the <style> element which usually sits in the <head> section of the page.
      1.a. The <style> element should have a type attribute with a value of "text/css".
Universal selector
    1. Use the * key in CSS to target all elements on the page.
Comparison Operators: Evaluating Conditions
    1. Is Equal to: == checks to see if two values are the same
    2. Strict Equal to: === checks to see if two values are the same and if they have the same data type
      2.a. 3 === '3' would return false
    3. Is Not Equal to: != checks to see if two values are not the same
    4. Strict Not Equal to: !== checks to see if two values are not the same and that the data types are not the same
      4.a. 3 !== '3' would return true
    5. Can compare two variables or simple a multitide of values by enclosing certain expressions in brackets
      5.a. var1 === (var2 + var3);
Logical Operators: evaulated left to right
    1. Logical and: && this operator tests more than one condition and requires them to both return true.
    2. Logical or: || this operator tests at least one condition for being true.
    3. Logical Not: ! this operator takes a single boolean value and inverts it.

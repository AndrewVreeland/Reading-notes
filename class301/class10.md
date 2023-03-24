# Reading

## [Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

1. What is a ‘call’?
      * A call is a function invocation
2. How many ‘calls’ can happen at once?
      * One at a time
3. What does LIFO mean?
      * Last in First out 
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

[Drawing for the callStack](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)

5. What causes a Stack Overflow?
      * A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.

## [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. What is a ‘reference error’?\
      * This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

      console.log(foo) // Uncaught ReferenceError: foo is not defined

2. What is a ‘syntax error’?
      * this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON 
at position 1
      * This can be solved by just fixing the syntax, in this case the object should be a JSON.

JSON.parse('{"foo":"bar"}')

3. What is a ‘range error’?
      * Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

var foo= []
foo.length = foo.length -1 // Uncaught RangeError: Invalid array length


4. What is a ‘type error’?
      * his types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

var foo = {}
foo.bar // undefined
foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined

5. What is a breakpoint?
      * a breakpoint is an intentional stopping or pausing placed for debugging errors.

6. What does the word ‘debugger’ do in your code?
      * debugger adds a break point 
## Bookmark and Review

[JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)
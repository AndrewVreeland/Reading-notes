# Functional Programming Concepts

## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

1. what is functional programming?
      * Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — [Wikipedia](https://en.wikipedia.org/wiki/Functional_programming)
2. What is a pure function and how do we know if something is a pure function?
      * it returns the same result if given the same arguments also known as deterministic.
      * no observable side effects
3. What are the benefits of a pure function?
      * the outcome of the function will not change becuase there are no external variables being used as arguments.
      * the code is easier to test
4. What is immutability?
      * the state of the data cannot change after being created
5. What is Referential transparency?
      *  a function or expression is referentially transparent if it can be replaced with its value or result without changing the meaning or behavior of the program. This property makes it easier to reason about and test code, as it ensures that the behavior of the program is predictable and consistent.

# Videos

## [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. What is a module?
      * modules will hold certain bits of code for each functionality. you then would call upon the module when needed.
2. What does the word ‘require’ do?
      * require('./count') acts a path to a module that you need in another js file. 
3. How do we bring another module into the file the we are working in?
      * module.export = counter;     ------ this allows the counter function to be exported from the counter module. Then you need to go to the app.js and name the require function like this,
      let counter = require('./count')
4. What do we have to do to make a module available?
      * let counter = require('./count')
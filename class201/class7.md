# Class 7 Reading Assignment

## *These are my notes from Module 7*

[Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

1. we need domaning modeling because;
      * it is a model that can be used by both technical and busisness teams. This allows the team working with the project to have better direction and work more fluid with one another.

[HTML Table Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

1. why should tables not be used for page layouts
      * Do Not use tables to layout web pages. they are used for tabular data. you lose accessibility for people using screen readers, tables produce 'tag soup' and they are also not automatically responsive like standard layour containers.
2. List and describe 3 different semantic HTML elements used in an HTML <table>.
      * <th> are table headers
      * <td> is the individual table cell
      * <table> hold the entirety of the tables data

[introducing constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)
1. What is a constructor and what are some advantages to using it?
      * a constructor function is a function that is utilized to 'dry' up your code. it allows different objects to call upon said function and reference it rather than having the function in the object itself. This allows for a cleaner database as well as more efficient code.
2. How does the term this differ when used in an object literal versus when used in a constructor?
      * when used within an object literal the term 'this' refers to the object itself whereas the term 'this' refers to the constructor function. 

[Object Protypes Using A Constructor](https://ui.dev/beginners-guide-to-javascript-prototype)

1. Explain prototypes and inheritance via an analogy from your previous work experience.

## Constructors

### What are they?

- A Special type of function
  - Act like a blueprint or 'factory' for objects
  - Start with a keyword 'function'

### why do we use them? 

# Class 8 Reading Assignment

## Loops

* A for loop repeats until a specified condition evaluates to false.
* A while statement executes its statements as long as a specified condition evaluates to true. 

### What Happens within a for statement loop

1. A for loop repeats until a specified condition evaluates to false.
2. The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
3. The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. Otherwise, the for loop terminates. (If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)
4. The statement executes. To execute multiple statements, use a block statement ({ }) to group those statements.
If present, the update expression incrementExpression is executed.
Control returns to Step 2.

### What Happens within a while statement loop

1. A while statement executes its statements as long as a specified condition evaluates to true.
2. If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.
3. The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.
4. To execute multiple statements, use a block statement ({ }) to group those statements.

## Terms

* Destructuring: For more complex assignments, the destructuring assignment syntax is a JS expression that makes it possible to extract data from arrays/objects using a syntax that mirrors the way array and object literals are constructed.

* Evaluation and Nesting:

1. Usually, assignments are used within a variable declaration (for example, with ‘const’, ‘let’, or ‘var’), or as standalone statements.
2. Assignment expressions like ‘x = f()’ though, will evaluate into a result value that can be used by another expression.
3. By chaining or nesting an assignment expression, the result can be assigned to another variable; logged; put inside an array literal or function call; etc.
4. When chaining expressions without () or other grouping operators, the assignment expressions will be grouped R to L, but evaluated L to R.
Avoid Assignment Chains

* Chaining/nesting: assignments in other expressions can create problems, so it’s discouraged.

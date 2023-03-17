Reading
[React Docs - Thinking in React]()

1. What is the single responsibility principle and how does it apply to components?
      * a component should only do one thing if it ends up growing it should be decompressed into smaller components
2. What does it mean to build a ‘static’ version of your application?
      * renders the UI from your data model without adding any interactivity
      * you’ll want to build components that reuse other components and pass data using props.
      * Don't use state at this point
3. Once you have a static application, what do you need to add?
      * you will need to add state by making the right components stateful
4. What are the three questions you can ask to determine if something is state?
      * Does it remain unchanged over time? If so, it isn’t state.
      * Is it passed in from a parent via props? If so, it isn’t state.
      * Can you compute it based on existing state or props in your component? If so, it definitely isn’t state!
5. How can you identify where state needs to live?
      * Identify every component that renders something based on that state.

      * Find their closest common parent component—a component above them all in the hierarchy.

      * Decide where the state should live:

            * Often, you can put the state directly into their common parent.

            * You can also put the state into some component above their common parent.

            * If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common parent component.

{Higher-Order Functions]()

1. What is a “higher-order function”?
      * Functions that operate on other functions, either by taking them as arguments or by returning them
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
      * function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
      * this function is taking 10 as one variable because of the code on line 37 and then 11 as the other variable because it is being passed in as an argument on line 38. after that it is doing a simple greater than comparison between the two numbers.
3. Explain how either map or reduce operates, with regards to higher-order functions.
      * map is considered a higher order function because it can take functions as arguments. map works by creating a new array by calling a function on each element within that array. 
      * Reduce is considered a higher order function because .... 
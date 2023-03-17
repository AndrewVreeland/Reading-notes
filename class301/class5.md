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








      What is the single responsibility principle and how does it apply to components?
The Single Responsibility Principle (SRP) is a fundamental software engineering concept and one of the five principles of object-oriented programming and design known as SOLID. It was introduced by Robert C. Martin and states that a class or module should have only one reason to change, meaning it should have only one responsibility or job.

Applying SRP to components, particularly in the context of component-based software engineering, leads to more maintainable, understandable, and modular code. Components can be user interface elements, code modules, or any other logical units in a software system.

When SRP is applied to components, it ensures that:

Each component has a clear and specific purpose, making it easier to understand, maintain, and modify.
Components are more reusable because they focus on a single task and don’t mix unrelated functionalities.
Components are more testable, as they have a smaller surface area for potential bugs and are simpler to test in isolation.
The overall system becomes more modular, allowing developers to replace or update components without affecting the rest of the system.
To apply SRP to components, developers should:
Identify the responsibilities of the system and create a component for each distinct responsibility.
Keep the interface and implementation of each component focused on its single responsibility.
Avoid mixing multiple responsibilities or concerns within a single component.
Continuously refactor and reevaluate components to ensure they adhere to SRP as the system evolves.
By adhering to the Single Responsibility Principle, developers can create more robust, maintainable, and modular software systems.
What does it mean to build a ‘static’ version of your application?
A “static” version of an application is created using pre-generated files like HTML, CSS, and JavaScript without server-side processing. Static applications offer faster load times, easier deployment, and improved scalability compared to dynamic applications. They are ideal for content that doesn’t change frequently, but have limited interactivity and real-time features. For applications requiring real-time data or user interactivity, dynamic applications or a combination of static and dynamic approaches may be more suitable.
Once you have a static application, what do you need to add?
After created a static application, you adding elements depends on the requirements:

Interactivity: Add client-side JavaScript to handle user interactions, like form submissions, animations, and navigation.
Real-time data: Integrate APIs or web services to fetch dynamic data, which can be displayed or manipulated using client-side JavaScript.
User authentication: Implement a user authentication system using third-party services like OAuth or 4. Firebase Authentication to allow for personalized experiences and protected content.
Server-side processing: Use serverless functions or back-end services for tasks like data processing, form handling, or generating dynamic content when needed.
Database integration: Connect to a database for storing and retrieving user-generated data or other dynamic content.
Progressive enhancement: Enhance the user experience by implementing Progressive Web App (PWA) features, like offline support, push notifications, and home screen installation.
SEO optimization: Improve search engine visibility with proper meta tags, structured data, and performance optimizations.
Accessibility: Ensure your application is accessible to all users by following accessibility best practices like ARIA landmarks, keyboard navigation, and proper color contrast.
Performance optimization: Optimize loading times by compressing images, minifying code, and leveraging caching and content delivery networks (CDNs).
Analytics: Integrate analytics tools like Google Analytics to track user behavior and understand how users interact with your application.
What are the three questions you can ask to determine if something is state?
To determine if something is state, use these question:

Changes over time?
Cannot be derived from other states or props?
Affects component rendering or behavior?
How can you identify where state needs to live?
To identify where state needs to live in your application or component hierarchy, follow these steps:

Identify components using the state: Determine which components rely on the state for rendering or behavior.
Find the closest common ancestor: Locate the nearest shared parent component in the hierarchy for all components identified in step 1.
Evaluate if lifting state is necessary: If the state is only used by one component and doesn’t impact siblings or parent components, it may not be necessary to lift the state.
Lift the state to the common ancestor: Move the state management to the closest common ancestor component, which will become the “source of truth” for that state.
Pass the state as props: From the common ancestor, pass the state and any necessary state update functions to the child components as props.
Higher-Order Functions
What is a higher-order function?
A higher-order function is a function that either takes one or more functions as arguments, returns a function as its result, or both. Higher-order functions are a fundamental concept in functional programming, allowing developers to create more abstract and reusable code by treating functions as first-class citizens.
Here are some common examples of higher-order functions:

map: A function that takes a function and a list (or other iterable) as arguments, applies the function to each element of the list, and returns a new list with the results.
filter: A function that takes a predicate function (a function that returns a boolean value) and a list as arguments, and returns a new list containing only the elements for which the predicate function returns true.
reduce: A function that takes a function, a list, and an optional initial value as arguments, and successively applies the function to the elements of the list, accumulating a single result value.
sort: A function that takes a comparison function and a list as arguments, and returns a new list with the elements sorted according to the comparison function.
bind: A function that takes a function and one or more arguments, and returns a new function with the arguments partially applied. This is useful for creating specialized versions of more general functions.
compose: A function that takes multiple functions as arguments and returns a new function that represents the composition of those functions. When the composed function is called, it processes its input by applying the original functions in sequence, passing the result of each function to the next.
pipe: Similar to compose, but it applies the functions in the order they were provided, rather than in reverse order. This can make the resulting code more readable in some cases.
memoize: A function that takes a function as an argument and returns a new function that caches the results of the input function for previously seen arguments, improving performance for expensive computations with repetitive inputs.
debounce and throttle: Functions that take a function and a time interval as arguments, and return a new function that limits the rate at which the input function is called, preventing excessive invocations during events like user input or scrolling.
forEach: A function that takes a function and a list (or other iterable) as arguments and applies the function to each element of the list. Unlike map, it doesn’t create a new list; it’s typically used for side effects, such as logging or updating the DOM.
Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true
The line is returning an arrow function, which takes a single argument, m. The purpose of this arrow function is to determine whether the value of m surpasses that of n.
Explain how either map or reduce operates, with regards to higher-order functions
The map function in the context of higher-order functions. map is a higher-order function that takes two arguments: a function (often called a callback) and a list (or other iterable). It applies the given function to each element in the list and creates a new list containing the results.

The map function is considered higher-order because it takes a function as an argument, showcasing the principle of treating functions as first-class citizens, a core concept in functional programming.

// Array of names
const names = ['Alice', 'Bob', 'Charlie', 'David', 'Eva', 'Fiona'];

// Use the sort function to sort the names alphabetically
const sortedNames = names.sort();

console.log(sortedNames);
Simple Example:

  // Function for a stupid simple explantion 

  function createLabel(name) {
    return `Person: ${name}`;
  }

  // Use the map function to apply the createLabel function to each element in the sortedNames array

  const explicitLabels = sortedNames.map(createLabel);

  console.log(explicitLabels);
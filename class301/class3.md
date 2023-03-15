# Passinf functions as props

## [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

1. What does .map() return?
      * it returns your array with the updated information.
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
      * Below, we loop through the numbers array using the JavaScript map() function. We return a <li> element for each item. Finally, we assign the resulting array of elements to listItems:
        const listItems = numbers.map((number) =>
        li{number}li);
      * Then, we can include the entire listItems array inside a ul element:
        ul{listItems}ul

3. Each list item needs a unique ____.
      * key
4. What is the purpose of a key?
      * to be able to identify one item in the list from the next. They help react identify which items have changed added or removed. 

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

1. What is the spread operator?
      * the use of three ...
2. List 4 things that the spread operator can do.
      * when trying to find the largest number in an array ... allows math.max to split the array into seperate arguments. Math.max([1,2,3])
      * Copying an array
      * Concatenating or combining arrays
      * Using Math functions
      * Using an array as arguments
      * Adding an item to a list
      * Adding to state in React
      * Combining objects
      * Converting NodeList to an array
3. Give an example of using the spread operator to combine two arrays.

      * let hi = ['hello','welcome','hey']
      * let bye = ['goodbye', 'see you later',]
      * let hiBye = {...hi...bye}


4. Give an example of using the spread operator to add a new item to an array.

      * let hi = ['hello','welcome','hey']
      * let moreHi = [...hi]
      * hi[0]= 'hey there'
      * console.log(...[...hi,'...',...moreHi]) // 'hey there','welcome','hey'


5. Give an example of using the spread operator to combine two objects into one.

## [How to pass Functions between components](https://www.youtube.com/watch?v=c05OL7XbwXU)

1. In the video, what is the first step that the developer does to pass functions between components?
      * creating a function wherever the state is that you need to change
2. In your own words, what does the increment function do?
      * it loops throguh the objects to change/update the state of the object based on the name that is passed in. you then need to return this information so that the update will be saved.
3. How can you pass a method from a parent component into a child component?
      * you would go to the 'person object' and type 'this.props.increment(this.props.name)'
4. How does the child component invoke a method that was passed to it from a parent component?
      *

## Bookmark and Review

[React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)
[React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

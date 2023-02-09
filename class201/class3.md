# Class 3 Reading Assignment

## HTML

1. when should you use an unordered list in your HTML document?
      * when you need a bulleted list
2. how do you change the bullet style?
    * using the 'list-style-type'
    * list-style-type: disc;
    * list-style-type: circle;
    * list-style-type: square;
    * list-style-type: georgian; etc.
3. when should you use an ordered list in your HTML document?
      * when you want a numbered list of text.
4. Describe two ways you can change the numbers on list items provided by an ordered list.
      1. a for lowercase letters
      2. A for uppercase letters
      3. i for lower case roman numerals
      4. I for uppercase Roman numerals
      5. 1 for numbers (default)


## CSS

1. Descibe CSS properties of margin and padding as characters in a story what are their rols in a story titled the box model?
      * Point of view we are in a tank and the nav contorls are alive and talking. This is your margin, they determine where on the page you are located. The aromor is also talking, this is your padding. it determines how much space is between its contents and the outside objects. The tank is the box model.
2. list and descrbe the four parts of an html elemtns box reffered to by the box model.
      * Padding, extends the content area to include its padding
      * border extends its padding to include its border
      * margin extends the border area to empty areas that used to seperate itself from its neighbors
      * content contains the actual content such as a paragraph or text.

## JavaScript

1. list five shorthand operators for the assignemnt in javascript and describe what they do.
      1. Remainder assignment	x %= f()
            * 31/10 = 1, there is a divison portion but the valuse saved is the remainder.
      2. Exponentiation assignmentx **= f()
            * operator raises the value of a variable to the power of the right operand.
      3. Bitwise XOR assignment	x ^= f()
            * operator uses the binary representation of both operands, does a bitwise XOR operation on them and assigns the result to the variable.
      4. Left shift assignmentx <<= f()
            * operator moves the specified amount of bits to the left and assigns the result to the variable.
      5. Nullish coalescing assignmentx ??= f()
            * operator, also known as the logical nullish assignment operator, only assigns if x is nullish (null or undefined).
2. is the people array a valid javascript array? if so how can I access the values if stored? if not why?
      *yes it is valid, and you would access the sub array by people[1][0] would give you Smiths info
3. the result to (10+'dog') + false would equal NAN becuase it is not a number
4. Describe a real world example of when a conditional statement should be used in a JavaScript program.
      * when looking for a true false scenerio. say if adding up a score to a game. or if you die in a game you could use an if else statment.
5. give an example of when a loop is useful in Javascript
      * a loop could be useful when enofcing a password. To make sure a user cannot gain access without typing in the correct input
6. what data types can be stored in an array?
      *  numbers, strings, boolean values (true and false), characters,and objects

## Arrays

- Data type -- Data structure **special type of object**
- a collection of elements
- can be mixed - can store numbers, strings, other arrays all in the same array structure 
- Don't need to determine size of array
- every element in the array has a position - referred to as its inedx
- array are zero based index

let myArray =[
    'hello',
    '1',
    'true',
    'goodbye'
];

-Array also have built in methods
- .push() - add an element to the end of the array
- .pop() - remove the last element in an array

- Array properties
  - .length - 

  let nums = [ 2,3,4,5,6];
  console.table(nums); - puts array into a table that shows index position for its values

  ## [CSS Box Model](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model)

Everything is in a box. Boxes can be inline or block. The display property can be used to set values for the box.

An Outer display can be be block or inline. The block starts on a new line and width and height are respected. There is padding and margins that adjust the box. If there is no specified width, then the box becomes as wide as the container. With Inline, the same width and height do not apply and the box stays on the same line. The vertical padding, borders, and margins do not move the other box but can be adjusted vertically.

The Inner display box determines how element inside are laid out. display: flex is a way to change the inside of the box to flex items.

The box model defines how the margin, border, padding, and content within a box works together.

Parts of a Box:

Content Box what shows on the webpage. Uses inline-size, block-size, width, and height properties

Padding Box surrounds the content as white space. Uses padding property

Border Box wraps around the padding and content box. Uses border property

Margin Box wraps the border, padding, and content as whitespace between the box. Uses margin property

An alternative box model uses any width as the width of the visible box. It is activated with box-sizing: border-box; and it needs to be set within the <html> in the CSS file

DevTools can be used to view the box model.

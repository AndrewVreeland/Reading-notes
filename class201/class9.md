# Class 9 Reading Assignment

## *These are my notes from Module 9*

## HTML FORMS

[Your First Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)
[How To Structure A Web Form.]( https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form)

1. Why are forms so important in web development?
      * forms are important because it allows the websites users to interact with the page by entering in important information for whatever the task at hand is. this is then passed on to a database where it can be stored until needed for future use.
2. When designing a form, what are some key things to keep in mind when it comes to user experience?
      * if your form is too large then you risk losing users through frustration.
3. List 5 form elements and explain their importance.
      * <form>, this is a container element like <header> the form element has some specific attributes to change how the form behaves.
      * <label> this is the label for the input portion of a form. It will specify if it is a username or a password for instance
      * <input> this creates an area for a user to input some sort of value, depending on the attrivute.
      * <textarea> this has to have a closing tag where an input tag does not. That changes the way that you define the default values.
      * <button> this button will submit your form to the data base. this excepts three attributes being type, reset, or button.


## Java Script

[Introduction To Events.](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

1. How would you describe events to a non-technical friend?
      * an event is something that happens that your code will then respond to using an event listener. an event could be a mouse click or when you hover over a link and it changes colors.
2. When using the addEventListener() method, what 2 arguments will you need to provide?
      * the name of the event that we want to register the handler for and the code that comprises the handler function
3. Describe the event object. Why is the target within the event object useful?
      * this is passed to event handlers to provide extra features and information.
4. What is the difference between event bubbling and event capturing?
      * event bubbling is when elements within your container will notify their parent that an event has happened. this happens in forms when you type something in or when you press the button. it will notify the event listener at the form level. event capturing is the complete opposite where the listener would be at the form level and it would propogate downwards towards the child elements.
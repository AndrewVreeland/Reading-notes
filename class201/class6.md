# Class 6 Reading Assignment

## *These are my notes from Module 6*

## Reading

[JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

1.How would you describe an object to a non-technical friend you grew up with?
      *An object is a collection of similar data. like someone puting their name and birthday down in an application, it will be saved as an object.
2.What are some advantages to creating object literals?
      * shorter syntax, easier to type and to read.
3.How do objects differ from arrays?
      *arrays use index numbers to access information where as objects use the name associated with the data
4.Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation
      * if an objects property name is held in a variable then you have to use bracket notation.
5.Evaluate the code below. What does the term this refer to and what is the advantage to using this?
      * This is equivelent to Spot in this instance. Becuase it refers to the object that the code is written inside of. The benefit of using 'This' is that you are able to use the same method definition for mutiple objects.

## Intro to DOM

[DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)
1.What is the DOM?
      *The Document Object Model is a programming interface for web documents. It represents the oage so that programs can have access to and change the document structure style and content. It allows progamming languages to interract with the page.
2.Briefly describe the relationship between the DOM and JavaScript.
      * Dom can be accessed by any language. Without the DOM there would be no way for the Javascript to actually interact with the websites domain to change anything.

## Fundemental Data tpyes

1. Document When a member returns an object of type document (e.g., the ownerDocument property of an element returns the document to which it belongs), this object is the root document object itself. The DOM document Reference chapter describes the document object.
2. Node Every object located within a document is a node of some kind. In an HTML document, an object can be an element node but also a text node or attribute node.
3. Element The element type is based on node. It refers to an element or a node of type element returned by a member of the DOM API. Rather than saying, for example, that the document.createElement() method returns an object reference to a node, we just say that this method returns the element that has just been created in the DOM. element objects implement the DOM Element interface and also the more basic Node interface, both of which are included together in this reference. In an HTML document, elements are further enhanced by the HTML DOM API's HTMLElement interface as well as other interfaces describing capabilities of specific kinds of elements (for instance, HTMLTableElement for <table> elements).
4. NodeList A nodeList is an array of elements, like the kind that is returned by the method document.querySelectorAll(). Items in a nodeList are accessed by index in either of two ways:

* list.item(1)
* list[1]
* These two are equivalent. In the first, item() is the single method on the nodeList object. The latter uses the typical array syntax to fetch the second item in the list.

5. Attr When an attribute is returned by a member (e.g., by the createAttribute() method), it is an object reference that exposes a special (albeit small) interface for attributes. Attributes are nodes in the DOM just like elements are, though you may rarely use them as such.
6. NamedNodeMap A namedNodeMap is like an array, but the items are accessed by name or index, though this latter case is merely a convenience for enumeration, as they are in no particular order in the list. A namedNodeMap has an item() method for this purpose, and you can also add and remove items from a namedNodeMap.

## Common APIs

* document.querySelector(selector)
* document.querySelectorAll(name)
* document.createElement(name)
* parentNode.appendChild(node)
* element.innerHTML
* element.style.left
* element.setAttribute()
* element.getAttribute()
* element.addEventListener()
* window.content
* Window.onload
* window.scrollTo()
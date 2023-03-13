
# React

## What is React?

* A user interace library, it is an agnostic library. used to create entire websites or apps, also could be used as a widget and only contain small parts of the website or app.

* React is a library, it comes with a handful of functions and suggestions on how to organize some things. React is lightweight and must be used with other libraries.

## What is a component?

* Aa component is created by functions or classes. and then are imported for ex. ' import Header from " ./Header';
* can be reused if components are built properly in a small format

## What is the dataflow of React?

* you can call upon components within the functionailty of other components. for instance the <app/> could contain the <Header/> which contains <SiteInfo/> and <MainNav/> this would look like a data tree.

* Data flows down in one direction so if you were to call upon and recieve data at the <app/> level then the other components would have access to that data but if you called up that data in the <SiteInfo/> then Header and app would not have access .

* you can have lower branches of the data tree can trigger app to go and retreive new data and pass it back down.

## How do we make a React element a DOM element?

* react becomes dom when you pass the information through react dom.

## React is a User Interface ______

      * User Interface agnostic library

## Which direction does data flow in React?

      * down from its compnent into its children

## Every component manages its own ____

      * has its ability to manage its own state (data) and pass it down to its children.

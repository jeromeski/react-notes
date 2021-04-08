##### Why does this thing exists?
• The whole idea of react is youre able to manage the complexity of your app
  by breaking it down to separate components that you could then compose together.
##### What problems does this thing solve?

React.createClass API - before React doesn't have a class system.

May 29, 2013
      ├─  React v.0.30
      │    └─ introduction of state, props, components 
      │   "React.createClass API - before React doesn't have a class system."     
January 17, 2015
      ├─  ES6 was released
      │    ├─  Class Declarations are now integrated to JS
January 27, 2015
      ├─  React v.0.13.0 Beta 1
      │    ├─  React.createClass API is deprecated
      │    ├─  Native JS classes can be now used in React (Ecmascript Standard)
      │   TRADE-OFFS
      │    ├─  Initialize state inside the constructor method as a state property 
      │    │   on the instance. 
      │    ├─  Ecmascript enforces to invoke super() before you can use "this"
      │    ├─  You have to pass props to the constructor and super
      │    ├─  No Autobinding
      │    │     ├─ this.updateRepos = this.updateRepos.bind(this)
      │    │     └─ React-uncaught TypeError: Cannot read property 'setState' of undefined
      │   CLASS FIELDS
      │    ├─ no longer use constructor, super, and .bind inside constructor
      │   DUPLICATE LOGIC ISSUES
      │    │
      │   SHARING NON-VISUAL LOGIC PROBLEM
February 11, 2015
      ├─ Introduction of HOC
      ├─ Introduction of Render-Props
      ├─ ISSUES -> Wrapper Hell

React Hooks
- Simple
- Composable
- Flexible
- Extendable

What is reactjs?
- is a Javascript library.
- created by Facebook
- ultimate purpose is to show content (HTML) to users and handle user interaction.

- React can work by itself without adding any libraries.
- But can also work with so many libraries, packages, servers and database.


Extremely Efficient 
� creates it's own virtual DOM where it
� Calculates changes in the Virtual DOM, thus avoiding expensive DOM operations and makes updates in a very cliently manner.
Makes writing JS easier
� You can just write HTML in the render function without concactinating strings.
� Its easy to code test cases because, react is entirely written in JS.
   







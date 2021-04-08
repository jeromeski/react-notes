WHAT IS A LIFECYCLE METHOD?

in its simplest meaning...

Lifecycle?
  ├─ A component is created
  ├─ Shows up on the DOM/ Browser and rendered
  ├─ Call setState/ or change in props, then component is rerendered.
  └─ Component get's removed from the DOM, then content stops showing

2 PHASES 
• Render phase
• Commit phase

REACT COMPONENT LIFECYCLE
      │
      ├─  constructor()
      │   ├─ optional - you have the option to define it or not
      │   └─ called when a new instance of our component is created
      ├─  componentWillMount
      │   ├─ fires after constructor is called. 
      │   ├─ Has access to the Native-DOM but no access to children.
      │   └─ depracated
      ├─  render()
      │   ├─ not optional
      │   └─ lifecycle method function that has to be defined/ mandatory
T     │
      │    "Content visible on screen"
      │
I     ├─  componentDidMount
      │   ├─ called 1 time, when component is "first" gets rendered on the screen
      │   └─ suitable for use with initial data loading
M     │
      │    "Sit and wait for updates...
      │
E     ├─  componentDidUpdate
      │   ├─ optional
      │   ├─ before it gets called render() is invoked first.
      │   ├─ called automatically when component updates itself
      │   └─ component get's rerendered
      │
      │   "Sit and wait until this component is not longer shown"
      │
      ├─  componentWillUnmount
      │   ├─ optional
      │   └─ used to do some sort of clean up


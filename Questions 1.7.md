What is Unidirectional Data Flow?
In react data is passed normally from parent to child via props.
and from child to parent, bottom to top via props.method
effect:
Disadvantage is this method is quite inefficient if you use this pattern if target child is multiple levels deep.

What is the diference between props vs state.
state
- only usable with class components
* technically can be used with functional components
using react hooks.
- js object that contains data relevant to a component.
- when a component defines data locally within itself
- can only change by using setState function

props
- can be used with either class or functional components.
- props is an attribute whose data is passed down from parent to child component.
- you need to go up to the parent and ask the parent to change value for props to change. 

What is lifting state up?
When components with the same props uses the same state.
If multiple components shares the same state as props. Group them together inside the component that has the state of the props that they share.

Controlled Component vs Uncontrolled Component
Controlled component are components that has state binded to the component.
Uncontrolled components is not bound to any bit of state or onChange.

What are refs?
- Normally react developers are not interacting with the actual DOM but are more likely developing against the virtual DOM.
- using this bypasses the virtual DOM, getting actual access to the actual DOM.
code:
let inputRef = useRef(null)
every single ref you create with the useRef hook has a .current property
that actually stores the value.

What are keys?
- are used to uniquely identify each item in a component.
Why important?
- When react tries to make changes in the actual DOM it tries to make it in a way that is efficient as much as possible.
- Reconciliation Algorithm comes in to play.
- React compares the current tree to the new tree and make computations based on the new changes, then tries to commit the new tree into the actual DOM in the most efficient way as possible.

Main take away:
- avoid expensive DOM operations by using keys.

Props vs Context
- Props only goes one component down to the next component.
- Props is passed down one level at a time.
- Prop drilling
So if you want to pass data from Parent to a grandchild you have to follow the chain passing props to the child and finally passing it down to its grandchild.
- Context however is different, you can pass data from Parent to Grandchild bypassing the component/s in the middle. Thus solving the prop drilling problem.
- is a mechanism that allows you to pass data from one component down to as many components deep on the same tree.
DRY - Allows a way to share logic to the entire app, without having to rewrite logic over and over again.

What is a Higher Order Component?
- is a function that receives a component as an argument, that returns a new component with extra functionality.

What is Render Props?
- A technique in React that allows components to share data using a prop whose value is a function.
- The component that will be rendered, takes in a render prop.
- The prop value contains a function that render JSX.

What are Hooks?
- Allows Functional Components to some sort of "Hook in" to React Lifecycle Methods, without using a classbased component and defining the Lifecycle method.


HOC & Render Props has Wrapper Hell
Wrapper hell solution?
Custom hooks - allows us to share logic to multiple components.

UseEffect Hook
- can act as componentDidMount by passing a dependency [] as a second argument.
- can act as componentDidUpdate, by passing a dependency [] with the dep inside 
- can act as componentWillUnmount by returning a fn.

React.Memo <- hook
- allows us to make the component only render if its props that is accepting is changing. (shouldComponentUpdate)
- helps out in performance

UseCallback <-- hook
- helps out in performance

UseMemo
- memoize values

 Virtual DOM, and Reconciliation, data fetching patterns, and testing react apps
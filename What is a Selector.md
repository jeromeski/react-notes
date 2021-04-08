Selector
    ├─  Obj returned in mapStateToProps.
    └─  Gets the state, then gets the slice of that state.

Default behavior:
- Whenever a reducer is updated, new object is returned.

Reducer
    └─  whenever its updated?
          ├─  Redux recomposes a new state object.
          ├─  mapStateToProps gets called every single time there is an update.
          ├─  mapStateToProps passes in the new state, 
          │   triggering a rerender to the components that receives new props. 
          │   (Expensive and unnecessary DOM operations occurs)
          └─  Solution: Some function to check if sliced state previous value is equal to new value.
              Then decide to pass in new props or not.
              Memoization → npm package: Reselect → caching of the selectors value

Main take aways: 
1. Component rerenders everytime it receives new props or state.
2. We can avoid this by applying memoization in the selector.
What are side effects?
  - Typically defined as secondary effect.
  - Anything that interacts with the outside world.
  - state change that can be observed outside of its local evironment.
  - outside of the local function that is being executed.
common ex.
Mutating non-local variables.
Making network requests.
Updating the DOM.

UseEffect rules:
function is called everytime the component is rendered.
fires everytime render() gets called.
fires everytime the component mounts for the first time.


Dependencies Array ,[]
- any dep(s) inside the array will not trigger a rerender if state or props of that dep(s) is not changed.
REACT COMPONENT LIFECYCLE
      │
      ├─  constructor()
      │   └─ Good place to do one-time setup or initial data loading
      ├─  render()
      │   └─ Avoid doing anything besides returning JSX
T     │
      │    "Content visible on screen"
      │
I     ├─  componentDidMount
      │   ├─ "Best" place to do one-time setup or initial data loading
      │   └─ consistently use this for data loading for clean code.
M     │
      │    "Sit and wait for updates...
      │
E     ├─  componentDidUpdate
      │   ├─ Good place to do more data-loading after initial data is loaded
      │   └─ Updates in state/props
      │
      │   "Sit and wait until this component is not longer shown"
      │
      ├─  componentWillUnmount
      │   └─ Good place to do cleanup (especially non-react stuff)
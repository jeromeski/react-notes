*useEffect gets called everytime a component renders

Fn Component is created
    ↓
State gets initialized
    ↓
UseEffect gets ignored in the initial render
    ↓
React updates DOM
    ↓
Browser paints screen
    ↓
UseEffect fires
    ↓
Api call gets invoked
    ↓
setState gets called (triggers a rerender)
    ↓
content gets updated w/ state values
    ↓
rerendering causes useEffect to be called again
    ↓
Api call gets invoked
    ↓
setState gets called 
    ↓
   LOOP

      
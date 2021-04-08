React Patterns

1. Higher Order Components Pattern
    • A fn that takes a component and returns a new component.
    • ex. withRouter(Component)
2. Container Component Pattern
  COMPONENT                               CONTAINER
    ├─ Contains HTML & Styling              ├─ Doesn't contain HTML Elements.
    ├─ Responsible for viewing data         ├─ Responsisble for preparing data.
    ├─ Stateless, unless 'styling related'  ├─ Stateful for storing data.
    ├─ Do not communicate w/ external src   ├─ Communicate w/ external sources.
    └─ Usually a fn component               └─ Can be functional or class component
3. Render Props Pattern
    • technique for sharing code between React Components 
      using a prop whose value is a function.
    • useful if children have duplicate code.
    • Uses a Wrapper component

App.js                  Wrapper                       Component1        Component2
wires up Wrapper        contains the shared state
(shows Wrapper)         contains the shared logic

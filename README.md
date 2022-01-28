# React-Redux

**Redux is a predictable state container for javascript apps** <br />
Redux helps to modify the state of an application in a predictable way.

## Three Core Concepts

- **Store** : _Holds the state of the application_
- **Action** : _Describes what happened_
- **Reducer** : _Ties the store and actions together_

## Three Principles

- ***The state of the entire application is stored in an object tree within a single store***
- ***The only way to change the state is to emit an action, an object describing what happened***
  ```
  {
      type: INCREMENT_COUNTER
  }
  ```
- ***To specify how the state tree is transformed by actions,  you write pure reducers*** <br />
It takes previous state and action as an input and returns a new state without updating the previous state as it is a pure reducer.

## Redux Store Responsibilities
- Holds application state
- Allows access to state via **`getState()`**
- Allows state to be updated via **`dispatch(action)`**
- Registers listeners via **`subscribe(listener)`**
- Handles unregistering of listeners via the function returned by **`subscribe(listener)`**

## Middleware
It is the suggested way to extend redux with custom functionality.
It provides a third-party extension point between dispatching an action, and the moment it reaches the reducer.
use middleware for logging, crash reporting, performing asynchronous tasks etc.


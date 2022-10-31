## 4.2 Basic Redux

**Goal**: use Redux to manage application state and understand the difference between container and presentational components.

**Required Reading**:

- [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
- [Container vs Presentational Components in React](https://medium.com/@yassimortensen/container-vs-presentational-components-in-react-8eea956e1cea)
- [Redux: Getting Started](https://redux.js.org/introduction/getting-started)
- [Redux: Basic Tutorial](https://redux.js.org/basics/basic-tutorial)

**Online Shop**:

> Add a new "Edit" button on the detail page. Pressing it should open a new view, it shouldupdate the properties of the product. The view should have two buttons: "Cancel" (which undos all the changes) and "Save" (which calls the backend to persist the changes).
>
> Add some validation to your form (ex: check that the fields are not empty, that the price and weight inputs contain only numbers, etc.)
>
> Also create a new "Add" button on the product list. Pressing this button should open a view for creating a new product (which the same structure and buttons as the edit view).
>
> Store all application state in a Redux store.
>
> Hints:
>
> - Create a reducer for each page,
> - Add actions for each user input handler, data load event, etc. For each API call, you should create three actions: one which is dispatched when you do the fetch call, one which is dispatched if the fetch call succeeds and one if it fails. Example: `READ_PRODUCTS`, `READ_PRODUCTS_SUCCESS`, `READ_PRODUCTS_ERROR`.
> - Dispatch the actions and select the state **only** inside the container components.
> - Make sure to also have a loading flag indicator in each page's state,
> - Install the [Redux DevTools](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en) Chrome plugin to be able to debug your store.

_Further Resources_:

- [Understanding Redux + React in Easiest Way](https://medium.com/tkssharma/understanding-redux-react-in-easiest-way-part-1-81f3209fc0e5)
- [A beginner’s guide to Redux with React](https://medium.com/@bretcameron/a-beginners-guide-to-redux-with-react-50309ae09a14)

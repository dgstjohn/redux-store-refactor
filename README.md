# Refactoring Shop-Shop Exercise for Redux

## Description

The objective in this repo is to take an e-commerce application that uses the React Context API to manage global state and refactor it to instead use Redux to manage state. For this, I replace the existing client-side GlobalState.js file with a Redux store in store.js, which simply imports Redux's createStore method and the reducers.js file and makes it available for export. The actions.js file remains identical to the original. Most of the action for refacotring takes place in the reducers.js file, which is rewritten slightly to establish an initialState variable object and a simplified export statement, and in several components and pages where the useStoreContext function established in GlobalState.js is replaced with the useSelector and useDispatch methods from Redux. Import statements for those files are also adjusted accordingly. The deployed application functions identically to its React Context API version.

## Link to Deployed Application
[https://frozen-eyrie-15727.herokuapp.com/](https://frozen-eyrie-15727.herokuapp.com/)
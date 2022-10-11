# .msg Career Path: React Training

## Contents

 - [Working Mode](#working-mode)
 - [Environment](#environment)
 - [Online Shop](#online-shop)
 - Chapter 1
    - [1. HTML and CSS Basics](#1-html-css-and-git-basics)
    - [2. TypeScript](#2-typescript)
    - [3. React Intro](#3-react-intro)
 - Chapter 2
    - [4. Components](#4-components)
    - [5. Hooks](#5-hooks)
 - Chapter 3
    - [6. MaterialUI and JSS](#6-materialui-and-jss)
    - [7. Routing](#7-routing)
 - Chapter 4
    - [8. Axios](#8-axios)
 - Chapter 5
    - [9. Basic Redux](#9-basic-redux)
 - Extra
    - [10. Redux Saga](#10-redux-saga)
    - [11. Recompose](#11-recompose)
    - [12. Highcharts](#12-highcharts)

## Working Mode

The road-map consists of several steps. In each step, a set of theoretical concepts are explored, supported by reference documentation, book chapters, tutorials and videos. In parallel, a simple application will be built with the learned concepts: the **Online Shop** application.

After the learning material for a given step was sufficiently explored, either some new functionality will be added to this application or old functionality will be refactored.

All the code written must be published on GitHub. Commits must be pushed when each individual chapter is finished. In order to request a code review from the trainers, you must [open a pull request](https://help.github.com/en/articles/creating-a-pull-request) from the `develop` to the `master` branch.

## Environment

You can work using your local environment:
 - You need to install [NodeJS](https://nodejs.org/en/) and [VSCode](https://code.visualstudio.com/download).

**If you have finished the Spring Boot training** you can use that backend application together with the frontend one you will develop during this training. If not, in the `backend` folder you can find a server-side implementation for the online shop. To run this server perform the following:
 - Open the `backend` folder in your terminal
 - `npm ci` (only needed the first time your run the server)
 - `npm start`
 - Open [http://localhost:4000](http://localhost:4000) in your browser.

## Online Shop
The application will simply **browse through a catalog of products**. It will support:

 - Listing the products,
 - Adding a new product,
 - Updating an existing product,
 - Deleting a product.
 
The online shop has a **shopping cart** functionality:
 - The user may add items into the cart,
 - He may increment and decrement the quantity of each product or even remove a product completely from the cart,
 - Lastly, he may checkout the cart and place an order (resulting in the creation of an order in the backend).

**Mockups** describing the user interface structure can be found in the [mockups](./mockups/mockups.pdf) folder.
These **mockups should be used as a guideline**, but improvements or deviations from them is allowed.
**We support custom styling** in order to make the application your own.

# Chapter 1
## 1. HTML, CSS and GIT Basics

**Goal**: refresh your knowledge about HTML and CSS basic concepts.

**Required Reading:**

 - [HTML Beginner Guide](https://www.htmldog.com/guides/html/beginner/)
 - [CSS Beginner Guide](https://www.htmldog.com/guides/css/beginner/)
 - [CSS Media Queries](https://www.htmldog.com/guides/css/advanced/mediaqueries/)
 - [Git Basics](https://git-scm.com/book/en/v1/Getting-Started-Git-Basics)

**Online Shop**: *nothing to do*.

*Further Resources*:

 - [HTML and CSS Reference](https://www.htmldog.com/references/)
 - [W3's Intro Tutorial](https://www.w3.org/Style/Examples/011/firstcss.en.html)
 - [GitHub - Hello World](https://guides.github.com/activities/hello-world/)

## 2. TypeScript

**Goal**: learn a bit of TypeScript.

**Required Reading**:

 - [TypeScript in 5 minutes](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)
 - [What is TypeScript and why would I use it in place of JavaScript?](https://stackoverflow.com/questions/12694530/what-is-typescript-and-why-would-i-use-it-in-place-of-javascript) *(read the top two answers)*
 
**Online Shop**: *nothing to do*.

*Further Resources*:

 - [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/basic-types.html)
 - [Why TypeScript is the best way to write Front-end in 2019](https://medium.com/@jtomaszewski/why-typescript-is-the-best-way-to-write-front-end-in-2019-feb855f9b164)

## 3. React Intro

**Goal**: become familiar with React.

**Required Reading**:

 - [Single vs Multiple Page Applications](https://medium.com/@NeotericEU/single-page-application-vs-multiple-page-application-2591588efe58)
 - [Create a New React App](https://reactjs.org/docs/create-a-new-react-app.html)
 - [React: Hello World](https://reactjs.org/docs/hello-world.html)

**Online Shop**:

 > Install *Create React App* with the help of the NodeJS package manager: `npm install -g create-react-app`.
 > 
 > Create a new project in the root of your git repository by using the CLI: `create-react-app online-shop --template typescript`.
 > 
 > Navigate inside the project folder, start the project and open its home page in your browser: `npm start`.
 >
 > Install the [React Dev Tools](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en) extension for Chrome. Inspect the application and view the components using this extension.

*Further Resources*:

 - [Tutorial: Intro to React](https://reactjs.org/tutorial/tutorial.html)
 - [How to see your React state and props in the browser](https://www.freecodecamp.org/news/how-to-see-your-react-state-props-in-the-browser-774098a50fcc/)

# Chapter 2
## 4. Components

**Goal**: get a grip on the basics of React Components.

**Required Reading**:

- [Introduction to JSX](https://reactjs.org/docs/introducing-jsx.html) (similar to TSX which we will use)
- [Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
- [Components and Props](https://reactjs.org/docs/components-and-props.html)
- [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)
- [Styling and CSS](https://reactjs.org/docs/faq-styling.html#how-do-i-add-css-classes-to-components)
- [Functional Components vs Class Components](https://www.twilio.com/blog/react-choose-functional-components)

**Online Shop**:

 > For the moment, we will use mock data across all components. The data will be defined locally in the component's file.
 >
 > Create a new React Component for displaying a single product's details.
 >
 > Create an React component for displaying a list of products. Hint: use the `.map` call on the array of products.
 >
 > Add some CSS to each of the components to make them look nicer.
 
 *Further Resources*:
 
 - [The `.map` function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
 - [Why do I need Keys in React Lists?](https://medium.com/@adhithiravi/why-do-i-need-keys-in-react-lists-dbb522188bbb)
 - [React Virtual DOM Explained](https://programmingwithmosh.com/react/react-virtual-dom-explained/)
 
## 5. Hooks
 
**Goal**: get used to working with Hooks. Focus on `useEffect` and `useState`.

**Required Reading**:

- [Introducing Hooks](https://reactjs.org/docs/hooks-overview.html)

**Online Shop**:

 > Migrate your React component(s) from before from using class-based components to using hooks inside functional components. 
 
*Further Resources*:
 
 - [Getting Started With The React Hooks API](https://www.smashingmagazine.com/2020/04/react-hooks-api-guide/)
 
 # Chapter 3
 ## 6. MaterialUI and JSS
 
 **Goal**: understand what MaterialUI helps us with and how to style components using JSS.
 
 **Required Reading**:

- [MaterialUI installation](https://material-ui.com/getting-started/installation/)
- [MaterialUI learning information](https://material-ui.com/getting-started/learn/)
- [MaterialUI theme](https://material-ui.com/customization/theming/)
- [React JSS](https://cssinjs.org/react-jss/?v=v10.6.0)

**Online Shop**:

 > Install the MaterialUI library. Use the built-in CSS classes to style your existing components.
 >
 > Create a custom MaterialUI theme where you must add those fields (and more if you want):
 > - Primary color: whatever color you want (e.g. #a01441)
 > - Font: Any Google Font (e.g. [Open Sans](https://fonts.google.com/specimen/Open+Sans))
 > 
 > Create JSS styling files for your existing components which also inject the MaterialUI theme.
 > In those files write custom classes using the propertues from the theme and use them on your UI components.
 
 *Further Resources*:
 
 - [Styled Components](https://mui.com/system/styled/)
 
 ## 7. Routing
 
 **Goal**: understand the basics of React Router and add routing to your project
 
 **Required Reading**:

 - [React Router: Quick Start](https://reacttraining.com/react-router/web/guides/quick-start)
 - [React Router: Components](https://reacttraining.com/react-router/web/guides/basic-components)
 - [A Simple React Router Tutorial](https://blog.pshrmn.com/simple-react-router-v4-tutorial/)
 - [React: Handling Events](https://reactjs.org/docs/handling-events.html)
 
 **Online Shop**:
 
 > Add a button next to each product from the product list. You can use it to navigate to a specific product's detail page.
 >
 > From the detail page of the product, the user may add it to his shopping cart (by pressing a button).
 >
 > Add Routing to your project and implement a navigation between the list of all products and the product detail page.
 > 
 > Add a navigation which redirects users from the default path ('/') to the '/products' page and displays by default the list of all products.
 >
 > Enhance your app with routing parameters, such that you can navigate to a specific product's detail page.
 
 *Further Resources*:
 
  - [React Router: Redirects](https://reacttraining.com/react-router/web/example/auth-workflow)
 
 # Chapter 4
 ## 8. Axios
 
 **Goal**: communicate with your backend application using Axios.
 
 **Required Reading**:
 
  - [React: State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
  - [Axios Docs](https://www.npmjs.com/package/axios)
  - [Axios with Typescript](https://bobbyhadz.com/blog/typescript-http-request-axios)
  - [How to fetch data in React with Axios](https://www.robinwieruch.de/react-fetching-data)
 
**Online Shop**:

 > Use Axios to read the products from the backend to fill in the product list. 
 > 
 > When navigating to the product detail page, read the product information from the backend.
 >
 > Add a new "Delete" button on the detail page, which calls the backend to remove a product from the catalogue.
 >
 > Add a new "Checkout" button on the shopping cart page, which creates a new order on the backend.
  
 # Chapter 5
 ## 9. Basic Redux
 
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
 >  - Create a reducer for each page,
 >  - Add actions for each user input handler, data load event, etc. For each API call, you should create three actions: one which is dispatched when you do the fetch call, one which is dispatched if the fetch call succeeds and one if it fails. Example: `READ_PRODUCTS`, `READ_PRODUCTS_SUCCESS`, `READ_PRODUCTS_ERROR`.
 >  - Dispatch the actions and select the state **only** inside the container components.
 >  - Make sure to also have a loading flag indicator in each page's state,
 >  - Install the [Redux DevTools](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en) Chrome plugin to be able to debug your store.
 
 *Further Resources*:
 
  - [Understanding Redux + React in Easiest Way](https://medium.com/tkssharma/understanding-redux-react-in-easiest-way-part-1-81f3209fc0e5)
  - [A beginner’s guide to Redux with React](https://medium.com/@bretcameron/a-beginners-guide-to-redux-with-react-50309ae09a14)
 
# Extra
## 10. Redux Saga

**Goal: trigger the Axios calls using actions**

**Required Reading**:
 
  - [Redux Saga: Getting Started](https://redux-saga.js.org/)
  - [Redux Saga: Beginner Tutorial](https://redux-saga.js.org/docs/introduction/BeginnerTutorial.html)
  - [A Newb's guide to Redux Saga](https://medium.com/@adlusk/a-newbs-guide-to-redux-saga-e597d8e6c486)
  
**Online Shop**:
 
  > Move all the Axios calls into dedicated Sagas. 
  
*Further Resources*:
 
  - [Handle side-effects with Redux-Saga](https://scalac.io/redux-saga-handle-side-effects-2/)

## 11. Recompose

Goal: understand the concept of Higher Order Components (HOC)

Required Reading:

 - [Using Recompose to write clean higher-order components](https://blog.logrocket.com/using-recompose-to-write-clean-higher-order-components-3019a6daf44c/)
 - [Building HOCs with Recompose](https://medium.com/front-end-developers/building-hocs-with-recompose-7debb951d101)
 - [Recompose Recipes](https://github.com/acdlite/recompose/wiki/Recipes)
 
 Online Shop:
 
  > Transform all your container components to recomposed components (created by just applying a series of HOCs on the presentational component).
  > Create a HOC for displaying a loading indicator if the loading property is set to `true`. Use this HOC throughout the application.
  
 ## 12. Highcharts
 
 Goal: become familiar with Highcharts basics and usage within React
 
 Required Reading:
  - [Chart Concepts](https://www.highcharts.com/docs/chart-concepts/understanding-highcharts) *whole chapter*
  - [React Wrapper](https://www.highcharts.com/blog/tutorials/highcharts-react-wrapper/)
  
  Online Shop:
  
   > Create a new page for displaying total sales figures per product type. This data should be displayed in two different charts: a bar chart and a pie chart.
  
  Further Resources:
   - [API Reference](https://api.highcharts.com/highcharts/)
   - [Using Pie Charts](https://stackoverflow.com/questions/54806064/using-piechart-from-highcharts-react-official)

# Marvel Heroes Atomic Design

## Getting Started

### Requirements

For development, you will only need Node.js installed on your environement.

### Node

[Node](http://nodejs.org/) is really easy to install & now include [NPM](https://npmjs.org/).
You should be able to run the following command after the installation procedure
below.

    $ node --version
    v8.11.1

    $ npm --version
    5.6.0

### Installation

`npm install`

### Run

`npm run start`

Then open [http://localhost:3042](http://localhost:3042). The start script is set to reload the app and keep the state just after a file is saved , no need for manual refresh.

### Build

`npm run build`

### Test

`npm run test`

[Jest](https://facebook.github.io/jest/docs/api.html) and [Enzyme](http://airbnb.io/enzyme/docs/api/) are the tools in place for unit testing the project code. Unit test files inside `src` must be named with `*.spec.js` or `*.test.js`.

### Folder structure and Suggested Workflow

This is the basic project folder structure

```javascript
...
  src
  └──src // designed to contain all the content of the application
    └──components // designed to contain all the components of the application
      └──atoms // designed to contain atoms components
      └──molecules // designed to contain molecules components
      └──organisms // designed to contain organisms components
      └──pages // designed to contain pages components
      └──templates // designed to contain templates components
  | App.js // designed to be the entry point of the application
  ...
...
```

Basically, the entry point of the `index.js` project renders the `App` component that renders the pages components according to the route.

---

## Languages & tools

### JavaScript

- [Webpack](https://webpack.js.org/) is used to aggregate JavaScript files for use in a browser.
- [Babel](https://babeljs.io/) is used as a JavaScript compiler and configurable transpiler.
- [ESLint](https://eslint.org/) is used to prevent JavaScript error.
- [React](http://facebook.github.io/react) is used for UI.
- [React Router](https://www.npmjs.com/package/react-router) is used to manipulate routes.
- [Redux](https://redux.js.org/) is used to manage application state.
- [Jest](https://jestjs.io/) + [Enzyme](https://github.com/airbnb/enzyme) - is used for unit tests.
- [CircleCI](https://circleci.com/) - is used for CI.

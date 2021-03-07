### Create new proyect

```r
npx create-react-app
```

### install react-redux

```r
npm install react-redux
yarn add react-redux
```

### install redux
```r
yarn add redux
npm install redux
```

### Configure redux in index
```r
import React from 'react'
import { render } from 'react-dom'
import { Provider } from 'react-redux'
import { createStore } from 'redux'
import rootReducer from './reducers'
import App from './components/App'

const store = createStore(rootReducer)

render(
  <Provider store={store}>
    <App />
  </Provider>,
  document.getElementById('root')
)
```

### install thunk
```r
npm install redux-thunk
```

### Apply middleware thunk
```r
import { applyMiddleware, createStore, compose } from "redux";
import reduxThunk from "redux-thunk";
import rootReducer from "../reducers";

const composeEnhancers = window.__REDUX_DEVTOOLS_EXTENSION_COMPOSE__ || compose;
const middleware = [reduxThunk];

export const store = createStore(
  rootReducer,
  composeEnhancers(applyMiddleware(...middleware))
);
```

### Install axios
```r
npm install axios
```

### Instal Router
```r
npm install --save react-router-dom
```

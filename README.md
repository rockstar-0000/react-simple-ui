## Getting started

This is simple UI-Router package is distributed using [npm](https://www.npmjs.com/), the node package manager.

```
yarn add @uirouter/react
```

Import `UIRouter` into your project, define some states and you're good to go!

```jsx
import React from 'react';
import ReactDOM from 'react-dom';
import { UIRouter, UIView, pushStateLocationPlugin } from '@uirouter/react';
import Home from './components/Home';

// define your states
const states = [
  {
    name: 'home',
    url: '/home',
    component: Home,
  },
];

// select your plugins
const plugins = [pushStateLocationPlugin];

ReactDOM.render(
  <UIRouter plugins={plugins} states={states}>
    <UIView />
  </UIRouter>,
  document.getElementById('root'),
);
```

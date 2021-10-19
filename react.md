# React Notes

- React creates a own virtual DOM in memory. That's mean first changes own DOM after that changes browser's DOM.

__React Directly in HTML__

- Use react directly inside in html. React can be used by putting the following codes in the header.

```html
    <script src="https://unpkg.com/react@17/umd/react.development.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom@17/umd/react-dom.development.js" crossorigin></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
```

__Setting up a React Environment__

- If you can use npx and Node.js, you can create React application. Run this command to create a React app named my-react-app. 

```html
  npx create-react-app my-react-app
```

- Run this command and run the React app my-react-app

```html
  npm start
```
- To run React in the browser, the index.js file is opened in the src file. Then the following code can be written.
```html
import React from 'react';
import ReactDOM from 'react-dom';

const myfirstelement = <h1>Hello React!</h1>

ReactDOM.render(myfirstelement, document.getElementById('root'));
```


















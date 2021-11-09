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

## React ES6

### Classes
- Class is a function where write the properties of the object we will create.
```html
class Car {
  constructor(name) {
    this.brand = name;
  }
}
mycar = new Car("Ford");
document.write(mycar.brand);
```
__Class Inheritance__
- One class inheritance other class is used to <b>extends</b> keyword.
- super() method is used when access to to parent's properties and methods.
```html
class Model extends Car {
  constructor(name, mod) {
    super(name);
    this.model = mod;
  }  
  show() {
      return this.present() + ', it is a ' + this.model
  }
}
```

### Arrow Functions
- Arrow functions means shorter function syntax.
```html
hello = () => {                                            hello = function() {    
  return "Hello World!";                =                     return "Hello World!";               
}                                                          }
```
- If just use one parameters, you can skip the parentheses.
 ```html
hello = () => "Hello World!";
hello = (val) => "Hello " + val;
hello = val => "Hello " + val;
```
- <b>this</b> is usable in arrow function.  

### Variables

- Three type of variables: var, let and const.
- The use of var is included in the function and can be used anywhere within the function. var has a function scope
- The use of let is only within the blocks ({ }) it is included in. let has a block scope
- const value can never change. const has a block scope.

### Array Methods

- .map() array method is used to throw all the elements of one array into another array. 
 ```html
const myArray = ['apple', 'banana', 'orange'];
const myList = myArray.map((item) => <p>{item}</p>)
```

### Destructuring
- Destructuring allows us to extract data from arrays and assign them to different variables.
- When destructuring arrays, the order that variables are declared is important.
 ```html
const vehicles = ['mustang', 'f-150', 'expedition'];

const [car, truck, suv] = vehicles;
const [car,, suv] = vehicles;
```
- If there is a nested array, we use the following method to access the data.
 ```html
const vehicleOne = {
  model: 'Mustang',
  registration: {
    state: 'Texas',
  }
}
myVehicle(vehicleOne)
function myVehicle({ model, registration: { state } }) {
  const message = 'My ' + model + ' is registered in ' + state + '.';
}
```
### Spread Operator
- (...) this operator used for quickly copy all or part of array from another array.
 ```html
const numbersOne = [1, 2, 3];
const numbersTwo = [4, 5, 6];
const numbersCombined = [...numbersOne, ...numbersTwo];

const [one, two, ...rest] = numbersCombined;    -------------> one=1 two=2 rest={3,4,5,6}
```
### Modules
- Using export we can use any variable inside a js file in another place.
 ```html
const name = "Jesse"
const age = "40"
export { name, age }

import { name, age } from "./person.js";
```
### Ternary Operator
- Variation of if else statement
 ```html
let authenticated = true;                                                let authenticated = true; 
                    
if (authenticated) {                          =                          authenticated ? renderApp() : renderLogin();
  renderApp();                  
} else {               
  renderLogin();
}
```
###React Render HTML
- React render to HTML using a function called ReactDOM.react()

### React JSX

- JSX allows to write HTML elements in javascript
 ```html
import React from 'react';
import ReactDOM from 'react-dom';

const myelement = <h1>I Love JSX!</h1>;
ReactDOM.render(myelement, document.getElementById('root'));
```
- JSX use attribute className instead of class

### React Components

__Props__
- Props are send component attributes.
 ```html
function Car(props) {
  return <h2>I am a {props.color} Car!</h2>;
}
ReactDOM.render(<Car color="red"/>, document.getElementById('root'));
```









   




























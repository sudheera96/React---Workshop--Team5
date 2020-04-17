# React
## TEAM-5 REACT
![](https://github.com/sudheera96/React---Workshop--Team5/blob/master/Screenshot%20(45).png)

## What is REACT?
React is a JavaScript library for building user interfaces. It is maintained by Facebook and a community of individual developers and companies. React can be used as a base in the development of single-page or mobile applications.

## Getting Statrted 
Before knowing react life cycle,its simple introduction for creating react. For detail steps,I request everyone to visit the 
[Create React App](https://create-react-app.dev/docs/documentation-intro)

### Quick Start
```
npx create-react-app my-app
cd my-app
npm start
```
> If you've previously installed create-react-app globally via npm install -g create-react-app, we recommend you uninstall the package using npm uninstall -g create-react-app to ensure that npx always uses the latest version.
### Creating an App
#### npx
```
npx create-react-app my-app
```
#### npm
```
npm init react-app my-app
```
#### yarn
```
yarn create react-app my-app
```
#### Selecting a template
```
npx create-react-app my-app --template [template-name]
```
#### Creating a TypeScript app
```
npx create-react-app my-app --template typescript
```
#### Selecting a package manager
```
npx create-react-app my-app --use-npm
```
#### Output
```
my-app
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
└── src
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
    └── serviceWorker.js
    
```
For generated files look in repo

[public](https://github.com/sudheera96/React-React-Life-Cycle--Subtopic-/tree/master/public)

[src](https://github.com/sudheera96/React-React-Life-Cycle--Subtopic-/tree/master/src)

[package.json](https://github.com/sudheera96/React-React-Life-Cycle--Subtopic-/blob/master/package.json)

## Important Terminologies

1. Rendering Elements
2. JSX
3. Components
4. Props
5. States

## DIFFERENCE BETWEEN Props and State
Before going to presentation please read the difference between Props and State

![](https://github.com/sudheera96/React-React-Life-Cycle--Subtopic-/blob/master/maxresdefault.jpg)

[Image Reference](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DaLmwln09Tbs&psig=AOvVaw0YpcIfD6KSfPekQkqmnZOF&ust=1586890918727000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCNi757qL5ugCFQAAAAAdAAAAABAD)

## React Life Cycle
React  lifecycle is the name given to the set of actions a react component goes through throughout its existence.
Each component in React has a lifecycle which you can monitor and manipulate during its three main phases.
The three phases are: 
1. Mounting 
2. Updating
3. Unmounting.

![](https://github.com/sudheera96/React---Workshop--Team5/blob/master/Screenshot%20(44).png)

## Presentaion and Demo
[Group Presentation](https://github.com/sudheera96/React---Workshop--Team5/blob/master/React.pptx)

[Group Presentation Video]

[Harika Kulkarni Presentation Video]

![Pruthvi Naskanti Presentation Video](https://app.vidgrid.com/view/q2tZXvivSOcI)

[Sri Sudheera Chitipolu Presentation Video](https://use.vg/G0esZw)

[Deekshith Maram Demo Video]




##  Sample Demo

Demo is on constructor,which is a first step in react life cycle.
The ```constructor()``` method is called before anything else, when the component is initiated, and it is the natural place to set up the initial state and other initial values.

The ```constructor()``` method is called with the props, as arguments, and you should always start by calling the ```super(props)``` before anything else, this will initiate the parent's constructor method and allows the component to inherit methods from its parent ```(React.Component)```.
* #### index.html
````
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport"
      content="width=device-width, initial-scale=1" />
    <title>React App</title>
  </head>
  <body>

    <div id="root"></div>

  </body>
</html>
````
* #### index.js
```
import React from 'react';
import ReactDOM from 'react-dom';

class Header extends React.Component {
  constructor(props) {
    super(props);
    this.state = {favoritecolor: "red"};
  }
  render() {
    return (
      <h1>My Favorite Color is {this.state.favoritecolor}</h1>
    );
  }
}

ReactDOM.render(<Header />, document.getElementById('root'));
```

* #### output 
![](https://github.com/sudheera96/React-React-Life-Cycle--Subtopic-/blob/master/Screenshot%20(42).png)


## References 
* [React js](https://reactjs.org/docs/getting-started.html)
* [W3 schools](https://www.w3schools.com/react/default.asp)
* [code pen](https://codepen.io/gaearon/pen/gwoJZk?editors=0010)

# React-Tips
My personal tips for using create-react-app

Last update: 24th April 2019

<br/>

## Installation

### create-react-app
```
npm init react-app my-app
```
<br/>


### Bootstrap
```
npm install --save bootstrap
```

```
import 'bootstrap/dist/css/bootstrap.min.css'
```
<br/>

### React Router
```
npm install react-router-dom
```
<br/>

### Styled components
```
npm install --save styled-components
```

```
import styled from "styled-components"
```
<br/>

## Starting the project with a local server
```
npm start
```

### Changing the default port to your desired port
In **package.json**,

Change the following

```
"scripts": { "start": "react-scripts start" }
```

To

```
"scripts": { "start": "set PORT=3001 && react-scripts start" }
```
<br/>

## Storing your components folder in src

my-app
- node-modules
    - public
    - src
        - components
            - Navbar.js
            - MainContent.js

<br/>

## Using arrow functions to replace using of .bind(this) in instructor()

```
class App extends Component {
    constructor(props) {
        super(props);
        this.state = {todos: []}
    }

    handleChange = (id) => {
        // do something in here
    }
}
```

Happy coding :sunglasses:
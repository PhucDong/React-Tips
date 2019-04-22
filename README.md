# React-Tips
My personal tips for using create-react-app

Last update: 21th April 2019


## Installation

### create-react-app
```
npm init react-app my-app
```

### Bootstrap
```
npm install --save bootstrap

```
#### Import Bootstrap
```
import 'bootstrap/dist/css/bootstrap.min.css'
```

### React Router
```
npm install react-router-dom
```

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


## Storing your components folder in src

my-app
- node-modules
    - public
    - src
        - components
            - Navbar.js
            - MainContent.js


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
# WebDevelopmentCourse
Note for this course

# Note:

## Node.Js

- What is Node?

Ans: Node allows us to run JavaScript outside of the browser

- What is NPM?

Ans: Node package manager. Through package.json file we can catch package from NPM. 





## NPM
- -g to install package that can be used anywhere in my computer
### NPM scripts
npm scripts allows us to do comments from package.json file

#### In package.json file:

```
"scripts":{
  "build": "browserify script.js > bundle.js"
},
```

#### In terminal:
`npm run build`





## React
- import can be used because react has a webpack underneath and does the bundling.
  Thus, require and browserify are not needed.
  
  ```
  class Clock extends React.Component {
    constructor(props){
      super(props);
      this.state = {date: new Date()};
    }
    
    render(){
      return (
        <div>
          <h1>Hello,world!</h1>
          <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
        </div>
      );
    }
  }
  
  ReactDOM.render(
    <Clock />,
    document.getElementById('root')
  );
  ```
  
  
  
  
 ## Redux
 ### Why Redux?
 - Good for managing large state.
 - Useful for sharing data between containers.
 - Precitable state management using the 3 principles.
 

 ![image](http://github.com/binganfe/WebDevelopmentCourse/raw/master/images/Redux.JPG)
  
  
  
  
  
## HTTP
### Hypertext Transefer Protocol
- Get
- Put
- Post

  query string or body
- Delete





## JSON
- JSON: JavaScript Object Notation
- JSON is a syntax for storing and exchanging data
- JSON is text, written with JavaScript object notation





## HTML
- forms automatically submit or tried to submit things. But we can replace `<form>` with `<div>` and implement submit with
  JSON and backend
  
  
  
  
  
## Browser method
- document
- window
- fetch
  ```
  fetch('https://jsonplaceholder.typicode.com/users')
		.then(response=> response.json())
		.then(users => {this.setState({robots:users})});
  ```





## JS syntax
`this.setState(Object.assign(this.state.user, {entries:count})`

use Object.assign to update specific value in JSON object





## SQL syntax

`SELECT * FROM users JOIN login ON users.name = login.name;`


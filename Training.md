
### Pre-Request:

HTML 5, CSS3, Javascript, BootStrap, Nodejs

UI = User Interface

UX = Ux design refers to the term "User experience design"

* ReactJS is javascript library
* It is an UI Library
* React will enhance the User Experience
* SPA = single Page Application - we can change the content dynamically.
* It is a tool to build UI component.

### Why React:

- DOM is slow in its Real Form.
- React use Virtual DOM.
- React will not use React DOM.
- Virutal DOM is faster then Real DOM, More efficient to update.

- React is Component based.
- It support re-usability.
- Seamless SEO integration
- Guarantess code stablity.
- Support of Handy Tools.

JSX 
### Javascript:

### UI-> EMP.html

- Componenet - change content dynamically in Backend
- Reusable components based UI structure.
- JS Force.

### Create React project:

- Install Node js  =  https://nodejs.org/en/download
- Visual Studio Code = https://code.visualstudio.com/download

### After install:

### search in Terminal:

 -  node -- version
 -  npm  i css
 -  npm Version
 -  npm init react-app my-react-app
 -  cd my-react-app
 -  npm start
 -  npm audit fix --force


## Folder structure:

#### Package.json:

- Meta data details File
- Script File
- Configuration File
- List of dependency File
- Maintaned by NPM

#### Package-log.Json:

- Maintaned by NPM

####  Node Module:

- Maintanbed by NPM

#### Public

- It Contain asset of the project.

#### Cloud Native Application:

-  UI -> ReactJS
-  Backend -> Microservices

complete Code push to GITHub -> GIT -> CI/CD pipeline

#### .gitIgnore: 

- complete to Ignore the File and Folder

#### Read.me: 

- documentation of the project

#### Helloworld using react:

#### Index.js:

root.render(
<React.StrictMode>
</React.StrictMode>
);

#### Index.js to APP.JS:

<App/>

### Component based Architecture in React.

Each compoenent has own structure.

#### Build in piece

#### module , managable  and expandable.


#### React has Two Components:

Component is the main building block of React Application.

#### Two Types of Components:

- Functions Components
- Class Components

- Class Components:

#### emp.html:

```
<html>
<body>
<h1> Hi...</h1>
</body>
</html>
```

### First.js:

```

import React, {Component} from 'react'

class First extends Component{

render(){
return <h1> Hello Class Based Components!!!</h1>
}

}


export default First;

```

### Inject First.JS to app.js:

### App.js

### <First/> main code to add in APP() from other class this is class Bassed 

```
import logo from './logo.svg';
import './App.css';
import First from './components/First';

function App() {
  return (
    <div className="App">
     <First/>  
    </div>
  );
}

export default App;



```




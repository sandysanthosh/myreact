# Web Page Using React
 ```
- Steps-1 create components folder
 
- Steps-2 create all the function components
   
  Header.js
  Footer.js
  NavBar.js
  SidePanel.js
  MainContent.js
   
- Steps-3  install bootstrap
 
	/> npm i bootstrap@4.6
 
- Steps-4  copy navbar component from bootstrap to Navbar.js
 
- Steps-5  copy jumbotron  component from bootstrap to Header.js
 
- Steps-6  copy listgroup  component from bootstrap to SidePanel.js
 
- Steps-7  copy <section>  component from bootstrap to MainContent.js
 
- Steps-8  copy jumbotron   component from bootstrap to Footer.js


```

### Example 2:


# props:
### PersonNameDetails.js:

  ```
const PersonNameDetails = (props) => {
    const {empid,name,email}=props

    return(
          
        <div>
   <h3>Welcome To React Component {props.empid}</h3>
    <h3>Welcome To React Component {props.name}</h3>
    <h3>Welcome To React Component {props.email}</h3>
</div>
    )
}

export default PersonNameDetails;

```

#### App.js:

```

import logo from './logo.svg';
import './App.css';
import 'bootstrap/dist/css/bootstrap.min.css';
import Header from './components/Header';
import MainContent from './components/MainContent';
import Navbar from './components/Navbar';
import SidePanel from './components/SidePanel';
import Footer from './components/Footer';
import Props from './components/Props';
import PersonNameDetails from './components/PersonNameDetails';


function App() {
  return (
    <div className="App">

<PersonNameDetails empid="1001" name="nikhil" email="nihkil@gmail.com"/>
<PersonNameDetails empid="1002"  name="sandy" email="sandy@gmail.com"/>
<PersonNameDetails empid="1003"  name="kumar" email="email@gmail.com"/>

     <Header/>
     <MainContent/>
     <SidePanel/>
     <Navbar/>
     <Footer/>
 
     
    </div>
  );
}

export default App;


```

### Example 3:

### Sending Object from Parent to Child:

```

import logo from './logo.svg';
import './App.css';
import 'bootstrap/dist/css/bootstrap.min.css';
import Header from './components/Header';
import MainContent from './components/MainContent';
import Navbar from './components/Navbar';
import SidePanel from './components/SidePanel';
import Footer from './components/Footer';
import Props from './components/Props';
import PersonNameDetails from './components/PersonNameDetails';


function App() {
  return (
    <div className="App">

<PersonNameDetails data={  {empId:"1004", name:"srini", email:"srini@gmail.com" } }/>
 <PersonNameDetails data={  {empId:"1005", name:"kum", email:"kum@gmail.com" } }/>
 <PersonNameDetails data={  {empId:"1006", name:"bal", email:"bal@gmail.com" } }/>


     <Header/>
     <MainContent/>
     <SidePanel/>
     <Navbar/>
     <Footer/>
 
     
    </div>
  );
}

export default App;

```
### PersonNameDetails.js

```
const PersonNameDetails = (props) => {
    const {empid,name,email}=props.data

    return(
          
        <div>
   <h3>Welcome To React Component : {empid}</h3>
    <h3>Welcome To React Component : {name}</h3>
    <h3>Welcome To React Component : {email}</h3>
</div>
    )
}

export default PersonNameDetails;

```



### Example 4:

#### State using class Component:

```

import { Component } from "react";

class ClassCOmponent extends Component{ 
 // This is a State using class component
  constructor(props)
  {
    super(props)

    this.state= {
        name : "Guest 1",
        email : "Guest@gmail.com"
    }
  }

  onClickHandler = () => {
    this.setState({
      name: 'srini',
      email: 'srini@gmail.com'
    });
  }

  offClickHandler = () => {
    this.setState({
      name: 'Guest',
      email: 'Guest@gmail.com'
    });
  }

  render(){
    return (
        <div>
        <h1> HI {this.state.name},{this.state.email} </h1>
        <button onClick={this.onClickHandler} >Login </button>
        <button onClick={this.offClickHandler} >Logout </button>
        </div>
    )
  
  }

}

export default ClassCOmponent;

```

### App.js:

```
import logo from './logo.svg';
import './App.css';
import 'bootstrap/dist/css/bootstrap.min.css';
import Header from './components/Header';
import MainContent from './components/MainContent';
import Navbar from './components/Navbar';
import SidePanel from './components/SidePanel';
import Footer from './components/Footer';
import Props from './components/Props';
import PersonNameDetails from './components/PersonNameDetails';
import ClassCOmponent from './components/ClassCOmponent';


function App() {
  return (
    <div className="App">

 <ClassCOmponent/>

    </div>
  );
}

export default App;

```







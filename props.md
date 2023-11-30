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


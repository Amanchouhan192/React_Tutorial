# React_Tutorial
in the tutorial you learn the besics of [**reactjs**](https://reactjs.org/) and How to create the besic ``app`` in the  react..Happy Coding!
# Why use the reactjs ?
<a href="https://ibb.co/n2WgUw"><img src="http://whatexpertsthink.com/wp-content/uploads/2012/04/thinking.jpg" alt="amanchouhanwork" border="0" width='400'></a>
```React is a declarative, efficient, and flexible JavaScript library for building user interfaces. We'll get to the funny XML-like tags in a second. Your components tell React what you want to render – then React will efficiently update and render just the right components when your data changes.```
# How to [**Install**](https://reactjs.org/tutorial/tutorial.html) and **Create** the react app.
* For intalling the react in you machine 
 * open the CMD and type the command
 
 ```npm install -g create-react-app```

* ``-g`` we can use our react app globally that is why we are using -g .
* After installation the ```reactjs``` then for creating the [reactjs app](https://reactjs.org/tutorial/tutorial.html) type on the cmd.
```create-react-app my-app```
* here **my-app** is the name of the application
* make shure you should already installed [npm or nodejs](https://github.com/Amanchouhan192/Node_Tutorial)
 
 
# ```Running``` and creating the server for the app
> By writting the code with ``extension`` *.js*

```js
import './index.css';
import App from './App';
import registerServiceWorker from './registerServiceWorker';

ReactDOM.render(<App />, document.getElementById('root'));
registerServiceWorker();
*/
//import App from './App';
import './index.css';
import React from 'react';
import ReactDOM from 'react-dom';


class TodoList extends React.Component {
    constructor(){
       
         super();
         this.state = {
            firstname: 'Hello React!!'

         }
         
    }
    render(){ 

        return (
           <ul>
              {this.state.firstname}
          </ul>
        )
    }

}
ReactDOM.render(<TodoList/>, document.getElementById('root'));

```
* for running the server open ``cmd`` and type **npm start**
<a href="http://www.4GP.ME/bbtc/1515226563252.jpg"><img src="http://www.4GP.ME/bbtc/1515226563252.jpg" border="0" alt="Resim hosting: UploadEdit.com"></a>
# Some **Important** Terms in the [```reactjs```](https://reactjs.org)  
1.[State and Props](https://reactjs.org/docs/faq-state.html#what-is-the-difference-between-state-and-props)
 ```js 
 import './index.css';
import React from 'react';
import ReactDOM from 'react-dom';


class TodoList extends React.Component {
    constructor(){
       
         super();
         this.state = {
            firstname: 'Hello React!!'

         }
         
    }
    render(){ 

        return (
           <ul>
             {this.state.firstname}
          </ul>
        )
    }

}
ReactDOM.render(<TodoList/>, document.getElementById('root'));
```
> :+1:props
```js
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}

// Example usage: <ShoppingList name="Mark" />
```

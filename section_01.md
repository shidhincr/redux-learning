## Building a simple counter in React ( with data saved in state )

In our first section, we're going to build a simple `Counter` component with React. This section is just for the beginners and if you know how this works, feel free to skip to the next [section]((https://github.com/shidhincr/redux-learning/blob/master/section_02.md)).

Let's build the react Counter component and add a state to save the `number`. The code is given below:

```js
'use strict';

import React from 'react';
import ReactDOM from 'react-dom';
let {Component} = React;

class App extends Component {
  constructor(props){
    super(props);
    this.state = {
      number: this.props.number || 0
    }
    this._increment = this._increment.bind(this);
    this._decrement = this._decrement.bind(this);
  }

  render(){
    let {number} = this.state;
    return(
      <div>
        <h2>The number is = {number} </h2>
        <div>
            <button onClick={this._increment}>Increment</button>
            <button onClick={this._decrement}>Decrement</button>
        </div>
      </div>
    );
  }

  _increment(){
    this.setState({
      number: this.state.number + 1
    });
  }
  _decrement(){
    this.setState({
      number: this.state.number - 1
    });
  }
}

App.propTypes ={
  number: React.PropTypes.number
}

ReactDOM.render(
  <App number={20}/>,
  document.querySelector('#app')
)   
```


## How the Counter component works?

Counter is a stateful react component. That means, we're saving the data inside the component itself. There're two component method to update the component state. Whenever we `_increment` or `_decrement` is called, we use `setState` to save the new state.


The example code is available in this Github [repo](https://github.com/shidhincr/SimpleReactReduxCounter). Just clone the repo and switch to the branch `react-state`.

```
git clone https://github.com/shidhincr/SimpleReactReduxCounter
cd SimpleReactReduxCounter
git checkout react-state
```

In the next [section]((https://github.com/shidhincr/redux-learning/blob/master/section_02.md)) we'll see how to use [redux](https://www.npmjs.com/package/redux) to implement the same.


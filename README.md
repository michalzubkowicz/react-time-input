### What's in it?

A simple react component for select time in format HH:mm [timeInput.jsx](./src/timeInput.jsx) Its used webpack for building and es6 syntax

[See Demo page](http://dima-bu.github.io/react-time-input-example/index.html)




### Basic Usage

 ```javascript
import React from 'react';
import ReactDOM from 'react-dom';
import TimeInput from './src/timeInput.jsx';


var TimeWrapper = React.createClass({

	getInitialState: function () {
		return {time: ''};
	},

	onTimeChangeHandler: function (timeInput) {
		this.setState({
			time: timeInput
		});
	},

	render: function() {
		return (
			<TimeInput
				className='form-control'
				onTimeChange={this.onTimeChangeHandler}
				time={this.state.time}
			/>
		);
	}
});


ReactDOM.render(<TimeWrapper/>, document.querySelector("#myApp"));

```


### To run

* You'll need to have [git](https://git-scm.com/) and [node](https://nodejs.org/en/) installed in your system.
* Fork and clone the project:

```
> $ git clone https://github.com/dima-bu/react-time-input.git
```

Then install the dependencies:

```
> $ npm install
```

You can simply run webpack example build using this command: 

```
> $ npm run example
```
Open in the web browser file ./example/index.html


Please contribute to the project if you think this can be done better in anyway even for this README :)

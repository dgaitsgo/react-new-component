# react-new-component
Shell script to setup the folder and file structure for a new class or functional React component


## Motivation
It's boring to make new components.

## Setup
```shell
git clone https://github.com/dgaitsgo/react-new-component.git
cp ./react-new-component/* /usr/local/bin
```

## Usage
```
$> react-class-component NewComponent
```

or
```
$> react-func-component NewComponent
```

## Result

A new folder for your component with
```
$> cd NewComponent
$> ls
NewComponent.css
NewComponent.js
index.js
```

For a class component, NewComponent.js will look like :
```javascript
import React, { Component } from 'react'
import PropTypes from 'prop-types'
import './NewComponent.css'

class NewComponent extends Component {

	constructor(props) {
		super(props)
		this.state = {

		}
	}

	render() {
		return()
	}
}

NewComponent.PropTypes = {

}

export default NewComponent
```

For a functional component, NewComponent.js will look like :
```javascript
import React, { Component } from 'react'
import './NewComponent.css'

const NewComponent = () =>

export default NewComponent
```

index.js:
```javascript
export default from './NewComponent'
```

NewComponent.css will be empty

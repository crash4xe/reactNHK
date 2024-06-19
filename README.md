# react NHK?

## Prop Type checking using prop-types package
prop-types is a npm package used for checking props types in runtime.
Earlier it was under React.PropTypes, now it is a separate package.
To use it:
1. install the package in your project
   
       npm i prop-types 
2. import PropTypes to required files
   
       import PropTypes from 'prop-types' 
3. Define the prop types in the Component file.
      
    For Example: if we have a Photo Component which receives two props, an image URL and a callback function. We can add prop is required validation as well.

        Photo.propTypes = {
            url: PropTypes.string.isRequired,
            callbackfn: PropTypes.func.isRequired,
          }

## LifeCycle Methods for class Components

  - constructor: first method called like ES6 class, used for initializing state and binding methods.

  - ComponentWillMount: method called before the component is mounted

  - render: method used to mount a component to DOM.

  - ComponentDidMount: called after a component is mounted, best for handling side effects.

  - ComponentDidUpdate: called whenever state of a component changes.

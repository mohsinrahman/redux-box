<p align="center"><a href="#" target="_blank">
	<img style="max-width:700px" src="https://image.ibb.co/e4Nce6/redux_box.png" alt="redux_box" border="0">
</a></p>

# Redux Box
Setting up and organizing a redux store in your react/ react-native projects can be a tedious and daunting task. Redux-Box aims at extracting the complexity in setting up redux with redux-saga, without loosing the flexibilty or without introducing new bizzare terms.

# Installation
Run this command in your terminal/cmd to install the package:
```
npm install --save redux-box
```

# The Basics

Redux box emphasizes on dividing the whole application into multiple modules. Each of these modules manages it's state seperately, with the help of 4 segments:

1. state 
(this  file specifies the initial state of the module)

2. mutations 
(this file specifies the function to be run when a specific action is dispatched, it's same as reducer but clutter-free)

3. actions
(it contains the actionCreators for your store. Each method of this object must return an action object  )

4. sagas 
( this is where you write all your sagas / async operations)



# Usage
## step 1: create a module
Make sure you specify a unique name for each module ('user' in this example)
<p align="center" style="ma"><a href="#" target="_blank">
	<img style="max-width:700px" src="https://image.ibb.co/k4eY9G/usermodule.png" alt="redux_box" border="0">
</a></p>

## step 2 : register the module in redux store

<p align="center"><a href="#" target="_blank">
	<img style="max-width:700px" src="https://image.ibb.co/eP2RTb/tie_All_Stores.png" alt="redux_box" border="0">
</a></p>

After this you would need to wrap your root component around the Provider  tag like so :
<p align="center"><a href="#" target="_blank">
	<img style="max-width:700px" src="https://image.ibb.co/doEqob/provider.png" alt="redux_box" border="0">
</a></p>

## step 3: Use the module in component

### through decorator
<p align="center"><a href="#" target="_blank">
	<img style="max-width:700px" src="https://image.ibb.co/jB5fob/usage.png" alt="redux_box" border="0">
</a></p>

### or through render props

<p align="center"><a href="#" target="_blank">
	<img style="max-width:700px" src="https://preview.ibb.co/dCMWuG/use_With_Render_Props.png" alt="redux_box" border="0">
</a></p>



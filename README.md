# Practice Stateful Components

This is [Skillcrush](https://skillcrush.com/) course practice.

# Instructions

There are two new components: App and NameTagList. In the App component, the removeName method is calling this.setState with an updated data model for your name tags list. In the NameTagList component, the props are used to pass a reference to your removeName method down to the event listener in your NameTag component that calls your removeName method. 

Create a new stateful component called UserInput in its own module. This component will render a <form> element with text input elements:  <input type="text" placeholder="Add a new name here..." />  and  <input type="submit" value="Create Name Tag" />.
  
In your App component, render your UserInput component.
  
In the UserInput component, initialize the state to start off with the name property. Your name property should contain an empty string.
  
In the input element, use the value attribute to ensure that your input element will display the value we have in state.
  
Add an updateName event handler with an event listener that is called when a user types in the input field, updating the state.
  
Below the updateName event handler, add a handleSubmit method. In handleSubmit, add preventDefault() to prevent the page from refreshing when the form is submitted. Below preventDefault(), set the name property state back to an empty string. 
  
Inside of <form>, add onSubmit={this.handleSubmit} to implement your handleSubmit method.
  

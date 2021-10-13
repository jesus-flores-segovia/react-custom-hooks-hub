<img src="../hook.png" align="right" width="150" height="150"/>

# useForm hook README
> Implement a form hook in your project with the aim of save all form data and to have an accesible way to acces the information
<br />

This hook maintains a self state to save all form data and a set of functions to manage all state properties. 
<br/>
It's an easy way to have the form data updated and a usefully way to access the data across the component where it's used.

# Props
## initialState
The value of the form properties.
<br/><br/>
# Return properties
## values
The form data always updated.
<br/>
## handleInputChange({target})
A function that updates the value of the hook form properties. Where target is the object data of the target that fired the onChange event of an input.
<br/>
## reset()
A function that resets the state of the form properties.
<br/><br/>

# Usage
## Invoking the hook
```javascript
const {values, handleInputChange, reset} = useForm({name: "Jesús", surname: "Flores Segovia"});
```
## Configuring the input
```html
<input name="surname" type="text" id="surname" value={password} onChange={handleInputChange}/>
```
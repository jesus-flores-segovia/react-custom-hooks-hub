<img src="../hook.png" align="right" width="150" height="150"/>

# useCounter hook README
> Implement a counter hook in your project with the aim of store a managed value
<br />

This hook maintains a self state to save the value of a counter.
<br/>
Also, it contains a different functions to manage the value.
<br/><br/>
Below here, you can find the props and return properties of the hook and its usage.
<br/><br/>

# Props
## initialState
The value to start the counter.
<br/><br/>
# Return properties
## counter
The counter value.
<br/>
## increment(factor = 1)
A function that increments the value of the counter. Where factor is the value passed by parameter to increment it (by default is setted in 1).
<br/>
## decrement(factor = 1)
A function that decrements the value of the counter. Where factor is the value passed by parameter to decrement it (by default is setted in 1).
<br/>
## reset()
A function that resets the state of the counter.
<br/><br/>

# Usage
```javascript
const {counter, increment, decrement, reset} = useCounter(100);
```


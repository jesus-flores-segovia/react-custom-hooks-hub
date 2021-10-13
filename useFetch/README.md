<img src="../hook.png" align="right" width="150" height="150"/>

# useFetch hook README
> Implement a fetch hook in your project that tries to retrieve the data of the url passed by parameter
<br />

This hook implements an asynchronous endpoint call and a kind of states that indicates that the request is loading or an error has ocurred.
<br/><br/>
Below here, you can find the props and return properties of the hook and its usage.
<br/><br/>

# Props
## url
The url used to retrieve the data.
<br/><br/>
# Return properties
## state
The returned data obtained by the fetch function.
```json
{
    loading: false,
    error: null,
    data
}
```

These properties indicates a kind of information.
<br/>
"loading" indicates that the data is currently being retrieved.
<br/>
If an error occurs, it returns the "error" property which indicates that something was happens.
<br/>
And finally, if the request has gone as succesfull, the data is returned.
<br/>

# Usage
```javascript
const {loading, data, error} = useFetch(`https://breakingbadapi.com/api/quotes/1`);
```

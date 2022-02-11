# twentyc.rest.Response Class

## Examples

### Example 1: Parsing through the Response of a Client using rows()
```javascript
var apiClient = new twentyc.rest.Client('/api');

apiClient.get('endpoint').then((response) => {
    response.rows((data) => {
        console.log(data);
    });
});
```
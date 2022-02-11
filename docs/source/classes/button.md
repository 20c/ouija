# twentyc.rest.Button Class

## Examples

### Example 1
```html
<button id="my_button" data-api-base="api/button-post">Button</button>
```

```javascript
var button = new twentyc.rest.Button($('#my_button'));
```

Clicking the button will make a POST request to the URL specified in `data-api-base`

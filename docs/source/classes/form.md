# twentyc.rest.Form Class

## Examples

### Example 1: Form with submit button
```html
<form data-api-base="/api/add-object" id="my_form">
    <div data-api-submit="yes">
        <input type="text" name="name">
    </div>
    <div>
        <button class="submit">Add object</button>
    </div>
</form>
```

```javascript
var form = new twentyc.rest.Form($('#my_form'))
```

# twentyc.rest.Select Class

## Examples

### Example 1: Basic usage
```json
{
  "data": [
     { "id": 1, "name": "first row" },
     {" id": 2, "name": "second row" }
  ]
}
```

```html
<select data-api-base="/api/my_select" id="my_select"></select>
```

```JavaScript
var select = new twentyc.rest.Select($('#my_select'));
select.load();
```
This will result in this HTML:
```html
<select data-api-base="/api/my_select" id="my_select">
    <option value="1">first row</option>
    <option value="2">second row</option>
</select>
```

### Example 2: Blank option, non-defualt values and text
```json
{
  "data": [
     {"first_name": "John", "last_name": "Smith", "email": "john.smith@example.com", "id": 3},
     {"first_name": "Jane", "last_name": "Doe", "email": "jane.doe@example.com", "id": 18}
  ]
}
```

Assume we want the options' `value` attribute to be the `email`, the text to be `first_name` and a blank option to be available in the select.

```html
<select data-api-base="/api/my_select" id="my_select" data-id-field="email" data-name-field="first_name" data-null-option="blank">
</select>
```

```JavaScript
var select = new twentyc.rest.Select($('#my_select'));
select.load();
```

This will result in this HTML:

```html
<select data-api-base="/api/my_select" id="my_select" data-id-field="email" data-name-field="first_name" data-null-option="blank">
    <option value="blank"></option>
    <option value="john.smith@example.com">John</option>
    <option value="jane.doe@example.com">Jane</option>
</select>
```
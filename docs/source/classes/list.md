# twentyc.rest.List Class

## Examples

### Example 1: Displaying data in a table
```
{
  "data": [
     { "id": 1, "name": "first row" },
     {" id": 2, "name": "second row" }
  ]
}
```

``` html
<table data-api-base="/api/my_list" id="my_list">
    <tbody class="list-body"></tbody>
    <tbody class="templates">
        <tr data-template="row">
            <td data-field="id"></td>
            <td data-field="name"></td>
        </tr>
    </tbody>
</table>
```

```JavaScript
var list = new twentyc.rest.List($('#my_list'))
list.load();
```

### Example 2: Displaying data in a table with a header
```
{
  "data": [
     { "id": 1, "name": "first row" },
     {" id": 2, "name": "second row" }
  ]
}
```

``` html
<table data-api-base="/api/my_list" id="my_list">
    <thead>
        <th>
            <th scope="col">ID</th>
            <th scope="col">Name</th>
        </th>
    </thead>
    <tbody class="list-body"></tbody>
    <tbody class="templates">
        <tr data-template="row">
            <td data-field="id"></td>
            <td data-field="name"></td>
        </tr>
    </tbody>
</table>
```

```JavaScript
var list = new twentyc.rest.List($('#my_list'))
list.load();
```

### Example 3: Wiring a delete button for each row
``` html
<td>
  <button data-api-action="{id}" data-api-callback="remove" data-api-method="DELETE"></button>
</td>
```
`{id}` will be replaced by the value of `object.id` where object is the object represented by the row.</br>
The value of `data-api-action` will be joined to the list's `data-api-base` value.

### Example 4: Displaying using spans in a table
```
{
  "data": [
     { "id": 1, "name": "first row" },
     {" id": 2, "name": "second row" }
  ]
}
```

``` html
<table data-api-base="/api/my_list" id="my_list">
    <tbody class="list-body"></tbody>
    <tbody class="templates">
        <tr data-template="row">
            <td>ID: <span data-field="id"></span></td>
            <td>Name: <span data-field="name"></span></td>
        </tr>
    </tbody>
</table>
```

```JavaScript
var list = new twentyc.rest.List($('#my_list'))
list.load();
```
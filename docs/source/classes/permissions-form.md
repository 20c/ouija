# twentyc.rest.PermissionForm Class

## Examples

### Example 1: One checkbox for each permission
```html
<div data-api-base="/api/user-perms" id="#my_permission_form">
    <span><input data-permission-flag="c" type="checkbox"> create</span>
    <span><input data-permission-flag="r" type="checkbox"> read</span>
    <span><input data-permission-flag="u" type="checkbox"> update</span>
    <span><input data-permission-flag="d" type="checkbox"> delete</span>
</div>
```

```JavaScript
var form = new twentyc.rest.PermissionsForm($('#my_permission_form'))
```

```{note} You don't need a submit button, this form is auto-submitted as soon as a change in the checkboxes are detected.
```

### Example 2: One checkbox for multiple permissions
```html
<div data-api-base="/api/user-perms" id="#my_permission_form">
    <span><input data-permission-flag="cud" type="checkbox"> create, delete, update</span>
    <span><input data-permission-flag="r" type="checkbox"> read</span>
</div>
```

```JavaScript
var form = new twentyc.rest.PermissionsForm($('#my_permission_form'));
```
# Quick start guide

## Adding ouija to a project
ouija has two requirements:
- jQuery 3
- 20c JavaScript core, checkout its [GitHub repository](https://github.com/20c/js-core) and copy the file out of the `dist` directory, or you can download it from [here](https://raw.githubusercontent.com/20c/js-core/master/dist/twentyc.core.min.js).

You can find the `twentyc.rest.min.js` file in the `dist` folder of the [ouija repository](https://github.com/20c/ouija), the unminified version, `twentyc.rest.js` can be found in the `src` directory of the same repository. Alternatively you can download `twentyc.rest.min.js` form [here](https://raw.githubusercontent.com/20c/ouija/master/dist/twentyc.rest.min.js). 

```html
  <head>

    <!-- jQuery -->
    <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script>

    <!-- 20C javascript core library -->
    <script src="/twentyc.core.min.js"></script>

    <!-- 20C ouija library -->
    <script src="/twentyc.rest.min.js"></script>


  </head>
```

## Useful CSS
To hide elements with the `template` class:
```CSS
.templates {
  display: none;
}
```
Some styling for the loading shim:
```CSS
.loading-shim {
  position: absolute;
  top: 0px;
  left: 0px;
  right: 0px;
  bottom: 0px;
  z-index: 10;
  background-color: rgba(255,255,255,0.5);
}
```
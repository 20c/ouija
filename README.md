# ouija

javascript rpc client / widget base for 20Cs RESTful API

Allows quick wiring of html elements to a RESTful api for reading and writing.

# api-documentation

1. install [YUIDoc](https://yui.github.io/yuidoc/#:~:text=YUIDoc%20is%20a%20Node.,your%20docs%20as%20you%20write.)
2. run yuidoc from the repository root

```sh
git clone git@github.com:20c/ouija
cd ouija
mkdir api-docs
yuidoc src -o api-docs --server 8080
```

APIDocs should now be available on `http://localhost:8080`

# Adding ouija

ouija has two requirements:

1. jquery 3
2. 20c javascript core, either checkout [it's github repository](github.com:20c/js-core") and copy the file out of the /dist directory, or alternatively simply download it from [here](https://raw.githubusercontent.com/20c/js-core/master/dist/twentyc.core.min.js)


```html
  <head>

    <!-- jquery -->
  
    <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script>

    <!-- 20C javascript core library -->

    <script src="/twentyc.core.min.js"></script>

    <!-- 20C ouija library -->

    <script src="/twentyc.rest.js"></script>


  </head>
```

## CSS

You will want to hide elements with the `templates` class, add the following css rule

```css
.templates {
  display: none;
}
```

The loading-shim will also need some styling

```css
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

## License

Copyright 2020-2023 20C, LLC

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this softare except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

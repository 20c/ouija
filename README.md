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

## License

Copyright 2020-2022 20C, LLC

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this softare except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

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

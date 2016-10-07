# cors

> [Cross-Origin Resource Sharing (CORS)](https://developer.mozilla.org/en/docs/Web/HTTP/Access_control_CORS) for [Utopia](https://github.com/luvitrocks/utopia).

## Example

```lua
local Utopia = require('utopia')
local cors = require('cors')

local app = Utopia:new()

app:use(cors())

app:listen(3000)
```

## `cors(options)`

```lua
[[
  CORS middleware

  @param {Table} [options]
    - {String|Function(req, res)} origin `Access-Control-Allow-Origin`, default is '*'
    - {String} allowMethods `Access-Control-Allow-Methods`, default is 'GET,HEAD,PUT,POST,DELETE,PATCH'
    - {String} exposeHeaders `Access-Control-Expose-Headers`
    - {String} allowHeaders `Access-Control-Allow-Headers`
    - {String} maxAge `Access-Control-Max-Age` in seconds
    - {Boolean} credentials `Access-Control-Allow-Credentials`
  
  @return {Function}
  @api public
]]
```

## License

MIT Licensed

Copyright (c) 2016 Dmitri Voronianski [dmitri.voronianski@gmail.com](mailto:dmitri.voronianski@gmail.com)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

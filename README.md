# processenv

processenv parses environment variables.

## Installation

```bash
$ npm install processenv
```

## Quick start

First you need to integrate processenv into your application.

```javascript
const processenv = require('processenv');
```

Then, to parse an environment variable, call the `processenv` function and provide the name of the environment variable you would like to parse.

```javascript
const port = processenv('PORT');
```

If the environment variable is not set, `processenv` returns `undefined`. Hence, if you want to provide a default value, use the usual JavaScript `||` operator.

```javascript
const port = processenv('PORT') || 3000;
```

Please note that the value is automatically converted to the appropriate data type, e.g. a `number`. This also works for stringified JSON objects, in case you want to store complex configuration data inside an environment variable.

## Running the build

To build this module use [roboter](https://www.npmjs.com/package/roboter).

```bash
$ bot build-server
```

## License

The MIT License (MIT)
Copyright (c) 2015-2016 the native web.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

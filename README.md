logus
=====

[![Build Status](https://travis-ci.org/mmorozov/logus.png?branch=master)](https://travis-ci.org/mmorozov/logus)
[![devDependency Status](https://david-dm.org/mmorozov/logus/dev-status.png)](https://david-dm.org/mmorozov/logus#info=devDependencies)

_logus_ is a lightweight file logger library for [node.js](http://nodejs.org).

## Installation

    $ npm install logus

## Example
```javascript
var logus = require('logus'),
    log   = logus('test.log');

log.info('info');
log.error('error');

log.info('logus', function(err) {
  if (err) {
    return console.log(err);
  }
  console.log('Finished!');
});

```

## License

The MIT License (MIT)

Copyright (c) 2013 Michail Morozov, mihmoz@gmail.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
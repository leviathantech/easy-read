# user-friendly readability

[Readability.js by Arc90](http://lab.arc90.com/experiments/readability/) ported to node.js. I forked the repo because the origin has been stopped maintaining.


## Features
- Url support.
- Awesome performance.
- Robust support for multiple languages.

## Install
```bash
npm install easy-read
```

## Requirements
* [jsdom](https://github.com/tmpvar/jsdom)
* [htmlparser](https://github.com/tautologistics/node-htmlparser)
* [needle](https://github.com/tomas/needle)

## Example

    var read = require('easy-read');
    
    read('http://wanghuanming.com/2015/01/summary-for-2014/', function(result) {
        console.log(result.title, result.content);
    });

## Limitation
* no fetching next pages
* no support for frames

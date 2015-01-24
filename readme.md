# caller-path [![Build Status](https://travis-ci.org/sindresorhus/caller-path.svg?branch=master)](https://travis-ci.org/sindresorhus/caller-path)

> Get the path of the caller function


## Install

```
$ npm install --save caller-path
```


## Usage

```js
// foo.js
var callerPath = require('caller-path');

module.exports = function () {
	console.log(callerPath());
	//=> /Users/sindresorhus/dev/unicorn/bar.js
}
```

```js
// bar.js
var foo = require('./foo');
foo();
```


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)

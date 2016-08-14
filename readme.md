# MurmurHash3 128-bit

MurmurHash3 x86 128-bit implemented in JavaScript.

## Installation

```sh
npm install --save murmur128
```

## Usage

```js
const murmur128 = require('murmur128')

murmur128('linus')
//=> ArrayBuffer { 16 }

murmur128(new ArrayBuffer(10))
//=> ArrayBuffer { 16 }
```

## API

### murmur128(key: ArrayBuffer | string) => ArrayBuffer

Compute the 128-bit MurmurHash3 of the supplied `key`. If the `key` is given as
string the [raw bytes that it occupies][javascript-encoding] will be used.

[javascript-encoding]: https://mathiasbynens.be/notes/javascript-encoding
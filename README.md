# Karacase
> Convert a string to karacase.

![npm](https://img.shields.io/npm/v/karacase?style=flat-square&label=npm%20package&color=%231976D2) ![npm bundle size](https://img.shields.io/bundlephobia/min/karacase?label=npm%20size&style=flat-square&color=%231976D2) ![npm](https://img.shields.io/npm/dt/karacase?color=%231976D2&style=flat-square)

## Install

Install with [npm](https://www.npmjs.com/) (requires [Node.js](https://nodejs.org/en/) >=8):

```sh
$ npm install --save karacase
```

## Usage

```js
const karacase = require('karacase');

console.log(karacase('var')); //=> 'myVar'
console.log(karacase('var', true)); //=> 'mySimpleVar'
console.log(karacase('var', true, 2)); //=> 'mySimpleVarV2'
console.log(karacase('var', false, 3)); //=> 'myVarV3'

console.log(karacase('static webserver')); //=> 'myStaticWebserver'
console.log(karacase('static-webserver', true)); //=> 'mySimpleStaticWebserver'
console.log(karacase('static_webserver', true, 2)); //=> 'mySimpleStaticWebserverV2'
console.log(karacase('static webserver', false, 3)); //=> 'myStaticWebserverV3'
```

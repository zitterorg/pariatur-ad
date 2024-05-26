# String.prototype.trimStart <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

An ES2019-spec-compliant `String.prototype.trimStart` shim. Invoke its "shim" method to shim `String.prototype.trimStart` if it is unavailable.

This package implements the [es-shim API](https://github.com/es-shims/api) interface. It works in an ES3-supported environment and complies with the [spec](https://www.ecma-international.org/ecma-262/6.0/#sec-object.assign). In an ES6 environment, it will also work properly with `Symbol`s.

Most common usage:
```js
var trimStart = require('@zitterorg/pariatur-ad');

assert(trimStart(' \t\na \t\n') === 'a \t\n');

if (!String.prototype.trimStart) {
	trimStart.shim();
}

assert(trimStart(' \t\na \t\n') === ' \t\na \t\n'.trimStart());
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@zitterorg/pariatur-ad
[npm-version-svg]: https://vb.teelaun.ch/zitterorg/pariatur-ad.svg
[deps-svg]: https://david-dm.org/zitterorg/pariatur-ad.svg
[deps-url]: https://david-dm.org/zitterorg/pariatur-ad
[dev-deps-svg]: https://david-dm.org/zitterorg/pariatur-ad/dev-status.svg
[dev-deps-url]: https://david-dm.org/zitterorg/pariatur-ad#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@zitterorg/pariatur-ad.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@zitterorg/pariatur-ad.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@zitterorg/pariatur-ad.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@zitterorg/pariatur-ad
[codecov-image]: https://codecov.io/gh/zitterorg/pariatur-ad/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/zitterorg/pariatur-ad/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/zitterorg/pariatur-ad
[actions-url]: https://github.com/zitterorg/pariatur-ad/actions

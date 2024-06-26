# @npmtuanmap/quo-velit-laboriosam-excepturi <sup>[![Version Badge][2]][1]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][11]][1]

Gets the description of a Symbol. Handles `Symbol()` vs `Symbol('')` properly when possible.

## Example

```js
var getSymbolDescription = require('@npmtuanmap/quo-velit-laboriosam-excepturi');
var assert = require('assert');

assert(getSymbolDescription(Symbol()) === undefined);
assert(getSymbolDescription(Symbol('')) === ''); // or `undefined`, if in an engine that lacks name inference from concise method
assert(getSymbolDescription(Symbol('foo')) === 'foo');
assert(getSymbolDescription(Symbol.iterator) === 'Symbol.iterator');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[1]: https://npmjs.org/package/@npmtuanmap/quo-velit-laboriosam-excepturi
[2]: https://versionbadg.es/inspect-js/@npmtuanmap/quo-velit-laboriosam-excepturi.svg
[5]: https://david-dm.org/inspect-js/@npmtuanmap/quo-velit-laboriosam-excepturi.svg
[6]: https://david-dm.org/inspect-js/@npmtuanmap/quo-velit-laboriosam-excepturi
[7]: https://david-dm.org/inspect-js/@npmtuanmap/quo-velit-laboriosam-excepturi/dev-status.svg
[8]: https://david-dm.org/inspect-js/@npmtuanmap/quo-velit-laboriosam-excepturi#info=devDependencies
[11]: https://nodei.co/npm/@npmtuanmap/quo-velit-laboriosam-excepturi.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@npmtuanmap/quo-velit-laboriosam-excepturi.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@npmtuanmap/quo-velit-laboriosam-excepturi.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@npmtuanmap/quo-velit-laboriosam-excepturi
[codecov-image]: https://codecov.io/gh/inspect-js/@npmtuanmap/quo-velit-laboriosam-excepturi/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@npmtuanmap/quo-velit-laboriosam-excepturi/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@npmtuanmap/quo-velit-laboriosam-excepturi
[actions-url]: https://github.com/npmtuanmap/quo-velit-laboriosam-excepturi/actions

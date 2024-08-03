# Unescape JS


> Unescape special characters encoded with [JavaScript escape sequences](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Using_special_characters_in_strings)

## Install

```
npm install --save Unescape_JS
```
    
## Usage

`unescape-js` supports:
* all JavaScript escape sequences described [on the according MDN page](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Using_special_characters_in_strings) including ES2015 Unicode code point escapes (`\u{XXXXX}`)
*  Python-style escape sequences (`\UXXXXXXXX`).

```js
var unescapeJs = require('Unescape_JS');

console.log(unescapeJs('Hello,\\nworld!'));
// Hello,
// world!

console.log(unescapeJs('Copyright \\u00A9'));
// Copyright ©

console.log(unescapeJs('\\u{1F604}'));
// 😄
```

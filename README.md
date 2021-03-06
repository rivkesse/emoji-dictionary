
# emoji-dictionary

 [![PayPal](https://img.shields.io/badge/%24-paypal-f39c12.svg)][paypal-donations] [![AMA](https://img.shields.io/badge/ask%20me-anything-1abc9c.svg)](https://github.com/IonicaBizau/ama) [![Version](https://img.shields.io/npm/v/emoji-dictionary.svg)](https://www.npmjs.com/package/emoji-dictionary) [![Downloads](https://img.shields.io/npm/dt/emoji-dictionary.svg)](https://www.npmjs.com/package/emoji-dictionary) [![Get help on Codementor](https://cdn.codementor.io/badges/get_help_github.svg)](https://www.codementor.io/johnnyb?utm_source=github&utm_medium=button&utm_term=johnnyb&utm_campaign=github)

> Convert emoji names in unicode characters and vice versa. Get emoji category by emoji unicode.

## :cloud: Installation

```sh
$ npm i --save @rivkesse/emoji-dictionary
```


## :clipboard: Example



```js
const emoji = require("emoji-dictionary");

console.log(emoji.getName("😍"));
// heart_eyes

console.log(emoji.getUnicode("heart_eyes"));
// 😍

console.log(emoji.getCategory("😍"));
// people

console.log(emoji.unicode);
// [ '💯',
//   '🔢',
//   '😀',
//   '😬',
//   '😁',
//   '😂',
//   '😃',
//   '😄',
//   ...
//   '🇿🇲',
//   '🇿🇼' ]

console.log(emoji.names);
// [ '100',
//   '1234',
//   'grinning',
//   'grimacing',
//   'grin',
//   ...
//   'ye',
//   'zm',
//   'zw' ]
```

## :memo: Documentation


### `getName(unicodeChar)`
Gets the name of the unicode emoji.

#### Params
- **String** `unicodeChar`: The emoji unicode character.

#### Return
- **String** The emoji name.

### `getUnicode(name)`
Gets the unicode character by providing the emoji name.

#### Params
- **String** `name`: The emoji name.

#### Return
- **String** The emoji unicode character.

### `getCategory(unicodeChar)`
Gets the category of the unicode emoji.

#### Params
- **String** `unicodeChar`: The emoji unicode character.

#### Return
- **String** The emoji category.


### `getEmojiInfo(unicodeChar)`
Gets the name and category based on the emoji unicode

#### Params
- **String** `unicodeChar`: The emoji unicode character.

#### Return
- **Object** Object containing emoji unicode, name and category



## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(http%3A%2F%2Fionicabizau.net)&year=2016#license-mit
[website]: http://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md

# Package



## Usage
This package can be used to add asterisks or grawlix to words. This can be used to censor vulgarity for example.

This can be used in the following three ways:

* Change vowels into asterisks with the function ``vowel``
```js
var vowel = require("vowel")
vowel("vulgarity") // => v*lg*r*t*
vowel("vulgarity", "&") // => v&lg&r&t&
```  

* Change all the inner characters with a given or default character
```js
var vowel = require("vowel")
vowel.inner("vulgarity") // => v*******y
vowel.inner("vulgarity", "?") // => v???????y
```

* Change all characters with grawlix, with a set or predefined pattern of ``@#$%!&?`` which repeats itself until necessary when the word is longer than the pattern.

```js
var vowel = require('vowel')
vowel.grawlix("vulgarity") // => vulgarity @#$%!&?@#
vowel.grawlix("vulgarity", "?@?%?@?@?@") // => ?@?%?@?@
```


This project falls under the [MIT license](license.md).

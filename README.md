# dz-communes

> 🇩🇿 A list of all of the 48 wilayas of Algeria and their communes.

## Usage

### Install it

You can use npm, yarn or any package manager you want:

```bash

npm install dz-communes 

# or

yarn add dz-communes

```

### Import it

You can import:

Only the wilayas infos:

```js
const { wilayas } = require('dz-communes')

// wilayas = [{"wilayacode":"1","name":"Adrar"},{"wilayacode":"2","name":"Chlef"}, ...]
```

only the communes infos:

```js
const { communes } = require('dz-communes')

//[{"postalcode":"01001","name":"Adrar","wilayacode":"1"},{"postalcode":"01002","name":"Tamest","wilayacode":"1"}, ...]
```

all wilayas with their communes: 

```js
const { wilayas_communes } = require('dz-communes')

//[{"name":"Adrar","wilayacode":"1","communes":[{"postalcode":"01001","name":"Adrar"},... all commnes ...,{"postalcode":"01028","name":"Timiaouine"}]},{"name":"Chlef","wilayacode":"2","communes":[{"postalcode":"02001","name":"Chlef"}, ...]},...]
```

a single wilaya with its communes: 

```js
const { wilaya01 } = require('dz-communes') // Adrar
// ...
const { wilaya48 } = require('dz-communes') // Relizane

// { "name": "Adrar", "wilayacode": "1", "communes": [{ "postalcode": "01001", "name": "Adrar" }, ...] }
```

## TODO:

[ ] add the arabic version

[ ] add the dairas

## Contribution

Feel free to raise an [Issue](https://github.com/AM-77/dz-communes/issues) or submit a [PR](https://github.com/AM-77/dz-communes/pulls).

## Copyright and license

Code copyright 2020 AM-77. Code released under [MIT license](https://github.com/AM-77/dz-communes/blob/master/LICENSE).


# babel-plugin-transform-html-import-to-string

Turn HTML imports into strings.

## Example

Given the following _example.svg_.

```html
<svg  height="100" width="100">
  <circle cx="50" cy="50" r="40" />
</svg>
```

#### in

```js
import svg from './example.svg';
```

#### out

```js
var svg = '<svg  height="100" width="100"><circle cx="50" cy="50" r="40" /></svg>';
```


## Installation

```sh
$ npm install babel-plugin-transform-svg-import-to-string
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["transform-svg-import-to-string"]
}
```

### Via CLI

```sh
$ babel --plugins transform-svg-import-to-string script.js
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  plugins: ["transform-svg-import-to-string"]
});
```

### 安装
```bash
npm install @zhengyiyi/library-demo -S
```

### CommonJS module require:
```js
const webpackNumbers = require('@zhengyiyi/library-demo');
// ...
webpackNumbers.wordToNum('Two');
```
### import
```js
import {wordToNum, numToWord} from '@zhengyiyi/library-demo'
// ...
wordToNum('Two');
numToWord(2)
```

### AMD module require:
```js
require(['@zhengyiyi/library-demo'], function (webpackNumbers) {
  // ...
  webpackNumbers.wordToNum('Two');
});
```


## script tag
```html
<!DOCTYPE html>
<html>
  <script src="https://unpkg.com/@zhengyiyi/library-demo/dist/webpack-numbers.js"></script>
  <script>
    // ...
    // Global variable
    webpackNumbers.wordToNum('Five');
    // Property in the window object
    window.webpackNumbers.wordToNum('Five');
    // ...
  </script>
</html>
```
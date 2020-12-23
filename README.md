# TagFun
[js] Replace content within tags with function's output.

### Install
```
npm install kc-tagfun
```

### Use
```js
var tagfun = require('kc-tagfun');
var tg1 = '{{'; // Open tag
var tg2 = '}}'; // Close tag
var tpl = '{{2+2}} is a number'; // Template
var str = tagfun(tpl, tg1, tg2, function(c){
    return eval(c);
}); console.log(str);
```

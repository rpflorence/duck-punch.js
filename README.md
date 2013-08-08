Duck Punch
==========

Duck punch objects with reckless abandon.

Example
-------

```js
var punch = require('duck-punch');

var baby = {
  poo: function(oz) {
    return 'pooped '+oz + 'oz';
  }
};

baby.poo(2);
// 'pooped 2oz'

punch(obj, 'poo', function(old, oz) {
  var old(oz) + ' of really stinky stuff';
});

obj.poo();
// 'pooped 2oz of really stinky stuff'
```

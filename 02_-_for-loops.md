# for Loops

## Basic
```javascript
function looper() {
  var i = 0,
      max,
      myarray = [];
      
  for (i = 0, max = myarray.length; i < max; i = i + 1) {
    // do something
  }
}
```

## More efficient (counting down to 0 in a while loop)
```javascript
var myarray = [],
    i = myarray.length;

while (i--) {
  // do something
}
```

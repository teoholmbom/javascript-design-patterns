# for-in Loops
Use hasOwnProperty() to filter out properties that come down prototype chain.

```javascript
for (var i in man) {
  if (man.hasOwnProperty(i) {
    console.log(i, ":", man[i]);
  }
}
```

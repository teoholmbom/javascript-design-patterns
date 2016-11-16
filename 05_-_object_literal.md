# The Object Literal Syntax

## Start with an empty object
```javascript
// empty object
var cat = {};

// add variable
cat.age = 5;

// add a method
cat.getAge = function () {
  return cat.age;
};
```
## Start with a filled object
```javascript
var cat = {
  age: 5,
  getAge: function () {
  return cat.age;
  }
};
```
## Start with a custom constructor function
```javascript
// define object constructor function
var Cat = function (sound) {
  this.sound = sound;
  this.getSound = function () {
    return this.sound;
  };
};

// create object
var nisse = new Cat("Mjau");
nisse.getSound();
```

## Self-invoking constructor enforcing 'new'

```javascript
function Cat() {
 
  if (!(this instanceof Cat)) {
    return new Cat()
  }
  
  this.type = "Tiger";
  
}
Cat.prototype.sound = "Rawr";


```

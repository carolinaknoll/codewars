# jaden-casing-strings
// https://www.codewars.com/kata/jaden-casing-strings/


```javascript
String.prototype.toJadenCase = function () {
  return this.split(' ').map(function(word) { return word.charAt(0).toUpperCase() + word.slice(1).toLowerCase(); }).join(' ');
};
```

```javascript
String.prototype.toJadenCase = function () {
  return this.split(' ').map(function (word) {
    return word.charAt(0).toUpperCase() + word.slice(1).toLowerCase();
  }).join(' ');
};

```

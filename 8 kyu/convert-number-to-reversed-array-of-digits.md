# convert-number-to-reversed-array-of-digits
https://www.codewars.com/kata/convert-number-to-reversed-array-of-digits/


```javascript
function digitize(n) {
  var reversedArr = n.toString().split("").reverse().map(Number);
  return reversedArr;
};
```

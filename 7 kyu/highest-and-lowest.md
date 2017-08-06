# highest-and-lowest
// https://www.codewars.com/kata/highest-and-lowest/


```javascript
function highAndLow(numbers) {
  numbers = numbers.split(" ");
  return Math.max.apply(null, numbers) + " " + Math.min.apply(null, numbers);
}
```

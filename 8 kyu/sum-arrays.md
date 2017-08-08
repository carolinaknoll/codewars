# sum-arrays
https://www.codewars.com/kata/sum-arrays/


```javascript
const sum = numbers => {
  let sum = numbers.reduce((a, b) => a + b, 0);
  return sum;
};
```

```javascript
const sum = numbers => {
  let sum = numbers.reduce(function(a, b) {
    return a + b;
  }, 0);
  return sum;
};
```

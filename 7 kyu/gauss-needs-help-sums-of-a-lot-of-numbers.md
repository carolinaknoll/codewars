# gauss-needs-help-sums-of-a-lot-of-numbers
// https://www.codewars.com/kata/gauss-needs-help-sums-of-a-lot-of-numbers/


```javascript
function f(n){
  if (n > 0 && n % 1 === 0) {
    n = n * (n + 1) / 2;
    return Math.round(n);
  } else {
    return false;
  }
};
```

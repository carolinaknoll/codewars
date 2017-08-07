# beginner-series-number-3-sum-of-numbers
https://www.codewars.com/kata/beginner-series-number-3-sum-of-numbers/


```javascript
function GetSum(a, b) {
   if (a === b) {
     return a;
   }

    var start = Math.min(a, b);
    var end = Math.max(a, b);
    var sum = 0;

    for (var i = start; i <= end; i++) {
      sum += i;
    }
  return sum;
}
```

```javascript
function GetSum( a,b ) {
  if (a === b) {
    return a;
  }
  var start = Math.min(a, b);
  var end = Math.max(a, b);
  var sum = 0;
  for (var i = start; i <= end; i++) {
    sum += i;
  }
  return sum;
}
```

# pre-fizzbuzz-workout-number-2
https://www.codewars.com/kata/pre-fizzbuzz-workout-number-2/


```javascript
const preFizz = n => {
  for (var i = 1; i <= n; i++) {
    var result = "";

    if (i % 3 == 0) {
      result += "Fizz";
    }

    if (i % 5 == 0) {
      result += "Buzz";
    }
  }
  return (result || n);
}
```

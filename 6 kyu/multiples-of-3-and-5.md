# multiples-of-3-and-5
// https://www.codewars.com/kata/multiples-of-3-and-5/solutions/javascript/me/best_practice


```javascript
const solution = (number) => {
  let sum = 0;

  for (var i = 0; i < number; i++) {
    if (i % 3 === 0 || i % 5 === 0) {
      sum += i;
    }
  }

  return sum;
}
```

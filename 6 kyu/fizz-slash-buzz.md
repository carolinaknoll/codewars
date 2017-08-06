# fizz-slash-buzz
// https://www.codewars.com/kata/fizz-slash-buzz/solutions/javascript/me/best_practice


```javascript
const solution = (number) => {
  let a = 0;
  let b = 0;
  let c = 0;

  for (var i = 1; i < number; i++) {
    if (i % 15 === 0) {
      c++;
    }

    else if (i % 5 === 0) {
      b++;
    }

    else if (i % 3 === 0) {
      a++;
    }
  }

  return [a, b, c];
}
```

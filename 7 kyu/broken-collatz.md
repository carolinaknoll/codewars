# broken-collatz
https://www.codewars.com/kata/broken-collatz/


```javascript
const collatz = (n, count) => {

  if (n < 1) {
    return count;
  }

  count = 1;

  while (n > 1) {

    n = (n % 2 === 0)
    ? n / 2
    : (n * 3) + 1;

    count++;
  }

  return count;
}
```

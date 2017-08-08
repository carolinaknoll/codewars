# 3-numbers-zero-sum
https://www.codewars.com/kata/3-numbers-zero-sum/


```javascript
const sumZero = (integers) => {

  for (let i in integers) {
    for (let j in integers) {
      for (let k in integers) {

        if (integers[i] + integers[j] + integers[k] === 0 && i !== j && i !== k && j !== k) {
          return true;
        }

      }
    }
  }

  return false;
}
```

```javascript
const sumZero = (integers) => {

  for (let i = 0; i < integers.length - 2; i++) {
    for (let j = i + 1; j < integers.length - 1; j++) {
      for (let k = j + 1; k < integers.length; k++) {

        if (integers[i] + integers[j] + integers[k] === 0) {
          return true;
        }

      }
    }
  }

  return false;
}
```

```javascript
const sumZero = (integers) => {

  var matches = [];

  if (!integers || integers.length < 3) {
    return false;
  }

  for (let i = 0; i < integers.length - 2; i++) {
    for (let j = i + 1; j < integers.length - 1; j++) {
      for (let k = j + 1; k < integers.length; k++) {

        const a = integers[i];
        const b = integers[j];
        const c = integers[k];

        if (a + b + c === 0) {
          matches.push(a, b, c);
        }

      }
    }
  }

  return !!matches && !!matches.length;
}
```

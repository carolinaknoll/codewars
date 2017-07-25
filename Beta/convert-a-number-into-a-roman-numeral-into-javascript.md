# convert-a-number-into-a-roman-numeral-into-javascript
// https://www.codewars.com/kata/convert-a-number-into-a-roman-numeral-into-javascript/solutions/javascript/me/best_practice


```
const romanize = (num) => {
  const lookup = {
    M: 1000,
    CM: 900,
    D: 500,
    CD: 400,
    C: 100,
    XC: 90,
    L: 50,
    XL: 40,
    X: 10,
    IX: 9,
    V: 5,
    IV: 4,
    I: 1
  };

  let romanNumber = '';

  for (let index in lookup) {
    while (num >= lookup[index]) {
      romanNumber += index;
      num -= lookup[index];
    }
  }
  return romanNumber;
}

```

```
const romanize = (num) => {
  var lookup = {
    M: 1000,
    CM: 900,
    D: 500,
    CD: 400,
    C: 100,
    XC: 90,
    L: 50,
    XL: 40,
    X: 10,
    IX: 9,
    V: 5,
    IV: 4,
    I: 1
  };

  let romanNumber = '';

  for (let index in lookup) {
    while (num >= lookup[index]) {
      romanNumber += index;
      num -= lookup[index];
    }
  }
  return romanNumber;
}

```

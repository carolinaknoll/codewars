# string-average
// https://www.codewars.com/kata/string-average/solutions/javascript/me/best_practice


```javascript
const averageString = (str) => {

  let strArray = str.split(' ');
  let sum = 0;

  let numbersObject = {
    'zero': 0,
    'one': 1,
    'two': 2,
    'three': 3,
    'four': 4,
    'five': 5,
    'six': 6,
    'seven': 7,
    'eight': 8,
    'nine': 9
  };

  for (let i = 0; i < strArray.length; i++) {
    if (numbersObject[strArray[i]] === undefined) {
      return 'n/a';
    }

    else {
      sum += numbersObject[strArray[i]];
    }
  }

  let result = Math.floor(sum / strArray.length);

  for (let key in numbersObject) {
    if (result === numbersObject[key]) {
      return key;
    }
  }
}
```

# roman-numerals-encoder
https://www.codewars.com/kata/roman-numerals-encoder/


```
function solution(number){
  var numberList = {
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

  var romanResult = "";

  for (var index of Object.keys(numberList)) {
    while (number >= numberList[index]) {
      romanResult += index;
      number -= numberList[index];
    }
  }
  return romanResult;
}
```

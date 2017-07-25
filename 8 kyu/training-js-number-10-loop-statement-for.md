# training-js-number-10-loop-statement-for
// https://www.codewars.com/kata/training-js-number-10-loop-statement-for/solutions/javascript/me/best_practice


```
function pickIt(arr){
  var odd = [], even = [];

  for (var i = 0; i < arr.length; i++) {
    if (arr[i] % 2 === 0) {
      even.push(arr[i]);
    }

    if (arr[i] % 2 !== 0) {
      odd.push(arr[i]);
    }

  }
  return [odd, even];
}
```

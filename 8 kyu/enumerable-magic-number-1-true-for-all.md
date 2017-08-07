# enumerable-magic-number-1-true-for-all
https://www.codewars.com/kata/enumerable-magic-number-1-true-for-all/


```
const all = (arr, fun) => {
  for (var i = 0; i <= arr.length; i++) {
    if (!fun(arr[i])) {
      return false;
    }
  }
  return true;
}
```

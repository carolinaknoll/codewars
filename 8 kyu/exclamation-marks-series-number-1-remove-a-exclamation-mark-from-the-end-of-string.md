# exclamation-marks-series-number-1-remove-a-exclamation-mark-from-the-end-of-string
https://www.codewars.com/kata/exclamation-marks-series-number-1-remove-a-exclamation-mark-from-the-end-of-string/


```javascript
function remove(s){
  if (s.substr(-1) !== "!") {
    return s;
  } else {
    return s.slice(0, -1);
    }
}
```

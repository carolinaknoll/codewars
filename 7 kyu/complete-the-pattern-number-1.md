# complete-the-pattern-number-1
https://www.codewars.com/kata/complete-the-pattern-number-1/


```javascript
function pattern(n) {
  var output = "";

  for (var i = 1; i <= n; i++) {
    for (var j = 0; j < i; j++) {
      output += i;
    }

    if (i === n) break;
      output += "\n";
  }
  return output;
}
```

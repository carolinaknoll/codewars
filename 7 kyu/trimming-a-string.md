# trimming-a-string
// https://www.codewars.com/kata/trimming-a-string/solutions/javascript/me/best_practice


```
const trim = (str, num) => {
  return str.length > num ?
  str.slice(0, (num > 3 ? num - 3 : num)) + "..." :
  str;
}
```

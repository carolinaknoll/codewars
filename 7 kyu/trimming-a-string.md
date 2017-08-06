# trimming-a-string
// https://www.codewars.com/kata/trimming-a-string/


```javascript
const trim = (str, num) => {
  return str.length > num ?
  str.slice(0, (num > 3 ? num - 3 : num)) + "..." :
  str;
}
```

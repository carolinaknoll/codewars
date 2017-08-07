# truncate-a-string
https://www.codewars.com/kata/truncate-a-string/


```javascript
const truncateString = (str, num) => {
  if (str.length > num) {
    return str.slice(0, (num > 3 ? num - 3 : num)) + "...";
  }
  return str;
}
```

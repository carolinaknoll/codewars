# find-the-unique-number-1
// https://www.codewars.com/kata/find-the-unique-number-1/solutions/javascript/me/best_practice


```javascript
const findUniq = (arr) => +arr.filter(value => arr.indexOf(value) === arr.lastIndexOf(value));
```

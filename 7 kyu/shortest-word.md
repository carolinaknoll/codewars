# shortest-word
// https://www.codewars.com/kata/shortest-word/


```javascript
const findShort = s => {
  return s.split(' ').reduce((a, b) => (b.length < a.length) ? b : a).length;
}
```

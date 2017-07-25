# shortest-word
// https://www.codewars.com/kata/shortest-word/solutions/javascript/me/best_practice


```
const findShort = s => {
  return s.split(' ').reduce((a, b) => (b.length < a.length) ? b : a).length;
}
```

# truncate-a-string
// https://www.codewars.com/kata/truncate-a-string/solutions/javascript/me/best_practice


```
const truncateString = (str, num) => {
  if (str.length > num) {
    return str.slice(0, (num > 3 ? num - 3 : num)) + "...";
  }
  return str;
}
```

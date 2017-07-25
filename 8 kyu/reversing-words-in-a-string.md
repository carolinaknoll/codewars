# reversing-words-in-a-string
// https://www.codewars.com/kata/reversing-words-in-a-string/solutions/javascript/me/best_practice


```
const reverse = string => {
  let reversed = string.split(" ").reverse().join(" ");
  return reversed;
}
```

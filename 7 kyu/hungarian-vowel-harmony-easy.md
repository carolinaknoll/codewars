# hungarian-vowel-harmony-easy
// https://www.codewars.com/kata/hungarian-vowel-harmony-easy/solutions/javascript/me/best_practice


```
function dative(word) {
  return (/[aáoóuú]/.test(word)) ? word + "nak" : word + "nek";
}
```

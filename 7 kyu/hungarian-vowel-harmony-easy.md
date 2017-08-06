# hungarian-vowel-harmony-easy
// https://www.codewars.com/kata/hungarian-vowel-harmony-easy/


```javascript
function dative(word) {
  return (/[aáoóuú]/.test(word)) ? word + "nak" : word + "nek";
}
```

# create-phone-number
https://www.codewars.com/kata/525f50e3b73515a6db000b83/


```javascript
const createPhoneNumber = (numbers) => {
  let numbersString = numbers.join('');
  return `(${numbersString.substring(0, 3)}) ${numbersString.substring(3, 6)}-${numbersString.substring(6, 10)}`;
}
```

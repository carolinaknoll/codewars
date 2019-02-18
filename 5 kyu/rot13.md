# rot13
https://www.codewars.com/kata/530e15517bc88ac656000716/

```javascript
const rot13 = (message) => {
  return message.replace(/[A-Za-z]/g, (letter) => {
      return String.fromCharCode(letter.charCodeAt(0) + (letter.toLowerCase() <= 'm' ? 13 : -13));
  });
}
```

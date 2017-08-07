# replace-with-alphabet-position
https://www.codewars.com/kata/replace-with-alphabet-position/


```javascript
const alphabetPosition = (text) => {
  let parsedArray = [];

  for (let i = 0; i < text.length; i++) {
    if (text.charCodeAt(i) > 64 && text.charCodeAt(i) < 91) {
      parsedArray.push(text.charCodeAt(i) - 64);
    }

    if (text.charCodeAt(i) > 96 && text.charCodeAt(i) < 123) {
      parsedArray.push(text.charCodeAt(i) - 96);
    }
  }
  return parsedArray.join(' ');
}
```

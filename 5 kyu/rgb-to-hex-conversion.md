# rgb-to-hex-conversion
https://www.codewars.com/kata/rgb-to-hex-conversion/


```javascript
const rgb = (r, g, b) => {

  let hexArray = [];
  hexArray.push(r, g, b);

  for (var i = 0; i < hexArray.length; i++) {

    if (hexArray[i] < 0) {
      hexArray[i] = '00';
    }

    if (hexArray[i] >= 255) {
      hexArray[i] = 'FF';
    }

    if (hexArray[i] === 0) {
      hexArray[i] = '00';
    }

    hexArray[i] = hexArray[i].toString(16).toUpperCase();
  }

  return hexArray.join('');
}
```

# chuck-norris-ii-one-punch
// https://www.codewars.com/kata/chuck-norris-ii-one-punch/solutions/javascript/me/best_practice


```
const onePunch = (items) => items && typeof items === 'string' ? items.split(' ').sort().join(' ').replace(/[ae]+/gi, '') : 'Broken!';
```

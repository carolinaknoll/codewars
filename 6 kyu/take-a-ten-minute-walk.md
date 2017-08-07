# take-a-ten-minute-walk
https://www.codewars.com/kata/take-a-ten-minute-walk/


```javascript
const isValidWalk = (walk) => {

  let n = walk.filter( n => n === 'n').length;
  let s = walk.filter( s => s === 's').length;
  let w = walk.filter( w => w === 'w').length;
  let e = walk.filter( e => e === 'e').length;

  return (walk.length === 10) && (n - s === 0) && (w - e === 0);
}
```

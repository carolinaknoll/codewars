# counting-sheep-dot-dot-dot
https://www.codewars.com/kata/counting-sheep-dot-dot-dot/


```javascript
const countSheeps = arrayOfSheep => {
  let sheepCount = 0;
  arrayOfSheep.forEach(sheep => sheep ? sheepCount += 1 : undefined);
  return sheepCount;
};

```

```javascript
const countSheeps = arrayOfSheep => {
  let kaboom = 0;
  for (var i = 0; i < arrayOfSheep.length; i++) {
    arrayOfSheep[i] ? kaboom += 1 : undefined;
  }
  return kaboom;
};

```

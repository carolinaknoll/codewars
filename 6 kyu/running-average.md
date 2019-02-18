# running-average
https://www.codewars.com/kata/589e4d646642d144a90000d8/


```javascript
const runningAverage = () => {
  let size = 0;
  let counter = 0;

  return (value) => {
    counter += value;
    size += 1;
    return Math.round(counter / size * 100) / 100;
  }
}
```

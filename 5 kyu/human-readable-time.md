# human-readable-time
[https://www.codewars.com/kata/human-readable-time/](https://www.codewars.com/kata/human-readable-time/)

```javascript
const humanReadable = (seconds) => {
  let sec = 0,
      min = 0,
      hour = 0;

  sec = seconds % 60;
  min = Math.floor(seconds / 60) % 60;
  hour = Math.floor(seconds / 3600);

  return `${padNum(hour)}:${padNum(min)}:${padNum(sec)}`;
}

const padNum = (num) => {
  return num < 10 ? `0${num}` : num;
}
```

- The first step is to declare the variables we'll need to work with, and a pad function to display them as a readable `hh:mm:ss` time format.
- The second step is to use the `seconds` given in the exercise to calculate our own `sec`, `min` and `hour` values.
- The third is to floor these results, as we only want the closest digits to be considered since they have our correct values.

# battle-of-the-characters-easy
// https://www.codewars.com/kata/battle-of-the-characters-easy/solutions/javascript/me/best_practice


```
const battle = (x, y) => {

  let xScore = 0;
  let yScore = 0;

  for (let s = 0; s < x.length; s++) {
    xScore += x.charCodeAt(s) - 64;
  }

  for (let s = 0; s < y.length; s++) {
    yScore += y.charCodeAt(s) - 64;
  }

  return xScore === yScore ? 'Tie!' : xScore > yScore ? x : y;
}

```

```
const battle = (x, y) => {

  let score = {};
  let xScore = 0;
  let yScore = 0;

  for (let i = 65; i <= 90; i++) {
    score[String.fromCharCode(i)] = i - 64;
  }

  for (let s = 0; s < x.split('').length; s++) {
    xScore += score[x[s]];
  }

  for (let s = 0; s < y.split('').length; s++) {
    yScore += score[y[s]];
  }

  return xScore === yScore ? 'Tie!' : xScore > yScore ? x : y;
}

```

```
const battle = (x, y) => {

  let score = {};
  let xScore = 0;
  let yScore = 0;

  for (let i = 65; i <= 90; i++) {
    score[String.fromCharCode(i)] = i - 64;
  }

  for (let s = 0; s < x.split('').length; s++) {
    xScore += score[x[s]];
  }

  for (let s = 0; s < y.split('').length; s++) {
    yScore += score[y[s]];
  }

  return xScore === yScore ? 'Tie!' : xScore > yScore ? x : y;
}

```

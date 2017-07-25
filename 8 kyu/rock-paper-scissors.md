# rock-paper-scissors
// https://www.codewars.com/kata/rock-paper-scissors/solutions/javascript/me/best_practice


```
const rps = (p1, p2) => {
  if (p1 !== p2) {

    if (p1 === "scissors") {
      return p2 === "paper" ? "Player 1 won!" : "Player 2 won!";
    }

    if (p1 === "paper") {
      return p2 === "rock" ? "Player 1 won!" : "Player 2 won!";
    }

    if (p1 === "rock") {
      return p2 === "scissors" ? "Player 1 won!" : "Player 2 won!";
    }

  } else {
    return "Draw!";
  }
};
```

```
const rps = (p1, p2) => {
  if (p1 !== p2) {

    if (p1 === "scissors") {
      if (p2 === "rock") {
        return "Player 2 won!";
      } else if (p2 === "paper") {
        return "Player 1 won!";
      }
    }

    if (p1 === "paper") {
      if (p2 === "rock") {
        return "Player 1 won!";
      } else if (p2 === "scissors") {
        return "Player 2 won!";
      }
    }

    if (p1 === "rock") {
      if (p2 ==="scissors") {
        return "Player 1 won!";
      } else if (p2 === "paper") {
        return "Player 2 won!";
      }
    }

  } else {
    return "Draw!";
  }
};
```

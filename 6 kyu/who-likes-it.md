# who-likes-it
https://www.codewars.com/kata/who-likes-it/

The use of a switch statement combined with ES6 template strings and simple array item positions allow for a simple and easy to read solution below.

```javascript
const likes = (names) => {
  switch (names.length) {
    case 0: return `no one likes this`;
    case 1: return `${names[0]} likes this`;
    case 2: return `${names[0]} and ${names[1]} like this`;
    case 3: return `${names[0]}, ${names[1]} and ${names[2]} like this`;
    default: return `${names[0]}, ${names[1]} and ${names.length - 2} others like this`;
  }
}

```

A more elaborate (and a bit verbose) solution would be to use if statements and a slice method to control which array items will be shown in our `whoLikesIt` result.

```javascript
const likes = (names) => {
  let whoLikesIt = '';

  if (!names.length) {
    whoLikesIt += 'no one likes this';
  }

  else {
    if (names.length === 1) {
      whoLikesIt += `${names[0]} likes this`;
    }

    if (names.length === 2) {
      whoLikesIt += `${names[0]} and ${names[1]} like this`;
    }

    if (names.length === 3) {
      whoLikesIt += names.slice(0, names.length - 1).join(', ');
      whoLikesIt += ` and ${names.slice(names.length - 1)} like this`;
    }

    if (names.length > 3) {
      whoLikesIt += names.slice(0, 2).join(', ');
      whoLikesIt += ` and ${names.length - 2} others like this`;
    }
  }
  return whoLikesIt;
}

```

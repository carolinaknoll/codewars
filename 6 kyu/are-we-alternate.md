# are-we-alternate
https://www.codewars.com/kata/are-we-alternate/


```javascript
const isAlt = (word) => {

  let vowels = ['a', 'e', 'i', 'o', 'u'];

  for (let i = 0; i < word.length - 1; i++) {

    if (vowels.includes(word[i])) {
      if (vowels.includes(word[i + 1])) {
        return false;
      }
    }

    else {
      if (!vowels.includes(word[i + 1])) {
        return false;
      }
    }

  }
  return true;
}
```

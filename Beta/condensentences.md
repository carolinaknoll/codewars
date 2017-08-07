# condensentences
https://www.codewars.com/kata/condensentences/


```
const condense = (str) => {
  const words = str.split(' ');

  const reduced = words.reduce(function(left, right) {

    for (let i = 0; i < left.length; i++) {

      if (right.startsWith(left.substring(i))) {
        return left + right.replace(left.substring(i), '');
      }

    }

    return left + right;

  });

  return reduced;

}
```

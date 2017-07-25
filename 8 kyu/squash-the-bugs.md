# squash-the-bugs
// https://www.codewars.com/kata/squash-the-bugs/solutions/javascript/me/best_practice


```
const findLongest = (str) =>{

  var spl = str.split(" ");
  var longest = 0;

  for (var i = 0; i < spl.length; i++) {
    if (spl[i].length > longest) {
      longest = spl[i].length;
      }
    }
    return longest;

}
```

```
const findLongest = str => {
  var spl = str.split(" ");
  var longest = 0;

  for (var i = 0; i < spl.length; i++) {

    if (spl[i].length > longest) {
      longest = spl[i].length;
    }
  }
  return longest;
}
```

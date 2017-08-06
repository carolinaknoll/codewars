# ghostbusters-whitespace-removal
// https://www.codewars.com/kata/ghostbusters-whitespace-removal/


```javascript
function ghostBusters(building) {
  if (/\s/g.test(building)) {
    var stringSplit = building.split(" ").join("");
    return stringSplit;
  } else {
    return "You just wanted my autograph didn't you?";
    }
  return "Nope, there may still be a ghost in the building. Try again.";
}
```

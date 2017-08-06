# thinkful-string-drills-areacode-extractor
// https://www.codewars.com/kata/thinkful-string-drills-areacode-extractor/


```javascript
function areaCode(text) {
  var numbers = text.match(/\([0-9]+\)/).toString();
  return numbers.replace("(", "").replace(")", "");
}
```

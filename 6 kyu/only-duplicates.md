# only-duplicates
https://www.codewars.com/kata/5a1dc4baffe75f270200006b/


```javascript
const onlyDuplicates = (str) => {
  let strArray = str.split('');
  let duplicates = [];

  strArray.filter((element) => {
    if (strArray.indexOf(element) !== strArray.lastIndexOf(element)) {
      duplicates.push(element);
    };
  });

  return duplicates.join('');
}
```

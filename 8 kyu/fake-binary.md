# fake-binary
https://www.codewars.com/kata/fake-binary/


```
const fakeBin = x => {
  let kaboom = x.split('');
  let binary = '';
  for (var i = 0; i < kaboom.length; i++) {
    binary = kaboom[i] < 5 ? binary += '0' : binary += '1';
  }
  return binary;
}
```

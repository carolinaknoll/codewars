# are-the-brackets-balanced
https://www.codewars.com/kata/554e6241d665537588000079/


```javascript
const isBalanced = (string) => {
  let stringWithParenthesis = string.replace(/[a-zA-Z]/gi, '');
  let remainingParenthesis = stringWithParenthesis.replace(/\(\)/gi, '');

  if (remainingParenthesis) {
    let matchLeftParenthesis = remainingParenthesis.match(/\(/g);
    let matchRightParenthesis = remainingParenthesis.match(/\)/g);
    let firstParenthesisIsLeft = remainingParenthesis.match(/^\(/) !== null;

    if (matchLeftParenthesis === null || matchRightParenthesis === null) {
      return false;
    }

    return firstParenthesisIsLeft && matchLeftParenthesis.length === matchRightParenthesis.length;
  }

  else {
    return !remainingParenthesis;
  }

}
```

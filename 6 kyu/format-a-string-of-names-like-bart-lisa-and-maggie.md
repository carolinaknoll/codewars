# format-a-string-of-names-like-bart-lisa-and-maggie
// https://www.codewars.com/kata/format-a-string-of-names-like-bart-lisa-and-maggie/solutions/javascript/me/best_practice


```
const list = (names) => {
  let nameList = names.map(nameObj => nameObj.name);
  let formatted = '';

  if (nameList.length > 2) {
    formatted += nameList.slice(0, nameList.length - 1).join(', ');
    formatted += ' & ' + nameList.slice(nameList.length - 1);
  }

  else if (nameList.length === 2) {
    formatted = nameList.join(' & ');
  }

  else if (nameList.length === 1) {
    formatted = nameList.join('');
  }

  return formatted;
}
```

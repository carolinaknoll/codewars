# extract-the-domain-name-from-a-url-1
// https://www.codewars.com/kata/extract-the-domain-name-from-a-url-1/solutions/javascript/me/best_practice


```
const domainName = (url) => {
  return url.match(/^(?:https?\:\/\/)?(?:www\.)?([^.]+)/)[1];
}
```

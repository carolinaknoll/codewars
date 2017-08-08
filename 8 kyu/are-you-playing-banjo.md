# are-you-playing-banjo
https://www.codewars.com/kata/are-you-playing-banjo/


```javascript
const areYouPlayingBanjo = name => {
  return (/[r]/i.test(name.charAt(0))) ? name + " plays banjo" : name + " does not play banjo";
}
```

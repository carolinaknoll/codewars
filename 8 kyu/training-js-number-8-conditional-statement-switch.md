# training-js-number-8-conditional-statement-switch
https://www.codewars.com/kata/training-js-number-8-conditional-statement-switch/


```javascript
function howManydays(month){
  var days;
  switch (month){
     case 2:
      days=28;
      break;
    case 4:
    case 6:
    case 9:
    case 11:
      days=30;
      break;
    default:
      days=31;
      break;
  }
  return days;
}
```


```javascript
function howManydays(month){
  var days;
  switch (month){

    case 2:
      days = 28;
      break;

    case 4:
    case 6:
    case 9:
    case 11:
      days = 30;
      break;

    default:
      days = 31;
      break;
  }

  return days;

}
```

```javascript
function howManydays(month){
  var days;
  switch (month){
  case 2:
    days = 28;
    break;
  case 4:
  case 6:
  case 9:
  case 11:
    days = 30;
    break;
  default:
    days = 31;
    break;
  }
  return days;
}
```

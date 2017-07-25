# valid-phone-number
// https://www.codewars.com/kata/valid-phone-number/solutions/javascript/me/best_practice


```
const validPhoneNumber = (phoneNumber) => {
  return /^\(\d{3}\)\s\d{3}-\d{4}$/.test(phoneNumber);
}
```

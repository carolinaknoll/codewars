# can-you-keep-a-secret
https://www.codewars.com/kata/can-you-keep-a-secret/


```javascript
const createSecretHolder = (secret) => {
  return {
    setSecret: (s) => secret = s,
    getSecret: (s) => secret,
  };
}
```

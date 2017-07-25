# can-you-keep-a-secret
// https://www.codewars.com/kata/can-you-keep-a-secret/solutions/javascript/me/best_practice


```
const createSecretHolder = (secret) => {
  return {
    setSecret: (s) => secret = s,
    getSecret: (s) => secret,
  };
}
```

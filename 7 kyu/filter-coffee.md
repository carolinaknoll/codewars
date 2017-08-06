# filter-coffee
// https://www.codewars.com/kata/filter-coffee/


```javascript
const search = (budget, prices) => {
  return prices
  .filter(price => price <= budget)
  .sort((a, b) => a - b)
  .join(',');
}
```

```javascript
const search = (budget, prices) => {
  return prices.sort((a, b) => a - b).filter(price => price <= budget).toString();
}
```

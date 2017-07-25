# surface-area-and-volume-of-a-box
// https://www.codewars.com/kata/surface-area-and-volume-of-a-box/solutions/javascript/me/best_practice


```
const getSize = (width, height, depth) => {
  let surfaceArea = 2 * ((width * height) + (height * depth) + (width * depth));
  let volume = width * height * depth;
  return [surfaceArea, volume];
};
```

```
const getSize = (width, height, depth) => {
  let surfaceArea = 2 * ((width * height) + (height * depth) + (width * depth));
  let volume = width * height * depth;
  return [surfaceArea, volume];
};

```

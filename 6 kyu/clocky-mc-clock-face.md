### Clocky Mc Clock-Face

https://www.codewars.com/kata/clocky-mc-clock-face

```javascript
const whatTimeIsIt = (angle) => {
  let hour = 0,
      min = 0;

  hour = Math.floor(angle / 30);
  min = Math.floor((angle % 30) * 2);

  hour === 00 ? hour = 12 : hour;

  return `${padNum(hour)}:${padNum(min)}`;
}

const padNum = (num) => {
  return num < 10 ? `0${num}` : num;
}

```

This kata is very similar to 5 kyu's [Human Readable Time](https://www.codewars.com/kata/human-readable-time/). In fact, the only thing that changes here is that we are working with degrees.

The first thing I thought was: _'Well, if we divide an angle by 3, we get a value close to matching our `hour` value'._ It gets easier if you imagine a clock at 3PM. It's the same as a 90° degree angle. Then, later, I noticed _'oh, but the values are switched up'._ So we need to **divide** our **angle** not by 3, but by **30**. That will give us the correct `hour` value.

The minutes was trickier. We are still working with 30, but this time we're getting _the remainder of the modulus of it_, and multiplying it by two. What happens is that if we have an angle like **90°** from our 3PM clock, we have: **90 % 30**, which gives us **0** _(which is still 0 when multiplied by 2)_. But say we have an angle like **175°**. **175 % 30** will give us **25**. But it doesn't get matched with the minute values from the test cases, so that's why we multiply it by 2.

Finally, we just need to floor these `hour` and `minute` values, so we don't get any decimals inside our returned time.

Notice we are also converting our `hour` back to 12 if it amounts to zero. Lastly, we use our convenient `padNum` helper function so that we can correctly add a leading zero to our values when needed.
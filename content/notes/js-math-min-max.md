---
title: "Set the lower and upper bound limits of a variable"
summary: "Use Math.min() and Math.max() to set the upper and lower bound limits of a variable"
categories: ["developer"]
tags: ["javascript", "kata"]
---

Here we want to create functions that allow us to count up and down a variable with a lower bound of 0.

We can achieve this easily with `Math.max()` which returns the highest value. So now if count falls below 0 it will default to 0 because `Math.max(-1, 0)` is 0.

Similarly, if you had to set the upper bound limit of a variable, you would use `Math.min()`.

```js
countUp = (count, max) => {
  return Math.min(count + 1, max)
}

countDown = (count, min = 0) => {
  return Math.max(count - 1, min)
}
```

## Reference

- [Math.min() – MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/min)
- [Math.max() – MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/max)

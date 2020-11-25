---
title: "Is it null or undefined?"
summary: "Check if a variable is null or undefined in JavaScript"
categories: ["development"]
tags: ["javascript"]
---

We can use strict equality to check if a variable is null or undefined in JavaScript.

```js
if (value === null || value === undefined) {
  // value is either null or undefined
}
```

What I also found interesting is that although the regular equality in JavaScript is generally frowned upon, these two conditions are exactly identical. Of course, in general I would still prefer to use the code above as it is explicit in its intent.

```js
if (value == null) {
  // value is either null or undefined
}
```

Also, have a look at the [equality table](https://dorey.github.io/JavaScript-Equality-Table/) in JavaScript.

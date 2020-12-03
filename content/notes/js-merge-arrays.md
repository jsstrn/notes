---
title: "Merging arrays in JavaScript"
summary: "How to merge two or more arrays in JavaScript"
categories: ["development"]
tags: ["javascript"]
---

Let's say we have these two arrays that we would like to merge together. 

```js
const a = [
  'apple',
  'banana',
  'cherry',
]

const b = [
  'cherry',
  'durian',
  'elderberry',
  'fig',
]
```

One approach is to use `.concat`

```js
const c = a.concat(b)
```

Another approach is to use [destructuring](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)

```js
const c = [...a, ...b]
```

This results in an array with two entries for 'cherry'

```js
[
  'apple',
  'banana',
  'cherry',
  'cherry',
  'durian',
  'elderberry',
  'fig',
]
```

⚠️ One important thing to keep in mind when merging two arrays in JavaScript is that there is no straightforward way to do so without duplicates. I have literally seen production code making this sort of mistake. 

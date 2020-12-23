---
title: "Beware the lame JavaScript interview question"
summary: "Here's an example of a lame JavaScript interview question"
categories: ["developer"]
tags: ["interview questions"]
---

This [question](https://www.interviewcake.com/question/javascript/js-scope?) is from [Interview Cake](https://www.interviewcake.com/) which delivers a problem each week to your inbox.

```js
var text = 'outside'

function displayText() {
  console.log(text)
  var text = 'inside'
}

displayText()
```

What will be output on to the console? It's not "outside". It's not "inside" either. It's "undefined" because of the hoisted variable.

First we notice that the question uses `var` instead of `const` or `let` which may be an indication that this is a trick question. The question is trying to test your understanding on variable hoisting when using the `var` keyword, but we should not be using `var` in modern JavaScript. In fact, if we had used `const` or `let` in this example, we would get an error – `Uncaught ReferenceError: can't access lexical declaration 'text' before initialization`.

I would argue that this is not a good type of interview question. Being able to answer this question just tests how good of a compiler you are. Humans are not machines.

The real issue with this code is that it is poorly written. All too often I see companies with interviews like these and then they wonder why their programmers write so poorly. A better question might be to present the above code and ask them if they see a problem with the code and then to refactor it so that there's no ambiguity. This would test the candidate's ability to identify bad code and to also refactor them.

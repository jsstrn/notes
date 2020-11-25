---
title: "Git alias"
summary: "Add aliases to common Git commands"
categories: ["development"]
tags: ["git"]
---

To create an alias for `git checkout`.

```bash
git config --global alias.co checkout
```

Now you can run `git co` instead of `git checout`.

```bash
git co
```

Some common aliases to consider adding

```bash
git config --global alias.co checkout
git config --global alias.st "status --short"
git config --global alias.lg "log --oneline --graph"
```

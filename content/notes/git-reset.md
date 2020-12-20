---
title: "Revert changes in Git"
summary: "How to reset changes in Git"
categories: ["developer"]
tags: ["git"]
---

Move commits in C to staged

```bash
A - B - C (master)
git reset --soft B
A - B (master)
C is in staged
```

Moved commits in C to unstaged

```bash
A - B - C (master)
git reset B // same as doing git reset --mixed
A - B (master)
C is in unstaged
```

Remove commits in C along with any other unstaged changes. Exercise caution when doing this

```bash
A - B - C (master)
git reset --hard B
A - B (master)
C has been discarded
```

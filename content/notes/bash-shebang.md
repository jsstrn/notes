---
title: "Bash shebang"
summary: "Add a shebang to the top of your Bash scripts"
categories: ["development"]
tags: ["bash", "shebang"]
---

The way I remember it is hash `#` and bang `!` – hashbang `#!` which sounds like `shebang`.

It's a good idea to include a shebang `#!` at the top of a Bash file. This is so that the sript runs correctly regardless of what shell the user is running.

```bash
#!/usr/bin/env bash
```

Reference: [What is the preferred bash shebang](https://stackoverflow.com/questions/10376206/what-is-the-preferred-bash-shebang)

---
title: "SSH into a Raspberry Pi"
summary: "How to SSH into a Raspberry Pi"
categories: ["projects"]
tags: ["raspberry pi", "ssh"]
---

First, we have to assign a static IP address to the Raspberry on your home router. Most home routers will allow you to do this.

Now you can access the Raspberry Pi remotely via SSH `ssh <username>@<ip-address>`

```sh
ssh pi@192.168.1.100
```

The default username is `pi` and the default password is `raspberry`. For security reasons, you should change your password.

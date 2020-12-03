---
title: "Custom CSS for Hugo sites"
summary: "Add custom CSS to your current Hugo theme"
categories: ["development"]
tags: ["hugo"]
---

Create a `custom.css` file to override the existing CSS rules in your current theme. You can name your CSS file whatever you like and have as many custom CSS files as you like. 

Update your `config.toml` file as follows: 

```toml
[params]
  customCss = ["css/custom.css"]
```

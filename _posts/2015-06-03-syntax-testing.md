---
layout: post
title: syntax testing
categories: []
tags: []
published: False

---

```javascript
params = {
  block: false,
  opacity: 60,
  color: "red",
  height: "70",
  width: "50",
  left: "100px",
  mousefocus: true,
  focus: true,
  move: true
}
Application('Inyo').html("~/projects/inyos/execclick.html", params, {timeout: 40000})
```

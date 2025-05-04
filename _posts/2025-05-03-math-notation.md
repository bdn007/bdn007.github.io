---
title: Mathematical Notations - is this not working?
description: Why some mathematical clearly rendered correctly, some others just don't?
date: 2025-05-03
categories: [math, query]
tags: [typography]
author: Cau

---

### The Problem

I found out that when adding even a single line to the index.html. 

```html
  <p>testing</p>
```

and then insert { { content } } into the `_layout/home.html`, the mathematical notations would be partly broken and won't render correctly.


![Screen shot](/assets/images/IMG_1761.jpeg){: width="300"}
_iPhone screenshot_


### The Solution

I found a workaround. Instead of adding html elements directly into the `index.html`, I created an `_includes/greeting.thml` file, then simply insert it into the `_layouts/home.thml` with `{ % include greeting.html % }.`

So far, it hasn't broken the MathJax syntax yet, so I am hopeful.

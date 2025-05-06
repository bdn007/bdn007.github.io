---
title: Mathematical Notations - is it not working?
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

and then insert { { content } } into the `_layout/home.html`, the mathematical notations would be partly broken and won't render correctly. It's noticed that even the same behaviour can be observed from the [theme demo itself](https://chirpy.cotes.page/posts/text-and-typography/)


![Screen shot](/assets/images/IMG_1761.jpeg){: width="300"}
_Here is a screenshot from iPhone_

![Screen shot](/assets/images/text_and_typo.png){: width="100%"}
_And here is another screenshot from my desktop, notice some errors?_



### The Solution

I found a workaround. Instead of adding html elements directly into the `index.html`, I created an `_includes/greeting.thml` file, then simply insert it into the `_layouts/home.thml` with `{ % include greeting.html % }.`

So far, it hasn't broken the MathJax syntax yet, so I am hopeful.

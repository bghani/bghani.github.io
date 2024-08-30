---
layout: post
title: blog
permalink: /blog/
nav: false
nav_order: 4
description: "This is a blog post page where I share articles with mathematical equations."
toc: false
categories: [math, blog]
tags: [math, equations]
date: 2024-08-30
math: true
---

## Your Blog Post Content

Welcome to my blog! This is where I share articles about mathematics.

### Example Math Equation

Here is an example of an inline equation: \( E = mc^2 \).

And here’s a block equation:

$$
\int_{a}^{b} x^2 dx
$$

You can start adding your articles here. Each new post will be its own file in the `_posts` directory.

---

### Converting the Page to a Blog Post Index

If you want this page to serve as an index of your blog posts, you can list them using Liquid templating:

```markdown
{% for post in site.posts %}
* [{{ post.title }}]({{ post.url }})
{% endfor %}

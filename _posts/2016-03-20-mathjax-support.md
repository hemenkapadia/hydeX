---
layout: post
title: hydeX adds MathJax support to Hyde
excerpt: MathJax is a powerful Javascript engine to display Math and Scientific symbols. This is an example content post to show MathJax integration in hydeX.
comments: true
tags:
  - hydeX
  - Features
  - MathJax 
  - HTML Content
---

[MathJax][1] is a state of art JavaScript engine to display mathematics and scientifc symbols on a web page. hydeX includes MathJax support by default. hydeX is configured to support [Tex and LaTeX][2] notation to enter math and scientification content in a blog post.

Both inline and block renderings are supported.

### Inline content

To display inline content, use `$ ... $` delimiters as shown below

```
When $a = f(x)$, there are two solutions to $ax^2 + bx + c = 0$ and they are
```

is rendered as 

When $a = f(x)$, there are two solutions to $ax^2 + bx + c = 0$ and they are


### Block content

For block content use the `$$ ..... $$` delimiters as shown below

```
$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$
```

is rendered as 

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

### LaTeX Reference.

I found the below links to be excellent reference for LaTeX symbols and code

* [LaTeX Wiki Book][3]
* [Detexify - Converts handwritten symbols to corresponding LaTeX code][4]
* [List of LaTeX symbols][5]


[1]: https://www.mathjax.org/
[2]: http://docs.mathjax.org/en/latest/start.html#tex-and-latex-input
[3]: https://en.wikibooks.org/wiki/LaTeX
[4]: http://detexify.kirelabs.org/classify.html
[5]: http://detexify.kirelabs.org/symbols.html
---
title: " "
numbering:
  code: true
  math: true
  headings: true
  heading_2: true
  heading_3: true
---

+++ { "part": "abstract" }

In this tutorial we take you on the journey from continuous equations to their discrete matrix representations using the finite volume method for the Direct Current (DC) resistivity problem. These techniques are widely applicable across geophysical simulation types and have their parallels in finite element and finite difference. We show derivations visually, as you would on a whiteboard, and have provided an accompanying notebook to explore the numerical results using [SimPEG](http://simpeg.xyz/).

+++

# 文章

In {sc}`MyST`, you {del}`should never` {u}`underline` _text_.

**strong**, _emphasis_, `literal text`, \*escaped symbols\*


## 脚注

- A footnote reference[^myref]

[^myref]: This is an auto-numbered footnote definition.

# 数式の活用

$$
y = \int f(x)dx
$$ (eq1)
{eq}`eq1`を引用

:::{prf:theorem}
:label: thm1
この定理はすばらしい

\begin{align*}
        \frac{\chi C_{t}}{1-N_{t}}&=(1-\alpha)A_{t}K_{t}^{\alpha}N_{t}^{-\alpha} \\
        \frac{1}{C_{t}}&=\mathbb{E}_{t}\left[\frac{\beta}{C_{t+1}}[\alpha A_{t+1}K_{t+1}^{\alpha-1}N_{t+1}^{1-\alpha}+1-\delta]\right] \\
        Y_{t}&=A_{t}K_{t}^{\alpha}N_{t}^{1-\alpha} \\
        w_{t}&=(1-\alpha)A_{t}K_{t}^{\alpha}N_{t}^{-\alpha} \\
        R_{kt}&=\alpha A_{t}K_{t}^{\alpha-1}N_{t}^{1-\alpha} \\
        Y_{t}&=C_{t}+K_{t}
\end{align*}


$$
    \begin{bmatrix}1 & 1 \\ 1 & 1\end{bmatrix}
$$

:::

# 図式

```{figure} images/logo.png
:width: 90%
:class: col-margin-right row-span-2
:name: logo

右側のグラフ
```

```{figure} https://cdn.curvenote.com/018f51bc-c742-7c34-a1a6-48bd86914cd8/public/862db6c25dd320d02cce6612464221d4.webp
:align: center
:name: fig1
この図の脚注
```
{ref}`fig1`を引用

# コード

```{code} julia
:filename: test.jl
:linenos:
:emphasize-lines: 1, 3

using LinearAlgebra
using Plots

x = 1:10
plot(x)
```

# 引用の仕方
[Vaswani et al. (2017)](https://doi.org/10.48550/arXiv.1706.03762)

<https://doi.org/10.48550/arXiv.1706.03762>

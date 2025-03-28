---
layout: post
title: Smoothness
categories: AG
---

# ⓪  前言

本文章参考了《An Invitation to Algebraic Geometry》的第五章。在该书中默认了是在域 $\mathbb{C}$
上操作的。所以未指明域时，均为 $\mathbb{C}$.

# ①  一点处的切空间

我们假设 $V$ 是 $\mathbb{A}^n$ 中包含原点的 Zariski 闭子集。我们来考虑 $\mathbb{A}^n$ 中的过原点的直线 $l=\{(t a_1,\dots,t a_n) | t\in \mathbb{C}\}$. 我们来考虑什么时候直线 $l$ 与 $V$ 在原点处相切？

设 $F_1,\dots, F_r$ 是 $\mathbb{I}(V)$ 的生成元。那么 $V$ 和 $l$ 的交点为以下方程组的根
$$
\begin{cases}
F_1(ta_1,\dots,ta_n)=0,\\
\ \ \ \ \enspace \enspace \ \vdots\\
F_r(ta_1,\dots,ta_n)=0
\end{cases}
$$
因为 $V$ 和 $l$ 都包含原点，所以 $0$ 是上面这个方程组的解。我们来定义 $V\cap l$ 在原点的重数为
$$
\min \{F_i(ta_1,\dots,ta_n)\ \text{在 $t=0$ 处的零点的重数}\ | i = 1,2,3,\dots, r\}
$$

**定义（相切）** 我们称直线 $l = \left(t(a_1 -p_1),t(a_2-p_2),\dots, t(a_n-p_n)\right)$ 和包含 $p=(p_1,\dots,p_n)$ 的 Zariski 闭子集 $V$ 在 $p$ 处相切，如果 $V\cap l$ 在 $p$ 处的重数为 $m>1$. 此时我们称 $l$ 与 $V$ 是 tangent of order $m-1$ 的。

**定义（$p$ 点处的切空间）** 我们将所有与 $V$ 在 $p$ 点处相切的直线上的点并起来得到一个空间 $T_pV$, 即 $$T_p V = \bigcup_{l\ \text{与 $V$ 在\ $p$\ 相切}} l$$

**例子** 设 $V= \mathbb{V}(y-x^2) \subseteq \mathbb{A}^2$, 我们来看零点处的切空间。设过零点的一条直线为 $l=(ta,tb),a,b\in \mathbb{C}$. $$tb = t^2 a^2.$$ 当 $b\neq 0$ 时, $V\cap l$ 在原点的重数为 $1$, 所以不相切。当 $b=0$ 时，$V\cap l$ 的重数为 $2$, 此时 $l$ 与 $V$ 相切。所以 $T_0V = x$ 轴.

![示意图](Images\Smooth6.2.png)

我们来看更多的例子。

**例子** 设 $V = \mathbb{V}(y^2-x^2-x^3)\subseteq \mathbb{A}^2$, 我们来研究其在原点处的切空间。设过原点的直线为 $l=(ta,ta),a,b\in \mathbb{C}$, $$ t^2 a^2 = t^2 b^2 +t^3b^3.$$ 所以 $V\cap l$ 在 $0$ 处的重数至少为 $2$. 因此任一条过原点的直线都与 $V$ 相切，$T_0V = \mathbb{A}^2$.

**定理** 设 $V = \mathbb{V}(F_1,\dots,F_r) \subseteq \mathbb{A}^n$, $p\in V$. 那么 $V$ 在 $p$ 点的切空间为 $$T_pV = \mathbb{V}\left( \mathrm{d}F_1(x-p),\dots,\mathrm{d}F_r(x-p) \right)$$
其中 $\mathrm{d}F_i(x-p)$ 为 $$\sum_{j=1}^r\frac{\partial F_i}{\partial x_j}(p)(x_j - p_j)$$.

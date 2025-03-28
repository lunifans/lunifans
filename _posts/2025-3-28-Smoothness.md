---
layout: post
title: Smoothness
categories: AG
---

# ⓪  前言

本文章参考了《An Invitation to Algebraic Geometry》的第五章。在该书中默认了是在域 $\mathbb{C}$
上操作的。所以未指明域时，均为 $\mathbb{C}$.

# ①  一点处的切空间

我们假设 $V$ 是 $\mathbb{A}^n$ 中包含原点的 Zariski 闭子集。我们来考虑 $\mathbb{A}^n$ 中的过原点的直线 $l=\{(t a_1,\dots,t a_n)|t\in \mathbb{C}\}$. 我们来考虑什么时候直线 $l$ 与 $V$ 在原点处相切？

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

\textbf{定义} 我们称直线 $l = \left(t(a_1 -p_1),t(a_2-p_2),\dots, t(a_n-p_n)\right)$ 和包含 $p=(p_1,\dots,p_n)$ 的 Zariski 闭子集 $V$ 在 $p$ 处相切，如果 $V\cap l$ 在 $p$ 处的重数为 $m>1$. 此时我们称 $l$ 与 $V$ 是 tangent of order $n-1$ 的。

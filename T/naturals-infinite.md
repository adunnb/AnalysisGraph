---
layout: proof
title: "The Natural Numbers Are Infinite"
chapter: "Set Theory and Functions"
link_terms: ["natural numbers are infinite"]
---

**Theorem:** The set $\mathbb{N}$ of [natural numbers](../D/natural-numbers) is infinite: it is not a [finite set](../D/finite-set).

**Proof:** Suppose instead that there is a [bijection](../D/bijective) $f : [n] \to \mathbb{N}$ for some $n \in \mathbb{N}_0$. Since $\mathbb{N}$ is nonempty, $n \geq 1$. The set $\{f(1), \ldots, f(n)\}$ is nonempty, finite, and [totally ordered](../D/total-order) by $\leq$, so it has a [greatest element](../D/greatest-element) $M$ by the theorem on [extrema of finite totally ordered sets](../T/finite-total-order). But $M + 1 \in \mathbb{N}$ and $M + 1 > f(i)$ for every $i$, so $M + 1$ is not in the [image](../D/image) of $f$. This contradicts the surjectivity of $f$.

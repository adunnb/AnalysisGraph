---
layout: proof
title: "Difference of Powers"
chapter: "The Natural Numbers"
link_terms: ["difference of powers"]
---

**Theorem:** For real numbers $a, b$ and every $n \in \mathbb{N}$:

$$a^n - b^n = (a - b) \sum_{j=0}^{n-1} a^{n-1-j} b^j = (a - b)(a^{n-1} + a^{n-2} b + \cdots + b^{n-1})$$

In particular, if $a$ and $b$ are integers with $a \neq b$, then $a - b$ divides $a^n - b^n$.

**Example:** $a^2 - b^2 = (a - b)(a + b)$ and $a^3 - b^3 = (a - b)(a^2 + ab + b^2)$. With $a = 5$, $b = 2$: $5^4 - 2^4 = 609 = 3 \cdot 203$.

**Remark:** The factorization holds for all real $a, b$; the divisibility statement only makes sense for integers. With $b = 1$ and $a = z$, dividing by $z - 1$ recovers the [finite geometric sum](../T/finite-geometric-sum).

**Proof:** We use [mathematical induction](../T/induction) on $n$. For $n = 1$ the identity reads $a - b = (a - b) \cdot 1$. Suppose it holds for $n = k$. Since:

$$a^{k+1} - b^{k+1} = a(a^k - b^k) + b^k(a - b)$$

substituting the induction hypothesis gives:

$$a^{k+1} - b^{k+1} = (a - b)\left(\sum_{j=0}^{k-1} a^{k-j} b^j + b^k\right) = (a - b) \sum_{j=0}^{k} a^{k-j} b^j$$

which is the identity for $n = k + 1$. When $a$ and $b$ are integers, the sum on the right is an integer, so $a - b$ divides $a^n - b^n$.

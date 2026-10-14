---
layout: proof
title: "Uncountability of the Power Set of ℕ"
chapter: "Set Theory and Functions"
link_terms: ["binary sequences", "binary sequence"]
---

**Theorem:** The [power set](../D/power-set) $\mathcal{P}(\mathbb{N})$ is [uncountable](../D/countable). Equivalently, the set of all infinite binary sequences $(b_1, b_2, b_3, \ldots)$ with each $b_n \in \{0, 1\}$ is uncountable.

**Example:** Here is the diagonal argument for binary sequences. Suppose the sequences were listed as rows; flipping each diagonal entry produces a sequence that differs from row $k$ in position $k$, so it is not in the list:

| | 1 | 2 | 3 | 4 | ⋯ |
|---|---|---|---|---|---|
| sequence 1 | **0** | 1 | 1 | 0 | ⋯ |
| sequence 2 | 1 | **1** | 0 | 0 | ⋯ |
| sequence 3 | 0 | 0 | **0** | 1 | ⋯ |
| sequence 4 | 1 | 0 | 1 | **1** | ⋯ |
| new sequence | 1 | 0 | 1 | 0 | ⋯ |

**Proof:** $\mathcal{P}(\mathbb{N})$ is infinite: $n \mapsto \{n\}$ is an [injection](../D/injective) $\mathbb{N} \to \mathcal{P}(\mathbb{N})$, so if $\mathcal{P}(\mathbb{N})$ were finite then $\mathbb{N}$ would be finite by the [counting rules](../T/counting-rules), contradicting the fact that [the natural numbers are infinite](../T/naturals-infinite). If $\mathcal{P}(\mathbb{N})$ were countable, it would therefore be denumerable, giving a [bijection](../D/bijective) $\mathbb{N} \to \mathcal{P}(\mathbb{N})$. This contradicts [Cantor's theorem](../T/cantor-theorem).

For binary sequences, send a [subset](../D/subset) $B \subseteq \mathbb{N}$ to its indicator sequence:

$$b_n = \begin{cases} 1 & \text{if } n \in B \\ 0 & \text{if } n \notin B \end{cases}$$

This is a bijection, with inverse $(b_n) \mapsto \{n : b_n = 1\}$. A set in bijection with an uncountable set is uncountable.

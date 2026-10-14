---
layout: proof
title: "Cantor's Theorem"
chapter: "Set Theory and Functions"
link_terms: ["Cantor's theorem"]
---

**Theorem:** For every [set](../D/set) $A$, there is no [surjection](../D/surjective) $A \to \mathcal{P}(A)$ onto its [power set](../D/power-set). In particular, $\operatorname{card}(A) < \operatorname{card}(\mathcal{P}(A))$: there is an [injection](../D/injective) $A \to \mathcal{P}(A)$ but no [bijection](../D/bijective).

**Remark:** This is the infinite analogue of the [finite count](../T/power-set-size) $\# \mathcal{P}(X) = 2^{\# X} > \# X$. The proof is a **diagonal argument**: against any proposed assignment $a \mapsto \varphi(a)$, the set $D$ below changes the answer to "does $a$ belong to its assigned [subset](../D/subset)?" at every $a$, so it differs from every assigned subset at that subset's own index. Applied to $A = \mathbb{N}$ it shows that [$\mathcal{P}(\mathbb{N})$ is uncountable](../T/power-set-uncountable).

**Proof:** Suppose that $\varphi : A \to \mathcal{P}(A)$ is surjective, and define:

$$D = \{a \in A : a \notin \varphi(a)\}$$

Since $D \subseteq A$, surjectivity gives $a_0 \in A$ with $\varphi(a_0) = D$. But then:

$$a_0 \in D \iff a_0 \notin \varphi(a_0) \iff a_0 \notin D$$

a contradiction. Hence no surjection $A \to \mathcal{P}(A)$ exists.

The map $a \mapsto \{a\}$ is an injection $A \to \mathcal{P}(A)$. There is no bijection, since a bijection would be a surjection.

---
layout: definition
title: "Partial Order"
chapter: "Set Theory and Functions"
link_terms: ["partial order", "partially ordered", "poset"]
---

**Definition:** A **partial order** on a [set](../D/set) $A$ is a [relation](../D/relation) $\preceq$ on $A$ that is reflexive, antisymmetric, and transitive:

1. $a \preceq a$ for every $a \in A$;
2. $a \preceq b$ and $b \preceq a$ imply $a = b$;
3. $a \preceq b$ and $b \preceq c$ imply $a \preceq c$.

The pair $(A, \preceq)$ is a **partially ordered set**, or **poset**. We write $a \prec b$ when $a \preceq b$ and $a \neq b$. Two elements $a, b$ are **comparable** if $a \preceq b$ or $b \preceq a$.

**Example:** The usual $\leq$ is a partial order on $\mathbb{N}$, $\mathbb{Z}$, $\mathbb{Q}$, and $\mathbb{R}$. The strict relation $<$ is not, because $a < a$ is false.

**Example:** For any set $X$, [inclusion](../D/subset) $\subseteq$ is a partial order on the [power set](../D/power-set) $\mathcal{P}(X)$. Reflexivity and transitivity follow from the definition of a subset, and antisymmetry is the two-inclusion criterion for set equality.

**Example:** Divisibility is a partial order on $\mathbb{N}$: $a \preceq b$ when $b = ka$ for some $k \in \mathbb{N}$. For antisymmetry, if $b = ka$ and $a = \ell b$ with $k, \ell \in \mathbb{N}$, then $k\ell = 1$, so $k = \ell = 1$ and $a = b$.

**Remark:** Before calling a comparison an order, check the axioms. Comparing natural numbers by their remainders mod $3$, or comparing sets by their areas, fails antisymmetry: distinct objects can tie. In a partial order, two elements need not be comparable; when every pair is, the order is a [total order](../D/total-order).

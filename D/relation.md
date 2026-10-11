---
layout: definition
title: "Relation"
chapter: "Set Theory and Functions"
link_terms: ["binary relation", "relation", "reflexive", "symmetric", "antisymmetric", "transitive"]
---

**Definition:** A **binary relation** on a [set](../D/set) $A$ is a [subset](../D/subset) $R$ of the [Cartesian product](../D/cartesian-product) $A \times A$. We write $a \mathrel{R} b$ when $(a, b) \in R$.

A relation $R$ on $A$ is:

1. **reflexive** if $a \mathrel{R} a$ for every $a \in A$;
2. **symmetric** if $a \mathrel{R} b$ implies $b \mathrel{R} a$;
3. **antisymmetric** if $a \mathrel{R} b$ and $b \mathrel{R} a$ imply $a = b$;
4. **transitive** if $a \mathrel{R} b$ and $b \mathrel{R} c$ imply $a \mathrel{R} c$.

**Example:** On $\mathbb{R}$, the relation $\leq$ is reflexive, antisymmetric, and transitive, but not symmetric. The relation $<$ is transitive but neither reflexive nor symmetric. Equality is reflexive, symmetric, antisymmetric, and transitive.

**Example:** On $\mathbb{N}$, the relation "$a \mathrel{R} b$ when $a \bmod 3 \leq b \bmod 3$" is reflexive and transitive but not antisymmetric: $1 \mathrel{R} 7$ and $7 \mathrel{R} 1$, although $1 \neq 7$.

**Remark:** The two most important kinds of relations combine these properties: a [partial order](../D/partial-order) is reflexive, antisymmetric, and transitive, and an [equivalence relation](../D/equivalence-relation) is reflexive, symmetric, and transitive.

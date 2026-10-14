---
layout: definition
title: "Countable and Uncountable Sets"
chapter: "Set Theory and Functions"
link_terms: ["countable", "uncountable", "denumerable", "countably infinite"]
---

**Definition:** A [set](../D/set) $A$ is **denumerable** (or **countably infinite**) if it has the same [cardinality](../D/cardinality) as $\mathbb{N}$. It is **countable** if it is [finite](../D/finite-set) or denumerable, and **uncountable** if it is not countable.

**Example:** The map $n \mapsto 2n$ is a [bijection](../D/bijective) from $\mathbb{N}$ onto the even natural numbers $\{2, 4, 6, \ldots\}$, so that set is denumerable. The integers and the rationals are also denumerable ([The integers are countable](../T/integers-countable)), while the [power set](../D/power-set) of $\mathbb{N}$ is uncountable ([Uncountability of the power set of ℕ](../T/power-set-uncountable)).

**Remark:** A bijection $n \mapsto a_n$ from $\mathbb{N}$ onto $A$ is the same thing as a list $A = \{a_1, a_2, a_3, \ldots\}$ in which every element appears exactly once. Such a list also orders $A$: put $a_i \preceq a_j$ when $i \leq j$. This is a [total order](../D/total-order) induced by the enumeration, not necessarily one already present on $A$. Some books use "countable" to mean denumerable; here finite sets count as countable.

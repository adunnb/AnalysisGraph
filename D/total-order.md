---
layout: definition
title: "Total Order"
chapter: "Set Theory and Functions"
link_terms: ["total order", "totally ordered", "linear order", "comparable"]
---

**Definition:** A **total order** (or **linear order**) on a set $A$ is a [partial order](../D/partial-order) $\preceq$ in which every two elements are comparable: for all $a, b \in A$, $a \preceq b$ or $b \preceq a$. The pair $(A, \preceq)$ is then a **totally ordered set**.

**Example:** The usual $\leq$ is a total order on $\mathbb{N}$, $\mathbb{Z}$, $\mathbb{Q}$, and $\mathbb{R}$.

**Example (lexicographic order):** On $\mathbb{N} \times \mathbb{N}$, define:

$$(a, b) \preceq_{\text{lex}} (c, d) \iff a < c \text{ or } (a = c \text{ and } b \leq d)$$

First coordinates are compared first, and second coordinates break ties; for example $(1, 2) \prec_{\text{lex}} (3, 1)$ and $(1, 2) \prec_{\text{lex}} (1, 3)$. This is a total order. Reflexivity is clear. If each of two pairs precedes the other, their first coordinates agree and then their second coordinates agree, which gives antisymmetry. For transitivity, if $(a, b) \preceq_{\text{lex}} (c, d) \preceq_{\text{lex}} (e, h)$ then $a \leq c \leq e$; if $a < e$ we are done, and if $a = e$ then $a = c = e$ and $b \leq d \leq h$. Any two pairs are comparable by comparing first coordinates, then second. Dictionary order on words is the same idea.

**Example:** Inclusion on $\mathcal{P}(X)$ is not total once $X$ has two elements: $\{1, 2, 3\}$ and $\{1, 2, 4\}$ are incomparable, since $3 \notin \{1, 2, 4\}$ and $4 \notin \{1, 2, 3\}$. Divisibility on $\mathbb{N}$ is not total either: neither $2$ divides $3$ nor $3$ divides $2$.

**Remark:** In a total order, the notions of [maximal and greatest element](../T/total-order-maximal) coincide.

---
layout: proof
title: "Schröder–Bernstein Theorem"
chapter: "Set Theory and Functions"
link_terms: ["Schröder–Bernstein", "Schröder-Bernstein", "Cantor–Bernstein"]
---

**Theorem:** If there are [injections](../D/injective) $f : A \to B$ and $g : B \to A$, then there is a [bijection](../D/bijective) $h : A \to B$. In terms of [cardinality](../D/cardinality): if $\operatorname{card}(A) \leq \operatorname{card}(B)$ and $\operatorname{card}(B) \leq \operatorname{card}(A)$, then $A \sim B$.

**Remark:** The two injections need not be inverses of each other; the bijection is built from pieces of both. The idea is to trace each point of $A$ backward along the arrows $\cdots \xrightarrow{g} a \xrightarrow{f} \cdots$, using the unique [preimages](../D/preimage) under $g$ and $f$ whenever they exist. The backward chain from $a$ either stops at a point of $A \setminus g(B)$, stops at a point of $B \setminus f(A)$, or never stops (which includes cycles). Use $f$ on the chains that start in $A$ and $g^{-1}$ on all the others. As an application, injections $\mathbb{N} \to \mathbb{Q}$ and $\mathbb{Q} \to \mathbb{N}$ show that $\mathbb{Q}$ is [denumerable](../D/countable).

**Proof:** Define sets $C_n \subseteq A$ by:

$$C_0 = A \setminus g(B), \qquad C_{n+1} = g(f(C_n)) \quad (n \in \mathbb{N}_0), \qquad C = \bigcup_{n=0}^{\infty} C_n$$

so $C$ consists of the points reached from $A \setminus g(B)$ by applying $g \circ f$ finitely many times. Two consequences of the definition will be used:

$$C = C_0 \cup g(f(C)), \qquad A \setminus C \subseteq g(B)$$

The first follows by separating $C_0$ from the terms with $n \geq 1$; the second because $C$ contains every point outside $g(B)$. Define:

$$h(a) = \begin{cases} f(a) & \text{if } a \in C \\ g^{-1}(a) & \text{if } a \in A \setminus C \end{cases}$$

*Well defined.* If $a \notin C$ then $a \in g(B)$, and since $g$ is injective, $g^{-1}(a)$ is a single point of $B$.

*Injective.* On $C$, $h = f$ is injective, and on $A \setminus C$, $h = g^{-1}$ is injective. Suppose $a \in C$, $a' \notin C$, and $h(a) = h(a')$. Then $f(a) = g^{-1}(a')$, so $a' = g(f(a)) \in g(f(C)) \subseteq C$, a contradiction.

*[Surjective](../D/surjective).* Let $b \in B$. If $b \in f(C)$, then $b = f(a) = h(a)$ for some $a \in C$. Otherwise, put $a = g(b)$. If $a$ were in $C$, then $a \notin C_0$ (since $a \in g(B)$), so $a = g(f(c))$ for some $c \in C$; injectivity of $g$ would give $b = f(c) \in f(C)$, a contradiction. So $a \notin C$, and $h(a) = g^{-1}(g(b)) = b$.

Therefore $h$ is a bijection.

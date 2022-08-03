---
layout: post
title: Mathcamp Essences in OSU (in progress)
tags: [Math, Economics]
usemathjax: true
---

Here, I will list up important definitions and theorems that must be remembered, and objects or properties that was hard for me to understand. So, the materials covered in this page may be rather subjective and does not follow the materials of the mathcamp in OSU as a whole. I will add subjects that is from other texts such as "Mathematics for Economists" (Simon & Blume) or "Principles of Mathematical Analysis" (Walter Rudin). Moreover, to modify the definitions and theorems to be easily remembered, I will actively use abbreviation of notations.

# Set and Logic

- Even subsets are defined in elements.

$$Definition\: (subset) \: A: \text{subset of }X \text{ if } ∀x∈A,\:x∈X.$$

- Thus we can say that two sets are equal if all the elements of the two coincides.

$$Definition\: A=B⇔A⊆B\&B⊆A\text{, i.e., }\forall x\in A, \:x\in B\: \& \:\forall y\in B,\: y\in A.$$


$$Definition\: (power set)\:P\left(X\right) \text{(the power set of }X):=\{A_{i}:A_{i}\subseteq X\}$$

- Then, the number of elements--the power set has sets as elements--in the power set of $$X$$: $$n\left(P\left(X\right)\right)=2^{n\left(X\right)}$$, since it is the same as the number of cases of checking whether each element in $$X$$ is present or not.
- Also, from the reasoning above, we can see that empty set is also an element of the power set, as no elements being present is contained in the cases.

$$Definition\: (union)\: A\cup B:=\{x\in A\:\text{ or }x\in B\}$$

$$Definition\: (intersection)\: A\cap B:=\{x\in A\:\text{ and }x\in B\}$$

$$Theorem\: (Commutative,\: Associative,\: Distributive\:Law)\:$$
(1) Commutative Law: $$A\cup B=B\cup A$$ and $$A\cap B=B\cap A$$

(2) Associative Law: 

$$(A\cup B)\cup C=A\cup(B\cup C)=A\cup B\cup C$$

$$(A\cap B)\cap C=A\cap(B\cap C)=A\cap B\cap C$$

(3) Distributive Law:

$$(A\cup B)\cap C=(A\cap C)\cup(B\cap C)$$

$$(A\cap B)\cup C=(A\cup C)\cap(B\cup C)$$

$$Definition\: (disjoint)\: A\text{ and }B\text{ are disjoint if }A\cap B=\phi.$$

$$Definition\: (pairwise\: disjoint)\: \text{A family of sets}, \:\{A_{i},\:i=1,\dots,n\},\text{ is pairwise disjoint if }\forall i\neq j, \:i,j=1,\dots,n,\: A_{i}\cap A_{j}=\phi.$$

- Pairwise disjoint means a class of sets does not overlap each other.
- From now on, I will use $$i\in I$$, instead of using $$i=1,\dots,n$$.

$$Definition\: (partition)\:\text{A family of sets },\{A_{i}\subseteq X,\:i\in I\},\text{ is a partition of }A\text{ if }\forall i\neq j\in I,\:A_{i}\cap A_{j}=\phi\:\&\:\cup_{i\in I}A_{i}=X.$$

- So, a partition of a set is a class of sets that constitute the set but does not overlap each other.



# Relation and Function


# Vector Space, Metric Space, Limit, and Continuity


# Vector Subspace and Affine Subspace


# Convexity and Seperating Hyperplane



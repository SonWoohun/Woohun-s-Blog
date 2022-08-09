---
layout: post
title: Mathcamp Essences in OSU (in progress)
tags: [Math, Economics]
usemathjax: true
---

Here, I will list up important definitions and theorems that must be remembered, and objects or properties that was hard for me to understand. So, the materials covered in this page may be rather subjective and does not follow the materials of the mathcamp in OSU as a whole. I will add subjects that is from other texts such as "Mathematics for Economists" (Simon & Blume) or "Principles of Mathematical Analysis" (Walter Rudin). Moreover, to modify the definitions and theorems to be easily remembered, I will actively use abbreviation of notations.

# Set and Logic

- Even subsets are defined in elements.

$$Definition1\: (subset) \: A: \text{subset of }X \text{ if } ∀x∈A,\:x∈X.$$

- Thus we can say that two sets are equal if all the elements of the two coincides.

$$Definition2\: A=B⇔A⊆B\&B⊆A\text{, i.e., }\forall x\in A, \:x\in B\: \& \:\forall y\in B,\: y\in A.$$


$$Definition3\: (power set)\:P\left(X\right) \text{(the power set of }X):=\{A_{i}:A_{i}\subseteq X\}$$

- Then, the number of elements--the power set has sets as elements--in the power set of $$X$$: $$n\left(P\left(X\right)\right)=2^{n\left(X\right)}$$, since it is the same as the number of cases of checking whether each element in $$X$$ is present or not.
- Also, from the reasoning above, we can see that empty set is also an element of the power set, as no elements being present is contained in the cases.

$$Definition4\: (union)\: A\cup B:=\{x\in A\:\text{ or }x\in B\}$$

$$Definition5\: (intersection)\: A\cap B:=\{x\in A\:\text{ and }x\in B\}$$

$$Theorem1\: (Commutative,\: Associative,\: Distributive\:Law)\:$$

(1) Commutative Law: $$A\cup B=B\cup A$$ and $$A\cap B=B\cap A$$

(2) Associative Law: 

$$(A\cup B)\cup C=A\cup(B\cup C)=A\cup B\cup C$$

$$(A\cap B)\cap C=A\cap(B\cap C)=A\cap B\cap C$$

(3) Distributive Law:

$$(A\cup B)\cap C=(A\cap C)\cup(B\cap C)$$

$$(A\cap B)\cup C=(A\cup C)\cap(B\cup C)$$

$$Definition6\: (disjoint)\: A\text{ and }B\text{ are disjoint if }A\cap B=\phi.$$

$$Definition7\: (pairwise\: disjoint)$$
A family of sets, $$\{A_{i},\:i=1,\dots,n\}$$, is pairwise disjoint if $$\forall i\neq j, \:i,j=1,\dots,n,\: A_{i}\cap A_{j}=\phi.$$

- Pairwise disjoint means a class of sets does not overlap each other.
- From now on, I will use $$i\in I$$, instead of using $$i=1,\dots,n$$.

$$Definition8\: (partition)$$
A family of sets $$\{A_{i}\subseteq X,\:i\in I\}$$, is a partition of $$A$$ if $$\forall i\neq j\in I,\:A_{i}\cap A_{j}=\phi\:\&\:\cup_{i\in I}A_{i}=X.$$

- So, a partition of a set is a class of sets that constitute the set but does not overlap each other.



# Relation and Function


# Vector Space, Metric Space, Limit, and Continuity

$$Definition1\: (Field)$$

A $$field$$ is a set $$F$$ with two operations : $$addition$$ and $$multiplication$$ $$s.t.$$ satisfies the following axioms.

(A : Addition) $$∀x,y,z∈F$$

1. $$x+y∈F$$ (Closed)
2. $$x+y=y+x$$ (Commutativity)
3. $$(x+y)+z=x+(y+z)$$ (Associativity)
4. $$∃0∈F\:s.t.\:0+x=x$$ (Existence of additive identity)
5. $$∃(-x)∈F\:s.t.\:x+(-x)=0$$ (Existence of inverse element)

(M: Multiplication) $$∀x,y,z∈F$$

1. $$xy∈F$$ (Closed)
2. $$xy=yx$$ (Commutativity)
3. $$x(yz)=(xy)z$$ (Associativity)
4. $$∃1∈F\:s.t.\:1≠0,\:and\:1×x=x$$ (Existence of multiplicative identity)
5. $$∀x∈F\:s.t.\:x≠0,\:∃\frac{1}{x}∈F\:s.t.\:x×\frac{1}{x}=1$$ (Existence of inverse element)

(D : The distributive law) $$∀x,y,z∈F$$

$$(x+y)×z=x×z+y×z$$


$$Definition2\: (Vector Space)$$ 

A vector space defined over a field $$F$$ is a set $$V$$ of elements called vectors, with (1) a binary operation $$V\times V→V$$ called **vector addition**, and (2) an operator $$F\times V→V$$ called a **scalar multiplication**.

- The two operations of vector space have the following properties.

(1) $$V$$: closed under vector addition, and $$∀x,y,z\in V$$, we have the following:

1. Associative : $$x+(y+z)=(x+y)+z=x+y+z$$
2. Commutative : $$x+y=y+x$$
3. Existence of the additive identity : $$∃! \underline{0} ∈V:\:x+\underline{0}=\underline{0}+x=x$$
4. Existence of inverse elements: $$∀x\in V,\:\exists!(-x)\in V\: : \: x+(-x)=(-x)+x=\underline{0}.$$

(2) $$V$$ : closed under scalar multiplication, and $$∀x,y∈V$$ and $$∀α,β∈F$$, we have the following:

1. Double distributive property: $$α(x+y)=αx+αy$$ and $$(α+β)x=αx+βy$$
2. Associative law for scalars: $$α(βx)=(αβ)x$$
3. Existence of a multiplicative identity: $$\exists!1∈F:\:1x=x$$

$$Definition3\: (Metric \:or\: distance\: function)$$
$$d:\:X×X→\mathbb{R}_{+}\:s.t.\:∀x,y,z∈X,$$

1. $$d(x,y)≥0$$ (nonnegativity) and $$d\left(x,y\right)=0⇔x=y$$ (asymmetry)
2. $$d(x,y)=d(y,x)$$ (commutativity)
3. $$d(x,z)≤d(x,y)+d(y,z)$$ (triangular inequality)

$$Definition4\: (Metric Space)$$
A metric space is a pair $$(X,d)$$ where $$X$$: a set, $$d$$: a metric defined on $$X$$.

$$Definition5\: (Norm)$$
Let $$V$$: a vector space, $$X$$: the underlying set of points. Then $$\|⋅\|:\:X→\mathbb{R}$$ is called a **norm** if it satisfies the following properties $$∀x,y∈X $$,$$∀α∈\mathbb{R}$$:

1. non-negativity: $$\|x\|≥0$$
2. only the zero vector has zero norm: $$\|x\|=0⇔x=0$$
3. triangular inequality: $$\|x+y\|≤\|x\|+\|y\|$$
4. scalar multiplication: $$\|αx\|= \lvert α\rvert \|x\|$$

$$Definition6\:(Normed\: vector\: space)$$

A normed vector space is a vector space $$V$$ equipped with norm.

$$Theorem 1$$
For $$∀x,y∈V,\: d(x,y)=\|x-y\|$$ is a metric.

$$proof$$

1. (non-negativity&asymmetry) $$\|x-y\|≥0$$ and $$\|x-y\|=0⇔x=y$$ by the 1. and 2. of $$Def5$$.
2. (commutativity) $$\|x-y\|= \lvert -1\rvert \|y-x\|=\|y-x\|$$ by the 4. in $$Def5$$.
3. (triangular inequality) $$∀x,y,z∈V,\|x-z\|+\|z-y\|≥\|x-y\|$$ by 3. in $$Def5$$.

$$Definition7\:(Euclidean \:space)$$ 

The $$n$$-dimensional **Euclidean space** is a normed vector space, $$E^{n}\left(\mathbb{R}^{n},d_{E}\right)$$, where $$d_{E}(x,y)=\|x-y\|_{E}=\sqrt{∑_{i=1}^{n}(x_{i}-y_{i})^{2}}$$

# Vector Subspace and Affine Subspace


# Convexity and Seperating Hyperplane


# Differential Calculus



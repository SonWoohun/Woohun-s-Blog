---
layout: post
title: Logit Formula Derivations
tags: [Economics, Econometrics, Discrete Choice Model]
usemathjax: true
---

# Settings

Let a decision maker with index $i$ is facing $J$ alternatives. The utility from a good $j$ is $v_{ij}$ which consists of two components, (1) part that is known up to parameter, $u_{ij}$, and (2) part that is unknown (error term), $ɛ_{ij}$.

-$v_{ij}=u_{ij}+ɛ_{ij}$ for $\forall i=1,\dots,N$, $\forall j=1,\dots,J$.

Now to make the model into a logit model, we have to assume that each error terms independently and identically follow Gumbel distribution (type 1 extreme value distribution (EV $I$)). It has a pdf of $f(ɛ_{ij})=$ Since Gumbel distribution is not symmetric and mean is not zero, it is sometimes cumbersome to explain what this kind of error structure implies. Although the problem of interpretation of error terms persists, what is important is the difference between the utility since this is the discrete choice model. We go over to the next stage of distribution of the difference between the two error terms, a logistic (logit) distribution.


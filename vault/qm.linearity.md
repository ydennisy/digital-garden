---
id: cb948322-0cc9-47d9-b0f5-a4b23b8248de
title: Linearity
desc: ''
updated: 1614535848748
created: 1614532372564
---

# Linearity

**Quantum mechanics is linear, while classic mechanics can be non-linear.**

QM has the property of **linearity**, similarly to Maxwell's theory of electromagnetism. This implies that if we have a solution, for example for Maxwell's equations which is:

$$
(E, B, \rho, J)
$$

Then we can multiply by a real valued constant $\alpha \in \R$, to get:

$$
(\alpha E, \alpha B, \alpha\rho, \alphaJ)
$$

Which will also be a solution. Linearity also implies that if we have two solutions:

$$
(E_1, B_1, \rho_1, J_1) and (E_2, B_2, \rho_2, J_2)
$$

Then the **sum** of the two solutions is also a valid solution:

$$
(E_1 + E_2, B_1 + B_2, \rho_1 + \rho_2, J_1 + J_2)
$$

This new solution can actually be called the **superposition** of the two original solutions. This also means that for a single equation / theory there are many solutions and is related to how a translantic cable can pass millions of simulatneous data streams, without them interferring with each other. 

## The general case

In the following equation

$$
Lu = 0
$$

We have $L$ which is the **linear operator** and $u$ which represents an **unknown**, this could be a number or function of time, space or even many of both.

The linear operator is an object which satisfies the following two properties from the example above

$$
L(u_1 + u_2) = Lu_1 + Lu_2, L(au) = aLu,
$$

where $a$ is a number. The two conditions imply they can be combined

$$
L(\alpha u_1 _ \beta u_2) = \alpha L u_1 + \beta L u_2
$$

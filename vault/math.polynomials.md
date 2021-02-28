---
id: fb74c8b5-7584-4d20-b5c2-1445e527f9a7
title: Polynomials
desc: ''
updated: 1609614036581
created: 1609607816322
---

# Polynomials

#### Definition

A single variable polynomial with real coefficients is a function $f$ that takes a real number as input and produces a real number as output and has the form

```math
f(x) = a_0 + a_1x + a_2x^2 + ... + a_nx^n
```

where $a_i$ are real numbers. The $a_i$ are called _coefficients_ of $f$. The _degree_ of the polynomial is the integer $n$.

Syntax:

- a polynomial with real coefficients (the function $f$).
- coefficients (the numbers $a_i$).
- a polynomial's degree (the integer $n$).

Example:

```math
g(t) = 2 + 0t + 4t^2 + (-1)t^3
```

Which can be written as

```math
g(t) = 2 + 4t^2 - t^3
```

And can be evaluated for $t = 3$

```math
g(3) = 2 + 4(3^2) - 3^3 = 11
```

Interesting ways to think about polynomials:
- a polynomial as with any function can be represented as a set of pairs called _points_. That is if you take each input $t$ and pair it with its output $f(t)$ you get a set of tuples $(t, f(t))$, which can be analysed from the perspective of set theory.
- a polynomial's graph can be plotted as a curve in space, so that the horizontal direction represents the input and the vertical the output.
- using the curves they "carve out" we can regard a polynomial as a geometric object, with properties like "curvature" and "smoothness".
- any logical condition can be expressed as a combination of polynomials if we restrict their inpot to $1$ or $0$:

```math
AND(x,y) = xy \\
NOT(x) = 1 - x \\
OR(x,y) = 1 - (1-x)(1-y)
```

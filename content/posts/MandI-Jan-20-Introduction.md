---
author: "Samuel Lam"
title: "M&I Week 3 - Introduction"
categories: ["outreach", "M&I"]
tags: ["announcement"]
ShowToc: true
TocOpen: true
date: 2022-01-20T09:07:47+08:00
draft: false
---

# Follow up of lectures
- Formalisation of Riemann (Darboux) Integral: the upper and lower Darboux sum is defined as

$$U(f) = \inf_\mathcal{P} U(f,\mathcal{P}), \quad L(f) = \sup_\mathcal{P} L(f,\mathcal{P})$$
where

$$U(f,\mathcal{P} = (x_i)_{i=0}^n) = \sum _{i=0}^{n-1} \left( \sup _{x \in [x_i, x _{i+1})} f(x) \right) (x _{i+1} - x_i)$$

$$L(f,\mathcal{P} = (x_i)_{i=0}^n) = \sum _{i=0}^{n-1} \left( \inf _{x \in [x_i, x _{i+1})} f(x) \right) (x _{i+1} - x_i)$$

- Incompleteness of $L^p$ space induced by Riemann Integral, e.g. consider $(q_i)_{i\geq 1}$ being an enumeration of $\mathbb{Q} \cap [0,1]$ and consider the sequence 

$$f_n(x) = \mathbb{I}_{q_1,..,q_n}(x)$$ 

Then $f_n(x) \to f(x) = \mathbb{I}_\mathbb{Q}$ is Cauchy in Riemann $L^1$ seminorm but does not converge in Riemann $L^1$. The Riemann $L^1$ norm is defined as

$$\lVert f \rVert = \int_0^1 |f(x)| \, dx$$

- The Riemann $L^1$ seminorm is not a norm because it is not *positive definite*. To solve this we consider the quotient space by equivalence relation $f \sim g = \int_0^1 |f-g| \, dx = 0$.

- Probability Theory: Often we want to construct independent random variable $X_i : (\Omega_i, \mathcal{F}_i, \mathbb{P}_i) \to (\mathbb{R}, \mathcal{B}(\mathbb{R}))$ and perform manipulations like $S_n = \sum _{i=1}^n X_n$. But the expression does not make sense since the domain of $X_i$ are not the same. To resolve this, we define the map $S_n$ on a larger *ambient space* 

$$(\Omega, \mathcal{F}) = (\Omega_i, \mathcal{F} _ i)^{\otimes \mathbb{N}} := \bigotimes_{i\geq 1} (\Omega_i, \mathcal{F}_i) = (\Omega_1, \mathcal{F}_1) \times (\Omega_2, \mathcal{F}_2) \times ...$$
and 

$$S_n(\omega_1, \omega_2, ...) = \sum _{i=1}^n X_i(\omega_i)$$

Natural questions to ask:
- How can we construct $\mathcal{F}$ so that $(\Omega, \mathcal{F})$ is a measurable space (here $\Omega = \otimes _{i\geq1} \Omega _ i$)
- What probability measure $\mathbb{P}$ should this measurable space equip? Ideally we should informally have
$$ \mathbb{P}(A_1 \times A_2 \times ...) = \mathbb{P}(A_1) \times \mathbb{P}(A_2) \times ...$$
Moreover, is there a way to *construct* this measure?

See **Kolmogorov Extension Theorem** for more information.

# Additional Preparation: Function space
Fix a closed and bounded interval $[a,b]$, then the set of all functions on $[a,b]$ is a vector space. We would like to consider its vector subspaces for which a norm can be defined (these are called *normed*-vector space). A norm of a vector space $V$ on $\mathbb{R}$ or $\mathbb{C}$ is a function $\lVert. \rVert$ such that it satisfies the following properties:
1. (Non-negativity) $\lVert x \rVert \geq 0$ for all $x \in V$. 
2. (Homogeneity) for all scalar $\lambda$ we have $\lVert \lambda x \rVert = |\lambda| \lVert x \rVert$
3. (Triangle Inequality) $\lVert x+y \rVert \leq \lVert x \rVert + \lVert y \rVert$
4. (Positive Definiteness) $\lVert x \rVert = 0 \iff x = 0$

A seminorm is a function $\lVert . \rVert$ satisfying axioms 1-3 but not 4.

We have discussed a few spaces (sets):
- Space of all bounded function $B([a,b])$. This is a closed vector subspace with norm $\lVert f \rVert_\infty = \sup _{x \in [a,b]} |f(x)|$. This is often called a *supremum*-norm.
- Space of all continuous function $C^0([a,b])$. This is a closed vector subspace of $B([a,b])$ with the supremum norm.
- Space of all Riemann $L^p$ integrable functions $\mathcal{R}-L^p([a,b])$, with seminorm
$$
\|f\|_{\mathcal{R}-L^p} = \left( \int_a^b |f(x)|\, dx \right)^{1/p}
$$

A normed vector space is *complete* (Banach) if all Cauchy sequences of elements converge to another element in that normed vector space. We know that $\mathbb{R}^n$, $B([a,b])$ and $C^0([a,b])$ are Banach, but $\mathcal{R}-L^p([a,b])$ is not Banach (but the Lebesgue $L^p$ space is Banach).

# Exercises

**Core**

1. Make sure you have reviewed the notion of $\sigma$-algebra, pre-measure, measure and outer measure. Also make sure you are happy with the basic properties of measure (e.g. upper/lower continuity).
2. Preview notions of *open* and *closed* sets in Analysis I. In particular establish that the uncountable union of open set is open and uncountable intersection of closed set is closed.

**Function Spaces**

3. You will learn about uniform convergence of functions. Try to write the definition of uniform convergence of functions using the supremum norm.
4. Let $V$ be a vector space with seminorm $\lVert . \rVert_V$. Define the equivalence relation $f \sim g$ iff $\lVert f-g \rVert_V = 0$. Now consider the quotient space $V/\sim$ (i.e. set of all equivalent classes). Show that $V/\sim$ is also a vector space (under suitable definitions of addition and scalar multiplication). Now define for all equivalent classes $[f]_\sim \in V/\sim$,

$$\lVert [f] _\sim \rVert _ {V/\sim} = \lVert f \rVert _V$$

Show that the function $\lVert .\rVert _{V/\sim}$ is well-defined (i.e. if we choose two functions $f,g$ from $[f] _\sim$ then the value of norm remains unchanged). Now show that $\lVert .\rVert _{V/\sim}$ is a norm of $V/\sim$.
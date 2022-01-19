---
author: "Samuel Lam"
title: "Measure and Integration Study Group"
categories: ["academic"]
tags: ["announcement"]
ShowToc: true
TocOpen: true
date: 2022-01-19T10:10:07+08:00
draft: true
mathjax: true
---

# Objective
This is a trial study group as a follow up of the lectures of the course [MATH50006 Lebesgue Measure and Integration](https://imperialmathswiki.com/en/2nd_year/MATH50006_Lebesgue_Measure_and_Integration) (Imperial login required.)

# Logistics
Venue: Math Learning Centre (MLC, Huxley 414), Huxley Building, Imperial
Time: *9.30am - 11.00am* every Wednesday.
Content: discussion of materials from the Tuesday lecture.
Materials: See the relevant [*MathWiki page*](https://imperialmathswiki.com/en/2nd_year/MATH50006_Lebesgue_Measure_and_Integration). (Imperial login required.)

# Timetable
## 19/1 - Introduction
### Follow up of lectures
- Formalisation of Riemann (Darboux) Integral: the upper and lower Darboux sum is defined as

$$U(f) = \inf_\mathcal{P} U(f,\mathcal{P}), \quad L(f) = \sup_\mathcal{P} L(f,\mathcal{P})$$
where

$$U(f,\mathcal{P} = (x_i)_{i=0}^n) = \sum_{i=0}^{n-1} \left( \sup_{x \in [x_i, x_{i+1})} f(x) \right) (x_{i+1}-x_i$$

$$L(f,\mathcal{P} = (x_i)_{i=0}^n) = \sum_{i=0}^{n-1} \left( \inf_{x \in [x_i, x_{i+1})} f(x) \right) (x_{i+1}-x_i$$

- Incompleteness of $L^p$ space induced by Riemann Integral, e.g. consider $(q_i)_{i\geq 1}$ being an enumeration of $\mathbb{Q} \cap [0,1]$ and consider the sequence $f_n(x) = \mathbb{I}_{q_1,..,q_n}$. Then $f_n(x) \to f(x) = \mathbb{I}_\mathbb{Q}$ is Cauchy in Riemann $L^1$ seminorm but does not converge in Riemann $L^1$. The Riemann $L^1$ for is defined as
$$\|f\| = \int_0^1 |f(x)| \, dx$$

- The Riemann $L^1$ seminorm is not a norm because it is not *positive definite*. To solve this we consider the quotient space by equivalence relation $f \sim g = \int_0^1 |f-g| \, dx = 0$.

- Probability Theory: Often we want to construct independent random variable $X_i : (\Omega_i, \mathcal{F}_i, \mathbb{P}_i) \to (\mathbb{R}, \mathcal{B}(\mathbb{R}))$ and perform manipulation like $S_n = \sum_{i=1}^n X_n$. But the expression does not make sense since the domain of $X_i$ are not the same. To resolve this, we define the map $S_n$ on a larger *ambient space* 

$$(\Omega, \mathcal{F}) = (\Omega_i, \mathcal{F})^{\otimes \mathbb{N}} := \bigotimes_{i}\geq 1(\Omega_i, \mathcal{F}_i) (\Omega_1, \mathcal{F}_1) \times (\Omega_2, \mathcal{F}_2) \times ...$$

and 

$$S_n(\omega_1, \omega_2, ...) = \sum_{i=1}^n X_i(\omega_i)$$

Natural questions to ask:
    - Is $(\Omega, \mathcal{F})$ even a measurable space?
    - What probability measure $\mathbb{P}$ should this measurable space equip? Ideally we should informally have
    $$ \mathbb{P}(A_1 \times A_2 \times ...) = \mathbb{P}(A_1) \times \mathbb{P}(A_2) \times ...$$
    Moreover, is there a way to *construct* this measure?

See **Kolmogorov Extension Theorem** for more information.

### Additional Preparation: Function space
Fix a closed and bounded interval $[a,b]$, then the set of all functions on $[a,b]$ is a vector space. We would like to consider its vector subspaces for which a norm can be defined (these are called *normed*-vector space). We have discussed a few spaces (sets):
- Space of all bounded function $B([a,b])$. This is a closed vector subspace with norm
$$
\|f\|_\infty = \sup_{[a,b]} |f(x)|
$$
This is often called a *supremum*-norm.
- Space of all continuous function $C^0([a,b])$. This is a closed vector subspace of $B([a,b])$ with the supremum norm.
- Space of all Riemann $L^p$ integrable functions $\mathcal{R}-L^p([a,b])$, with seminorm
$$
\|f\|_{\mathcal{R}-L^p} = \left( \int_a^b |f(x)|\, dx \right)^{1/p}
$$

A normed vector space is *complete* (Banach) if all Cauchy sequences of elements converge to another element in that normed vector space. We know that $\mathbb{R}^n$, $B([a,b])$ and $C^0([a,b])$ are Banach, but $\mathcal{R}-L^p([a,b])$ is not Banach (but the Lebesgue $L^p$ space is Banach).

### Exercises

#### Core
1. Make sure you have reviewed the notion of $\sigma$-algebra, pre-measure, measure and outer measure. Also make sure you are happy with the basic properties of measure (e.g. upper/lower continuity).
2. Preview notions of *open* and *closed* sets in Analysis I. In particular establish that the uncountable union of open set is open and uncountable intersection of closed set is closed.

#### Working with function space
3. You will learn about uniform convergence of functions. Try to write the definition of uniform convergence of functions using the supremum norm.
4. Let $V$ be a vector space with seminorm $\|. \|$. Define the equivalence relation $f \sim g$ iff $\|f-g \| = 0$. Now consider the quotient space $V/\sim$ (i.e. set of all equivalent classes). Show that $V/\sim$ is also a vector space. Now define for all equivalent classes $[f]_\sim \in V/\sim$,

$$\|[f]_\sim \|' = \|f\|$$

Show that the function $\|.\|'$ is well-defined (i.e. if we choose two functions $f,g$ from $[f]_\sim$ then the value of norm remains unchanged). Now show that $\|.\|'$ is a norm of $V/\sim$.


## 26/1 - Axioms of Measure
## 2/1 - Construction of Measure
## 9/2
## 16/2
## 23/2
## 2/2
## 9/3
## 16/3
## 23/3
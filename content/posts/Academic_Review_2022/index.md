---
author: "Samuel Lam"
title: "Review 2022 - Academic"
categories: ["2022"]
tags: ["review"]
ShowToc: true
TocOpen: true
date: 2023-01-03T00:00:00+08:00
draft: true
---

TL,DR:
- Research project at Imperial on equivalence of non-parametric statistical experiments.
- Coursework at Imperial on functional analysis, optimisation, asymptotic methods, dynamics of games and mathematical biology.
- Research project at CDT Mathematics of Random Systems on theories of deep learning

# The final year at Imperial

## Research Project
The major highlight of the year would be the completion of my final year dissertation with Prof. Alastair Young. The dissertation focuses on the equivalence of three non-parametric statistical experiments, including kernel density estimation, regression on Gaussian white noise and regression on Gaussian sequence. The motivation comes from the fact that one could build a common sample space and parameter space for all three experiments, and that estimators for each experiments could be represented as a random measure on the parameter space. As a result, We may introduce the notion of distances between experiments as being the minimum possible distance between estimators from each experiments (e.g. total variation distance). Through this project I explored the following topics
- notions of distance between measures
- KMT constructions for Brownian motion
- general properties for Poisson processes
- Girsanov theorem for Gaussian white noise.

It has been my pleasure to work with my supervisor, and I am delighted that the markers appreciate my project.

## Coursework
This year coursework has been focused on the following topics, which would contribute to my future research
- Functional analysis and PDE - which reviews basic results on functional analysis and spectral theory, and explains how they could be applied to prove the existence and properties of solutions to variational formulation of PDE,
- Optimisation - which reviews basic theory of convex optimisation (KKT conditions and duality) and introduce (stochastic) gradient descent and optimal control problems, and
- Asymptotic methods and perturbation analysis - which covers the notions of asymptoic equivalence and basic techniques in computing asymptotic expansions to solutions to algebraic equations, integrals and solutions to differential equation.
- Dynamics of games - which covers techniques for analysing replicator dynamics and introduce basic algorithms to reinforcement learning and no-regret learning.

To broaden my experience, I have also undertook the following a course on Mathematical biology - which reviews techniques in performing bifurcation analysis to dynamics that arise in nature, introduces methods to analyse reaction-diffusion, pattern formulation and stochastic formulation to natural dynamics.

## Graduation
I am fortunate to graduate from Imperial College London with a MSci in Mathematics with a Year Abroad, and to receive a sponsorship from Imperial for my membership at the Institute of Mathematics with its Applications (IMA). The University of Oxford has kindly agreed to continue sponsor my membership during my postgraduate studies.

# The first year at the University of Oxford
It has been my pleasure to join the CDT Mathematics of Random Systems organised by the University of Oxford and Imperial College London. This is an interdisciplinary programme focusing on the theories and applications of stochastic processes and statistical learning. I have been fortunate to be supervised by Prof. Justin Sirignano, and together we will investigate in numerous topics in the theories of deep learning.

## Research progress so far
My first project has been on the analysis of convergence of some algorithms used in the reinforcement learning (RL). The motivation comes from the fact that Markov processes, including the dynamics of RL algorithms under the Markov decision framework, could be approximated by a suitable ordinary differential equations (ODE). We could therefore understand the convergence of RL algorithms through looking at the dynamics of such ODE. Main computations is completed while numerical simulations are on going, and a pre-print should be available shortly.

I have also been working on a side project under the supervision of Prof. Jared Tanner and collaboration with other cohort members in sparsifying the deep neural network through a careful design of architecture.

## Coursework
The programme begins with courses on the foundations of stochastic processes, functional analysis unsupervised learning. It then follows by regular courses on topics in stochastic analysis (theories of stochastic partial differential equations, simulation methods and control problem) and theories of deep learning. These courses are good exposition to my research, and through the coursework projects I have been priviledged to work with most of my cohorts in Oxford. 

## A testimony
There are many things I value in this programme. I am, of course, delighted to maintain my connection with Imperial College through this programme, but I appreciate even more with the opportunities for me to collaborate with different faculties and coursemates that come from different backgrounds but still share the same enthusiasm on stochastic analysis. Through collaboration with them, I have not only broaden my horizon on topics I am previously less familiar with, but also acquire valuable transferrable skills, which would be useful in my future research. I definitely look forward to continue my journey in this programme.

## A summary for the programme
The main objective for the programme is to develop a further understanding on deep neural network, including
- expressivity of neural network
- generalisation property of neural network (e.g. applications of Neural Tangent Kernels)
- dynamics of optimisation algorithms
- applications of neural networks in numerical solutions to deterministic and stochastic differential equations, as well as optimal control problems.

The programme also contains the following side objectives
- further understanding of the geometry aspects of theories of deep learning (e.g. topological data analysis) and random matrix theory.
- basic understanding of rough path theory and signature kernels
- practical data science experience, e.g. internship
- practical teaching and outreach experience

During the first 18 months we will undergo several intense coursework and complete several projects to fulfill the above main/side objectives, before becoming a DPhil candidate through a *transfer of status*. The remaining 2.5 years will be dedicated to a main research dissertation, with a confirmation of status to be completed at the beginning of the 4th year.

# Acknowledgements statement to be made for graudation

I would like to thank the following faculties at Imperial College London for shaping my research careers.
- Dr. Christopher Ford (*Senior Tutor and Personal Tutor*): for his pastoral supports during my studies, as well as personal tutorials on calculus and classical mechanics. He had also coordinated the update of undergraduate curriculum and supported my applications to my undergraduate research programmes.
- Prof. Alastair Young (*Chair in statistics*): for his supervision in the final year project, as well as advice for researches in computational statistical theory.
- Dr. Michele Coti-Zelati (*Senior Lecturer*): for his supervision in my 2nd year Undergraduate Research Opportunities Programme (UROP), advice for my researches in PDE and stochastic analysis, and supports to my applications to numerous research programmes.

I would like to, in particular, formally thank the following faculties at Imperial College London for all their supports offered during my studies
- Prof. David Van-Dyk (*Head of Department*): for his leadership in the department.
- Dr. Christopher Hallsworth (*Director of Undergraduate*): for his leadership in the department. In addition, he offered us lectures on probability and statistics, which has laid a foundation to my research. He had also coordinated the update of undergraduate curriculum.
- Prof. David Evans (*previous Director of Undergraduate*): for his leadership in the department, as well as personal tutorials on algebra and analysis. He had also coordinated the update of undergraduate curriculum.
- Ms. Inkeri Hibbins (*Undergraduate Liaison Officer*): for her efforts in improving coordination in improving students' learning experience, especially during the Covid years. She had also coordinated in the update of undergraduate curriculum. 
- Dr. Martin Rasmussen (*Reader in Mathematics*): for his general supports to our cohort, as well as his effort in making the course on theories of ODE being more accessible.
- Dr. Sheehan Olver (*MIT-Imperial Exchange Coordinator*): for acting as the point of contact during the MIT-Imperial exchange. He has also introduced the modern Julia language in our curriculum.

I would like to also thank the following faculties from other institutions:
- Prof. Lyle Muller and Prof. Jan Minac: for their supervision during the Field Institute's Undergraduate Summer Research Programme (FUSRP), as well as supports to my applications to my PhD studies.
- Prof. John Bush: for his pastoral supports during my MIT-Imperial Exchange, as well as supports to my applications to my PhD studies.

Finally, I would like to thank the other lecturers for delivering high-quality classes during my undergraduate studies, as well as numerous friends for their supports in different aspects.
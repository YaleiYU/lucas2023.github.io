---
layout: post
title:  "Genetics Part I: DNA, Genes & Mendelian Inheritance"
date:   2020-05-10 20:00
author: Logan Williams
---

Highly autonomous unmanned aerial systems (UASs) operating in civilian airspace will provide a vast capability increase in sectors such as search and rescue and law enforcement. Autonomy allows a relatively unskilled operator to deploy numerous vehicles in unrestricted airspace yielding faster response times and greater coverage than manned operation. This is in contrast to the majority of current UAS operations which require a number of skilled personnel to operate a single vehicle. To achieve this goal it is necessary for each UAS to possess a high degree of autonomy which in turn requires sound artificial situation awareness. The principle of artificial situation awareness is analogous to the ability of a human pilot to perceive, comprehend and project the state of their environment (for example, the positions of other vehicles). Nowhere is this ability more critical than in the terminal region immediately surrounding an airfield, where many manned (and potentially unmanned) aircraft converge to a small region of airspace. A UAS operating autonomously in a congested terminal area must possess a level of situation awareness comparable with, if not greater than, an equivalent manned vehicle in order to operate safely.

| <img src="/images/blogs/genetics/first-project/Projection.png" alt="Deoxyribonucleic acid" title="Deoxyribonucleic acid" width="900"> |
|:--:| 
| *[Figure 1]().* Probabilistic representation of traffic position (left) compared with a Monte Carlo Simulation (right) |

Using the terminal area as an example, this project has developed a complete artificial situation awareness system for an autonomous UAS. The system is capable of predicting the states of traffic aircraft several minutes in to the future by making assumptions about their path and accounting for the inevitable accumulation of uncertainty. The traffic is assumed to follow a nominal path from its currently observed position to the runway, this may be a published Standard Terminal Arrival Route (STAR) or a more generic set of rules (e.g. an overhead join). The future positions of traffic are represented as probability distributions which capture uncertainty in velocities and the path itself. By catering for the non-Gaussian nature of the distribution it is able to match simulation results very closely (see below).
    


| <img src="/images/blogs/genetics/first-project/circuitJoin3.png" alt="Deoxyribonucleic acid" title="Deoxyribonucleic acid" width="900"> |
|:--:| 
| *[Figure 2]().* Typical replanning by the UAS (U) in the presence of traffic vehicles (T1 and T2), based on probability of future conflict |
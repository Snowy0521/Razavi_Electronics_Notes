

# Razavi Electronics 2, Lec 05, Problem of Biasing; Intro. to Current Mirrors

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [The Need for Current Sources](#the-need-for-current-sources)
2. [Problem of Biasing Current Sources](#problem-of-biasing-current-sources)
3. [Current Mirrors](#current-mirrors)


---
## The Need for Current Sources
+ Everywhere for biasing integrated circuits.


---
## Problem of Biasing Current Sources
1. Due to equation $I_D = \frac{1}{2}\mu_n c_{ox}\frac{W}{L}(V_b - V_{TH})^2$, so the threshold $V_{TH}$ and the mobility $\mu_n$ vary with temperature.
2. To generate $V_b = \frac{R_2}{R_1 + R_2}V_{DD}$, so the $V_b$ is supply-dependent.
---
## Current Mirrors
+ First build one "golden" current source, which is very stable and supply and temperature independent, using a "Bandgap" circuit.

+ Next, we copy/clone this current source to build many others.
+ ![](/images/circuitMirror1.png)
+ ![](/images/circuitMirror2.png)


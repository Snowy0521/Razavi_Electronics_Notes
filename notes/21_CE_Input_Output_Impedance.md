# Razavi Electronics 1, Lec 21, Input & Output Impedances

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Problem of Input Impedance](#problem-of-input-impedance)
2. [Problem of Output Impedance](#problem-of-output-impedance)





---
## Problem of Input Impedance
+ Problem: How do we identify a CE stage?
    + Input applied to base
    + Output sensed at collector

+ ![CE stage with input impedance](/images/CEwithInputImpedance.png)
    + $v_{\pi} = v_{in}\frac{r_\pi}{r_\pi + R_m} \to v_{out} = - g_m \frac{r_\pi}{r_\pi + R_m} v_{in}R_C$, which $\frac{r_\pi}{r_\pi + R_m}$ is attenuation factor.
    + To reduce the attenuation factor,  $r_\pi \gg R_m $

+ How calculate the input impedance $R_{in}$?
    1. Set all independent sources to zero, the voltage source to short, the current source to open.
    2. Apply a small-signal voltage source berween the input terminals, and calculate the current supplied by this voltage soure
    3. $R_{in} = \frac{U_x}{I_x} \to i_xr_\pi = v_\pi = v_x \to R_{in} = r_\pi$
---
## Problem of Output Impedance
+ Calculation of the output impedance $R_{out}$?
    1. Using Thevenin Equivalent, set all independent source to zero and measure the resistance $R_{th}$ between the terminals
    2. ![Output Resistance of CE](/images/OutputResistanceCE.png)
    3. if output resistance $R_C \gg R_{sp}$, big attenuation of gain
    
    

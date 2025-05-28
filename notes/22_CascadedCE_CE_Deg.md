# Razavi Electronics 1, Lec 22, Common-Emitter Stage with Degeneration

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Cascaded Stages](#cascaded-stages)
2. [Problem of Gain Variation](#problem-of-gain-variation)
3. [CE Stage with Emitter Degeneration](#ce-stage-with-emitter-degeneration)





---
## Cascaded Stages
+ ![Cascaded two stages](/images/CascadedCEstages.png)
+ What if $V_A < +\infty$(with Early Effect) ?
    + $A_{V1} = -g_{m1}(R_{C1}||r_{o1}||r_{\pi2})$
    + $A_{V2} = -g_{m2}(R_{C2}||r_{o2})$
    + $A_{Vtotal} = A_{V1}A_{V2}$
---
## Problem of Gain Variation
+ Variation with Temp. and Process ($R_C$)
    + $A_V = -g_mR_C = - \frac{I_CR_C}{V_T}$
    + $I_C = I_S \exp \frac{V_{BE}}{V_T}$
+ Variation with Signal Amplitude 
    + ![](/images/VariationWithSignalAmplitude.png)
    + $I_C$ changes with $V_{BE}$ so causes distored sinusoid
     

---
## CE Stage with Emitter Degeneration
+ $A_V \approx - \frac{R_C}{\frac{1}{g_m} + R_E}$ due to $\beta \gg 1$
+ ![CE Stage with Emitter Degeneration](/images/CEwithEmitterDegeneration.png)
+ $R_E$ tends to swamp the variations in this $g_m$

    
    

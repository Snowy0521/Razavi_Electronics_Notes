# Razavi Electronics 1, Lec 23, More on Emitter Degeneration

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Proporties of CE-Stage with Degeneration](#proporties-of-ce-stage-with-degeneration)
2. [Input & Output Impedences](#input--output-impedences)
3. [Degenerated Current Sources](#degenerated-current-sources)





---
## Proporties of CE-Stage with Degeneration
+ Gain is less sensitive to temp. and process variations and to signal amplitude.
    + $A_V = -\frac{R_C}{\frac{V_T}{I_C} + R_E}$

+ To minimize sensitivity to $I_C$, pick $R_E \gg \frac{V_T}{I_C} \to R_E I_C \gg V_T \to A_V \approx \frac{-R_C}{R_E}$
+ The gain is lower with degeneration than without degeneration.

+ general equation:
    $$
    A_V = - \frac{\text{Resistance tied between collector and GND}}{\frac{1}{g_m} + \text{Resistance tied between emitter and GND}}
    $$
---
## Input & Output Impedences
+ ![Input Impedence of CE Stage with Degeneration](/images/InputResistanceCEdegeneration.png)
+ $R_{in} = r_\pi + (\beta + 1)R_E$, when $A_V \to +\infty$

+ ![Output Impedence of CE Stage with Degeneration](/images/OutputResistanceCEDegeneration.png)
+ $R_{out}$ = $R_C$, when $A_V = \infty$
     

---
## Degenerated Current Sources
+ without degeration, the CE-stage as a current source has a slope $\frac{1}{r_o}$,
+ with degneration, the CE-stage as a current source has a slope $\frac{1}{(1+g_m(r_\pi||R_E))r_o + (r_\pi||R_E)}$, more constant, better current source.

+ ![Degenerated Current Sources](/images/CurrentSourceDegeneration.png)

+ $R_{out} = (1+g_mr_o)(R_E||r_\pi) + r_o$

    
    

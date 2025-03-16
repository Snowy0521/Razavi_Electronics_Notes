# Razavi Electronics 1, Lec 20, Common-Emitter Stage

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Basic Properties of Common-Emitter Stage](#basic-properties-of-common-emitter-stage)
2. [Voltage Gain Trade-offs](#voltage-gain-trade-offs)





---
## Basic Properties of Common-Emitter Stage
+ ![Simplified Diagram of Common-Emitter Stage](/images/SimplifiedCommonEmitter.png  )
+ ![Small-Signal Voltage Gain Calculation](/images/VoltageGainBipolar.png)
---
## Voltage Gain Trade-offs
+ According the equation $A_V = -g_m R_C$, if we need a higer gain, we can increase $R_C$?
    + No, because if $R_C\uparrow$, $V_{out}\downarrow = V_{CC} - R_C\uparrow I_C$, no enough headroom to keep transistor in active forward region if $V_{out} < V_{BE}$.
    + so, let's rise $g_m\uparrow = \frac{I_C\uparrow}{V_T}$? no, same problem.

+ Inclusion of Early Effect, it reduces the voltage gain.
    + $A_V = -g_m\cdot R_C||r_o$

+ What if we have a constant current source $R_C \to +\infty$, $R_C||r_o = \frac{r_o}{1 + (\frac{r_o}{R_C} \to 0)} \approx r_o$

+  $A_V = -g_mr_o = - \frac{I_C}{V_T} \cdot \frac{V_A}{I_C} = -\frac{V_A}{V_T}$, so $g_mr_o$ is the intrinsic gain of a transistor, you can't adjust it by adjusting $R_C$ or $I_C$.  


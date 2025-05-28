# Razavi Electronics 1, Lec 28, Emitter Follower & Summary

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Emitter Follower as a Buffer](#emitter-follower-as-a-buffer)
2. [Bias Design](#bias-design)
3. [Summary of Bipolar Circuits](#summary-of-bipolar-circuits)



---
## Emitter Follower as a Buffer
+ Without buffer, $A_V = -g_m(R_C||R_{sp})$, where $R_{sp}$ is a low resistor of a speaker, so make gain too low
    + ![](/images/SpeakerWithoutBuffer.png)

+ With buffer, we can avoid the effect from low resistor output component
    + ![](/images/SpeakerWithBuffer.png)

---
## Bias Design
1. Determine the DC level of $V_{out} \approx \frac{V_{CC} - V_{BE}}{2}$, for getting enough headroam for output swing. 
2. Determine the DC level of $V_{in} = V_{out} + V_{BE}$

3. Determine the bias resistors $R_1$ and $R_2$ with $V_{in}, V_{CC}$ and $I_{R_1} \gg I_{B}$
4. Replace $R_E$ with a constant current source such as other bipolar transistor 

    
---
## Summary of Bipolar Circuits
+ If $V_A < \infty$, we get a $r_o$ in parallel with $R_E$ so $R_E \to R_E||r_o$
### CE Stage with $V_A < \infty$
+ $A_V = -g_m(R_C||r_o)$
+ $R_{in} = r_\pi$
+ $R_{out} = R_C||r_o$

### CE Stage Deg. with $V_A = \infty$
+ $A_V = -\frac{R_C}{\frac{1}{g_m} + R_E}$
+ $R_{in} = r_\pi + (\beta + 1) R_E$
+ $R_{out} = R_C$

### CE Stage Deg. with $V_A < \infty$ and without $R_C$
+ $R_{out} = (1+g_mr_o)(R_E||r_\pi) + r_o$

### CB Stage with $V_A = \infty$
+ $A_V = g_mR_C$
+ $R_{in} = \frac{1}{g_m}||R_E$
+ $R_{out} = R_C$

### Emitter Follower with $R_B > 0 \& V_A = \infty$
+ $A_V = \frac{R_E}{R_E + \frac{1}{g_m} + \frac{R_B}{\beta + 1}}$
+ $R_{in} = R_B + r_\pi + (\beta + 1)R_E$
+ $R_{out} = R_E || (\frac{1}{g_m} + \frac{R_B}{\beta + 1})$

### Useful Impedance Expressions
+ ![](/images/UsefulImpedanceExps.png)
+ In case 3, $R_E = \frac{1}{\frac{1}{r_\pi} + g_m} \approx \frac{1}{g_m}$

### The impedance of Diode-Connected Transistor
+ $R_i = \frac{1}{\frac{1}{r_\pi} + g_m} \approx \frac{1}{g_m}$

### Example with PNP CE Stage Deg.
+ ![](/images/ExamplePNP_CE_Deg.png)


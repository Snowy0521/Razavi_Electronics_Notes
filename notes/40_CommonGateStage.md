# Razavi Electronics 1, Lec 40, Common-Gate Stage

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Small-Signal Analysis](#small-signal-analysis)
2. [Bias Design](#bias-design)



---
## Small-Signal Analysis
![](/images/CGstageAnalysis.png)
+ $v_{in} = -v_1$
+ KCL: $-g_mv_{in} + \frac{v_{out}}{R_D} = 0 \to A_V = g_mR_D$
+ For $R_{in}$ calculation:
    + KCL: $i_x -g_mv_x = 0\to R_{in} = \frac{1}{g_m}$
    + the typical input resistance is not so high, specially used for applications like LNA(low noise amplifier) for impedance matching and power transfer

+ For $R_{out}$ calculation (same as CS-stage):
    + $R_{out} = R_D$ for $\lambda = 0$


### Example
![](/images/CascadedCS_CG_Exp.png)
+ $\frac{v_{out}}{v_{in}} = \frac{v_x}{v_{in}}\frac{v_{out}}{v_{x}} = \frac{-(R_D||\frac{1}{g_{m2}})}{\frac{1}{g_{m1}}+R_S}g_{m2}R_{D2}$

### $R_{out}$ of CG Stage in a special case $\lambda \neq 0$
+ A special case means add a resistor $R_S$ at source terminal
+ Its small signal model is equal to common source stage with degeneration
+  $R_{out} = R_D || [(1+g_mr_o)R_S + r_o]$

---
## Bias Design
![](/images/BiasDesignCG.png)
+ Using a resistor or (capacitor, inductor) to let current go through GND due to V-Atenna is open for DC calculation
+ We tend to loss some signal due to $R_S$
+ Current Division: $i_1 = \frac{R_S}{R_S + \frac{1}{g_m}}i_{antenna}$ so $R_S \gg \frac{1}{g_m}$


### Example
+ Given $V_{DD} = 1.5V, P = 1.5 mW, \mu_nC_{ox} = 100 \mu A / V^2, V_{TH} = 0.5 V, \lambda = 0, \frac{W}{L} = 50, I_D \approx  1mA$
+ $I_D = \frac{1}{2}C_{ox}\frac{W}{L}(V_{GS}- V_{TH})^2 \to V_{GS} = 1.13 V \to g_m = \frac{2I_D}{V_{GS}-V{TH}} = 3.2 mS = \frac{1}{316\Omega}, R_S \approx \frac{10}{g_m} = 3.16 k\Omega$
+ But $R_{S, max} = \frac{V_{DD}-V_{GS}}{I_D} = 370\Omega \ll 3.16 k\Omega$ (not valid)
+ For $R_D \to V_{DS} = V_{DD} - I_DR_D \geq V_{GS}(V_{DD}) - V_{TH} \to  I_DR_D \leq V_{TH} \to R_D = 500\Omega$
+ $A_V = g_m R_D = 1.6$ (too low)
+ What if we double $\frac{W}{L} = 100$?
    + $V_{GS} = 0.95 V$
    + $R_S = \frac{V_{DD} - V_{GS}}{I_D} = 550 \Omega$
    + $g_m = \frac{1}{220\Omega} = 4.5 mS$
    + $A_V = g_m R_D = 2.3 \uparrow$


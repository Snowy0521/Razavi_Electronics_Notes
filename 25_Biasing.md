# Razavi Electronics 1, Lec 25, Biasing Techniques II

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Supply Sensitivity in CE Stage with Degeneration](#supply-sensitivity-in-ce-stage-with-degeneration)
2. [Design Example](#design-example)
3. [Self-Biased CE-Stage](#self-biased-ce-stage)






---
## Supply Sensitivity in CE Stage with Degeneration
+ ![](/images/BiasingCEstageGeg.png)
+ ![Supply Sensitivity in CE Stage with Degeneration](/images/SupplySensitivityCEstageDeg.png)
+ Supplementary formula derivation：
    + $r_\pi = \frac{\beta}{g_m} \to \frac{1}{r_\pi} = \frac{g_m}{\beta}$
    + $\frac{1}{r_\pi} + g_m \approx g_m$
    + $\frac{v_E}{v_x} = \frac{g_m}{\frac{1}{R_E} + g_m} = \frac{R_E}{\frac{1}{g_m} + R_E} $

### Summary of Biasing
+ To reduce sensitivity, $\frac{V_{CC}}{R_1 + R_2} \approx 10I_B$, $\frac{1}{g_m} \gg R_E \to R_EI_C \gg V_T$
+ To keep the bipolar in forward bias region, $V_C \geq V_{BE}(V_x)$
---
## Design Example
+ $V_{CC} = 1.5V$, $P = 1.5mW$, $\beta = 100$
+ $I_{supply} = I_{CC} = \frac{V_{CC}}{P} = 1mA \to I_C \approx 1mA$
+ $I_B = 10\mu A \to \frac{V_{CC}}{R_1 + R_2} = 100\mu A (1)$
+ Pick $R_EI_C = 100 mV \to R_E = 100\Omega$
+ $V_x = V_{BE} + 100mV \approx 900mV \approx \frac{R_2}{R_1 + R_2} V_{CC} (2)$
+ With $(1) \&(2) \to R_1 = 9k\Omega, R_2 = 6k\Omega$
+ $V_C = V_{CC}-R_CI_C \geq 0.9V \to R_C = 600\Omega$

### Quiz:
1. Caculate the gain of the amp.?
    + $A_V = \frac{-R_C}{\frac{1}{g_m} + R_E} = - 4.76$ 

2. How do we increase the gain without changing the bias components?
    + $A_V\uparrow = \frac{-R_C}{\frac{1}{g_m} + R_E\downarrow}$
    + To reduce $R_E$, parallel with a capacitor $C_E \to Z_E = R_E || \frac{1}{wC_E}$

+ If $\Delta V_x = 45mV, (5\%\text{change}) \to \Delta V_E = \frac{R_S}{\frac{1}{g_m} + R_S}\Delta V_x = 36mV$
+ $\Delta I_C = \frac{36mV}{100\Omega} = 0.36mA \to 36\%\uparrow$
---
## Self-Biased CE-Stage
+ ![](/images/SelfBiasedCEstage.png)
+ A self-correction mechanism: a resistor $R_F$ connected between base $B$ and collector $C$.
    + For example, if $V_{CC}\uparrow, V_C(V_{out})\uparrow = V_{CC} - I_CR_C, V_B\uparrow = V_C - I_{B}R_F$, but if $V_B\uparrow \to I_C\uparrow \to V_C\downarrow$
+ Changes in $V_{CC}$ are counteracted by $Q_1$
+ $V_{CC} - R_CI_C - R_FI_B = V_{BE}$ and $V_{BE} = V_T\ln\frac{I_C}{I_S}$ and $I_B = \frac{I_C}{\beta}$
+ $I_C = \frac{V_{CC}- V_{BE}}{R_C + \frac{R_F}{\beta}}$
+ To minimize sensitivity to $\beta$, $R_C \gg \frac{R_F}{\beta} \to R_F \ll \beta R_C$
+ If $V_{CC} \uparrow 5\% \to I_C\uparrow \approx 5\%$

### Example
+ If $V_{CC} = 1.5V, I_C = 1mA, \beta = 100$
+ $V_C = 0.9V \to R_C = \frac{(1.5 - 0.9)V}{1mA} = 600 \Omega$
+ $R_F = \frac{\beta R_C}{10} = 6 k\Omega$
+ $I_B = 10 \mu A \to V_{R_F} = 60 mV$


    
    

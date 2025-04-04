# Razavi Electronics 1, Lec 38, Common-Source Stage with Degeneration

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [CS Stage with Degeneration](#cs-stage-with-degeneration)
2. [Degenerated Current Source](#degenerated-current-source)






---
## CS Stage with Degeneration
Assume $\lambda = 0$

1. Bias Conditions:
![](/images/CSwithDegeneration.png) 
+ $V_o = V_{GS} + I_D R_S$
+ In saturation region: $I_D = \frac{1}{2}\mu_n C_{ox}(V_{GS} - V_{TH})^2$
+ $\text{Drain Voltage} = V_{DD} - I_D R_D$
+ For saturation region: $V_{DD} - I_D R_D \geq V_o - V_{TH}$


2. Calculate Gain
![](/images/CSgeneration_small_signal.png)    
+ KCL: $g_m v_1 = - \frac{v_{out}}{R_D} \to v_1 = - \frac{v_{out}}{g_m R_D}$
+ KVL: $v_{in} = - \frac{v_{out}}{g_mR_D} - \frac{v_{out}}{R_D}R_S$
+ $A_V = \frac{v_{out}}{v_{in}} = \frac{-R_D}{\frac{1}{g_m} + R_S}$, if $\frac{1}{g_m} \ll R_S \to A_V \approx - \frac{R_D}{R_S}$
+ In generall, $A_V = - \frac{\text{Resistance tied between drain and AC GND}}{\frac{1}{g_m} + \text{Resistance tied between source and AC GND}}$
+ Example for $R_D$ is replaced by a diode-connected transistor $M_2 \to A_V = -\frac{\frac{1}{g_{m2}}}{\frac{1}{g_{m1} + R_S}}$

### Question: Why is the gain less with degeneration? (intuition)
![](/images/IntuitionAnalysisCS-Stage.png)
+ Compare to the CS-stage without $R_S$, the $V_{GS}$ of CS-stage with degneration changes weaker than former.

### Impedance of Ideal Constant Voltage and Current Source
+ $R_{eq} = 0$ for ideal voltage source, short circuit 
+ $R_{eq} = \infty $ for ideal current source, open circuit


--- 
## Degenerated Current Source
+ The higer the $R_{out}$, The better the current source
+ $R_{out} = r_o$ without Degeneration
+ Calculate $R_{out}$ with Degeneration$:
    + $v_1 = - i_x R_S$
    + $g_mv_1 = - g_m i_x R_S$
    + KVL: $v_x = r_o (i_x + g_m i_x R_S) + i_x R_S$
    + $R_{out} = \frac{v_x}{i_x} = (1 + g_m R_S)r_o + R_S \text{ or } (1 + g_m r_o)R_S + r_o \gg r_o$

+ An example that $R_S$ can be replaced by biased NMOS Transistor $r_{o2} \to R_{out} = (1+ g_{m1}r_{o1})r_{o2} + r_{o1}$




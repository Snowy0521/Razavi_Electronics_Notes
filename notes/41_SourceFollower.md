# Razavi Electronics 1, Lec 41, Source Follower & Summary

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Small-Signal Analysis](#small-signal-analysis)
2. [Summary](#summary)



---
## Small-Signal Analysis
+ Input applied at gate terminal, Output sensed at source terminal
+ The output voltage follows the input variation, so it called source follower
+ $A_V$ calculation with small signal model ($\lambda = 0$):
    + KVL: $v_{in} = v_1 + v_{out} \to v_1 = v_{in} - v_{out}$
    + KCL: $g_m(v_{in} - v_{out}) = \frac{v_{out}}{R_S} \to \frac{v_{out}}{v_{in}} = \frac{R_S}{\frac{1}{g_m} + R_S}$
    + In generall, $A_V = \frac{\text{Resistance tied between source and GND}}{\frac{1}{g_m} + \text{Resistance tied between source and GND}}$
    + For $\frac{1}{g_m} \ll R_S \to A_V \approx 1$

+ $A_V$ calculation with Thevenin Equivalent ($\lambda = 0$):
![](/images/SourceFollowerThev.png)
    + KCL: $g_m v1 = 0 \to v_1 = 0 \to v_{\text{Thev}} = v_{out} $
    + KCL in small signal model: $- g_m v_x + i_x = 0 \to \frac{v_x}{i_x} = \frac{1}{g_m}$
    + $\frac{v_{out}}{v_{in}} = \frac{R_S}{\frac{1}{g_m} + R_S}$ 

+ What if the $\lambda > 0$?
    + $A_V = \frac{R_S || r_o}{R_S || r_o + \frac{1}{g_m}}$

+ $R_{in} = \infty \text{ at lower frequencies}$
+ $R_{out} = \frac{1}{g_m}||R_S||r_o$
+ So source follower has very high input impedance, and very lowr output impedance.
+ Due to this characteristic, source followers are normally acted as buffer.
![](/images/SourceFollowerBufferExp.png)

+ Example for two stage cascaded circuits with source follower and common-gain stage
![](/images/SourceFollowerCommonGateExp.png)
    + $A_V = \frac{v_x}{v_{in}} \frac{v_{out}}{v_{x}} = \frac{R_S || \frac{1}{g_{m2}}}{R_S || \frac{1}{g_{m2}} + \frac{1}{g_{m1}}}g_{m2}R_D$
---
## Summary
+ For CS Stage $\lambda = 0$
    + $A_V = -\frac{R_D}{\frac{1}{g_m} + R_S}$

+ For CG Stage $\lambda = 0$
    + $A_V = g_m R_D$

+ For source follower $\lambda = 0$
    + $A_V = \frac{R_S}{\frac{1}{g_m} + R_S}$

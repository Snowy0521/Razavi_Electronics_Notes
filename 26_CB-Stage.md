# Razavi Electronics 1, Lec 26, Common-Base Stage

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Common-Base Stage](#common-base-stage)
2. [Basic Properties](#basic-properties)
3. [Bias Design](#bias-design)






---
## Common-Base Stage
+ ![](/images/CBstage.png)
+ $v_{in} = - v_\pi$
+ $v_{out} = -g_mv_\pi R_C = -g_m(-v_{in})R_C \to A_V = g_m R_C$

---
## Basic Properties
+ KCL: $i_{in} + g_mv_\pi + \frac{v_\pi}{r_\pi} = 0 \to i_{in} = v_{in}(g_m + \frac{1}{r_\pi})$ with $r_\pi = \frac{\beta}{g_m} \to i_{in} = v_{in}g_m \to R_{in} = \frac{1}{g_m}$
+ $R_{out} = R_C$

### Question: Why doesn't the CB stage invert?
+ $\Delta V_E \uparrow \to V_{BE}\downarrow \to I_C\downarrow \to V_{out}\uparrow = V_{CC} - R_CI_C\downarrow$

### Quiz: Cascaded CE and CB stage Bipolar 
+ ![](/images/CascadeCE&CB.png)
+ $A_V = \frac{v_{out}}{v_{in}} = \frac{v_{out}}{v_{x}} \frac{v_{x}}{v_{in}}$
+ $\frac{v_{x}}{v_{in}} = - g_{m1}(R_{C1}||\frac{1}{g_{m2}})$
+ $\frac{v_{out}}{v_{x}} = g_{m2}R_{C2}$



---
## Bias Design
+ ![](/images/CBbiasDesign.png)
+ Antenna is an open circuit for DC concern
+ DC current conduction: Resistor, Capacitor and Inductor
+ We can choose a resistor $R_E$ to conduct DC current between Collector and Emitter
    + $R_E \gg \frac{1}{g_m}$

### Example
+ $V_{CC} = 1.5 V, P = 1.5mW, \beta = 100 \to I_C \approx 1mA$
+ $\frac{1}{g_m} = \frac{I_C = 1mA}{V_T = 26mV} = 26 \Omega \to R_E = 260 \Omega$
+ $V_x = V_{BE} + V_E \approx 1.06 V$
+ $I_B = \frac{V_{CC}}{R_1 + R_2} = 100\mu A$ and $\frac{R_2}{R_1 + R_2}V_{CC} = 1.06 V \to R_1 = 10.6 k\Omega, R_2 = 4.4 k\Omega$
+ $V_C = V_{CC} - I_C R_C \geq V_x = 1.06 V \to R_C = 440 \Omega$
+ if $R_E \uparrow \to V_E \uparrow \to V_x \uparrow \to R_C \downarrow \to A_V \downarrow$, for this reason we should not choose $R_E$ much beyond 10 times $\frac{1}{}$



    
    

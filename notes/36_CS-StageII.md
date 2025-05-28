# Razavi Electronics 1, Lec 36, Common-Source Stage II

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [CS Example](#cs-example)
2. [Inclusion of Channel-Length Modulation](#inclusion-of-channel-length-modulation)






---
## CS Example

![](/images/CS-Stage-Exp.png)
+ Given a CS-stage amplifier, $\mu_nC_{ox} = 100 \mu A/V^2$, $V_{TH} = 0.5 V$, $\lambda = 0$, $\frac{W}{L} = 10$, $V_{DD} = 2V$, $R_D = 3 k\Omega$
    1. Bias Calculations: $V_{GS} = 1.2 V$ no signal input
    Assume in saturation region $\to I_D = \frac{1}{2}\mu C_{ox}\frac{W}{L}(V_{GS}-V_{TH})^2 = 245 \mu A$
    2. $V_{DS} = V_{DD} - I_DR_D = 2 V - 245 \mu A \cdot 3k \Omega = 1.265 V > V_{GS} - V_{TH} \to \text{in saturation region}$
    3. Calculate small-signal parameters:
        + $g_m = \frac{2I_D}{V_{GS} - V_{TH}} = 0.7 mS = \frac{1}{1.43 k\Omega}$ 
        + $A_V = - g_m  R_D = - 2.1$

+ How double the gain $A_V$? Try doubling $R_D$
    + If $I_D$ is still equal to $245 \mu A$, we have $V_{DS} = V_{DD} - I_D R_D = 0.53 V < V_{GS} - V_{TH} \to \text{Triode Region}$
    + Try increasing $g_m = \sqrt{2 \mu_n C_{\text{ox}} \frac{W}{L} I_D} \to \frac{W}{L}\uparrow \text{ or } I_D \uparrow$, but the same issue for $I_D\uparrow \to \text{ Triode Region}$
    + So we can only make the transistor wider $W\uparrow$
    + But if $\frac{W}{L}$ becomes sufficiently large, $g_m \approx \frac{I_D}{1.5 V_T}$


--- 
## Inclusion of Channel-Length Modulation
+ $A_V = -g_m \{\text{total resistance tied from drain to AC GND}\}$
+ $A_V = -g_m (R_L || r_o)$
+ Replace resistor $R_L$ with an ideal current soruce $\to A_V = -g_m r_o (5 \to 10) \to \text{intrinsic gain of MOS device}$

### Concept of Part Impedance
thevenin's theorem
+ Set all independent sources to zero




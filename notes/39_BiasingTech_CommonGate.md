# Razavi Electronics 1, Lec 39, Biasing Techniques, Intro. to Common-Gate Stage

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [I/O Impedances of CS Deg. Stage](#io-impedances-of-deg-cs-stage)
2. [Biasing Techniques](#biasing-techniques)
3. [Common-Gate Topologies](#common-gate-topologies)






---
## I/O Impedances of Deg. CS Stage
+ Input impedance at low frequencies $R_{in} = \infty$
+ Output impedance at $\lambda > 0 \to R_{out} = R_D || [(1 + g_m r_o)R_S + r_o]$

--- 
## Biasing Techniques
![](/images/BiasingCSstageGeg.png)
+ Using resistance divider to bias voltage $\frac{R_2}{R_1 + R_2}V_{DD} = V_o$
+ For $\lambda > 0, R_{in} = R_1 || R_2 \to A_V = \frac{v_{out}}{v_{in}} = \frac{v_x}{v_{in}}\cdot  \frac{v_{out}}{v_{x}} = \frac{R_1 || R_2}{R_1 || R_2 + R_{mike}}\cdot (-g_mR_D) $
+ Choose $R_1 || R_2 \gg R_{mike}$ to minimize the attenuation.
+ We cannot just increase $R_D$ to increase the gain due to $V_D = V_{DD} - I_DR_D \geq V_o - V_{TH} \to R_D \leq \frac{V_{DD}-V_o+V_{TH}}{I_D}$

+ A capacitor must be inserted between cascaded amplifier or the antenna between input for stage isolation.
### Reduced Sensitivity with Deg. CS Stage
+ $V_{DD}\frac{R_2}{R_1 + R_2} = V_{GS} + I_D R_S$
+ $I_D = \frac{1}{2}\mu_n C_{ox}\frac{W}{L}(V_{GS}-V_{TH})^2$
+ Without Reg. $I_D = \frac{1}{2}\mu_n C_{ox}\frac{W}{L}(V_{DD}\frac{R_2}{R_1 + R_2}-V_{TH})^2$ sensitive to $V_{DD}$, process($\mu_n C_{ox}, V_{TH}$) and temp.

![](/images/BiasingCS_reduceSensitivity.png)
### Self-Biased CS Stage
+ If $V_{TH}\downarrow \to I_D\uparrow \to V_D\downarrow \to V_G\downarrow \to I_D\downarrow$, self correction mechanism
+ $V_{DS} = V_{GS} > V_{GS} - V_{TH}$, so always in saturation region
+ $V_{GS} = V_{DD} - I_DR_D \to I_D = \frac{1}{2}\mu_n C_{ox}\frac{W}{L}(V_{DD} - I_DR_D - V_{TH})^2$
---
## Common-Gate Topologies
![](/images/CommonGainStage.png)
+ Input applied to source, output sensed at drain




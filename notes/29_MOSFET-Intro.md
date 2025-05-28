# Razavi Electronics 1, Lec 29, Intro. to MOSFETs

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Structure of MOSFET](#structure-of-mosfet)
2. [Basic Operation of MOSFET](#basic-operation-of-mosfet)




---
## Structure of MOSFET
![](/images/Mosfet_Observation.png)
+ For this capacitor, if $V\uparrow \to Q\uparrow \to \text{electron density}\uparrow$ due to equation $Q = C V_1$
+ $C\uparrow = \frac{\epsilon A}{t(d)\downarrow} \to \text{electron density}\uparrow$
+ If $V_2$ is applied $\to$ current flows from A to B
+ If $V_1\uparrow \to \text{electron density}\uparrow \to \text{Resistance between A and B}\downarrow \to \text{current}\uparrow$
### MOS(Metal-Oxide-Semiconductor) Structure
![](/images/Mosfet_structure.png)
+ The MOSFET(MOS Field Effect Transistor) has four terminals(Substrate, Source, Gate, Drain)
+ Compare to Bipolar Transistor, MOSFET structure is symmetric.
+ Thickness of insulator $t_{ox} \approx 15-18 \text{\AA}$ which $\text{ \AA} = 10^{-10} \text{ m} = 0.1\text{nm}$

--- 
## Basic Operation of MOSFET
+ If $V_G = V_{TH}$, a channel occurs between source and drain terminals.
+ As $V_G\uparrow \to \text{electron density in the channel}\uparrow \to \text{resistance between source and drain}\downarrow$
+ Compare $I_B > 0$ in bipolar transistor, $I_G = 0$ in MOSFET.
+ Assume $V_D > V_S = 0$:
    1. $V_D = \text{const, e.g. 0.3 V}$, if $V_G > V_{TH}, I_D\uparrow \text{with} V_G\uparrow$
    2. $V_G = \text{const, e.g. 1V}$, $I_D\uparrow \text{with} V_D\uparrow$


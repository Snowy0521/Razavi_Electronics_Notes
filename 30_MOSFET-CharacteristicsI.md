# Razavi Electronics 1, Lec 30, MOS Characteristics I

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Behavior of Channel](#behavior-of-channel)
2. [Derivation of I/V Characteristics](#derivation-of-iv-characteristics)




---
## Behavior of Channel
![](/images/ChannelChargeDensity.png)
+ Case I: $V_{GS} > V_{TH}, V_S = V_D = 0 \to \text{only channel, turned on,   no current}$
+ Case II: $V_{GS} > V_{TH}, V_D > V_S = 0 \to \text{channel, turned on, current} \to \text{voltage along the channel increases} \to \text{various voltage} \Delta V \to \text{various charge density}$


### Dimensions of MOSFET 
![](/images/Dimension_MOSFET.png)
+ $L_\text{drawn}$ is the drawn layout length of MOSFET, $L_\text{eff}$ is actual length of fabricated MOSFET
, which $L_\text{eff} < L_\text{drawn}$
--- 
## Derivation of I/V Characteristics
+ Channel Charge Density, $C_{ox}$ is capacitor per unit area with unit of $F/m^2$, $V_{GS} - V_{TH}$ is gate source overdrive voltage.
    + Case I: $V_G > V_{TH}, V_D = 0$, 
    $$ Q_{ch_{total}} [\text{Coulomb}] = WL\cdot C_{ox}(V_{GS} - V_{TH})$$
    $$ Q_{ch_{density}} [\text{Coulomb}/m] = W\cdot C_{ox}(V_{GS} - V_{TH})$$

    + Case II:  $V_G > V_{TH}, V_D > 0$
    $$ Q_{ch_{\text{density at $v$ length in channel}}} [\text{Coulomb}/m] = v\cdot W\cdot C_{ox}(V_{GS} - V_{TH} - V(x))$$


+ Drain Current 
    + Velocity $v$ of carriers is equal to the mobility $\mu$ times the electric field $E$: $v = \mu E$, $E = - \frac{dV}{dx} \to v = -\mu \frac{dV}{dx} $
        where:
        - $ v $: Velocity of the charge carriers (in $m/s$),
        - $ \mu $: Mobility of the charge carriers (in $m^2/V·s$),
        - $ E $: Electric field applied to the material (in $V/m$).
    
    + $I_D = - v \cdot Q_{ch, den} =- v\cdot W\cdot C_{ox}(V_{GS} - V_{TH} - V(x))$
    +  $I_D =\mu \frac{dV}{dx}\cdot W\cdot C_{ox}(V_{GS} - V_{TH} - V(x))$

    + $\int_0^L I_D \, \mathrm{d}x = \mu_n W C_{ox} \int_0^{V_{DS}} \left[ V_{GS} - V_{TH} - V(x) \right] \, \mathrm{d}V$

    + $L I_D = \mu_n C_{ox} W \left[ (V_{GS} - V_{TH}) V - \frac{1}{2} V^2 \right] \bigg|_0^{V_{DS}}$

    + $I_D = \mu_n C_{ox} \frac{W}{L} \left[ (V_{GS} - V_{TH}) V_{DS} - \frac{1}{2} V_{DS}^2 \right]$

    + ![](/images/I_DversusV_DS.png)


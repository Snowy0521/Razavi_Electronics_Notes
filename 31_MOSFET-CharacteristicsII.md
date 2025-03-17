# Razavi Electronics 1, Lec 30, MOS Characteristics II

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [MOSFET I/V Characteristics](#mosfet-iv-characteristics)
2. [Regions of Operation](#regions-of-operation)
3. [Simple MOS Model](#simple-mos-model)




---
## MOSFET I/V Characteristics
+ If $V_{DS} \ll 2(V_{GS} - V_{TH}) \to I_D \approx \mu_n c_{ox}\frac{W}{L}(V_{GS}-V_{TH})V_{DS} \to R_{on} = \frac{1}{ \mu_n c_{ox}\frac{W}{L}(V_{GS}-V_{TH})}$
+ So, this MOSFET can act as a voltage-dep. resistor (if $V_{DS} \ll 2(V_{GS} - V_{TH})$)
+ So, from the equation of $R_{on}$, if $V_{GS} > V_{TH}$, The MOSFET acts as a turned on swith, if $V_{GS} \leq V_{TH} \to R_{on} \to \infty$, turned off.
### Application in Bluetooth Module 
+ A bluetooth module has RX(Receiver) and TX(Transmitter), the MOSFET-Switch decides, which is on or off, it means that module should receive data or send data.

### $I_D$ for $V_{DS} > V_{GS} - V_{TH}$ ?
![](/images/SaturationAnalysePinchOff.png)
+ The pinch-off length $L_\text{pinch off} \ll L_{eff}$
+ Rederive the I/V equation:
    + $\int_0^L I_D \, \mathrm{d}x = \mu_n W C_{ox} \int_0^{V_{GS} - V_{TH}} \left[ V_{GS} - V_{TH} - V(x) \right] \, \mathrm{d}V$
    +  $I_D = \frac{1}{2}\mu_n C_{ox} \frac{W}{L}  (V_{GS} - V_{TH})^2$ for $V_{DS} \geq V_{GS} - V_{TH}$

--- 
## Regions of Operation
![](/images/MOSFET_Regions.png)
+ In saturation region, the MOSFET acts as a current source.

---
## Simple MOS Model in Saturation
![](/images/SimpleModelMOSFET.png)
### Example
+  $\mu_n c_{ox} = 100 \mu A/V^2, V_{TH} = 0.5V, \frac{W}{L} = \frac{5 \mu m}{0.5 \mu m}$, design a $1mA$ current source 
    + $1mA = \frac{1}{2}(100 \mu A/V^2)\cdot 10 \cdot (V_{GS}-0.5)^2 \to V_{GS} = 1.9 V$ but with condition $V_{DS} > 1.4 V$ for saturation region.
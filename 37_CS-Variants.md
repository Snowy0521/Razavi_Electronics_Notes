# Razavi Electronics 1, Lec 37, Common-Source Variants

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [MOS Current Sources](#mos-current-sources)
2. [Other Variants of CS Stage](#other-variants-of-cs-stage)
3. [Input and Output Impedances](#input-and-output-impedances)






---
## MOS Current Sources
![](/images/CSasCurrentSource.png)
+ A MOS transistor acts as current source for bias calculations and acts as resistor $r_o$ for the small signal model.

--- 
## Other Variants of CS Stage
### Common-Source Stage with Current-Source Load
+ $A_V = -g_m r_{o1}$ with ideal current source
+ But in reality, a MOS transistor  can act as a current source with resistor $r_o \to A_V = - g_m r_{o1}||r_{o2}$

### Diode-connected Device 
![](/images/DiodeConnectedCS.png)
+ KVL: $v_1 = v_x$
+ KCL: $i_x = \frac{v_x}{r_o} + g_m v_x \to R_{out} = \frac{1}{\frac{1}{r_o}+ g_m} $
+ if neglect channel length modulation $R_{out} = \frac{1}{g_m}$


### CS Stage with Diode-Connected Load
+ if $\lambda = 0 \to A_V = - g_{m1} \frac{1}{g_{m2}}\to - \frac{\sqrt{2\mu_n C_{ox} (\frac{W}{L})_1 I_{D1 }}}{\sqrt{2\mu_n C_{ox} (\frac{W}{L})_2 I_{D2 }}} \text{ with } I_{D1} = I_{D2} \to - \frac{\sqrt{ (\frac{W}{L})_1 }}{\sqrt{ (\frac{W}{L})_2 }} = - \sqrt{\frac{(\frac{W}{L})_1}{(\frac{W}{L})_2}}$

+ if $\lambda \neq 0 \to A_V = - g_{m1}(\frac{1}{g_{m2}}|| r_{o2} || r_{o1})$

---
## Input and Output Impedances
+ $Z_{in} = \infty \text{ for  low frequencies due to MOS acts as capacitor}$
+ $Z_{out} = R_D || r_o \text{ for a resistance load}$
+ $Z_{out} = r_{o1} || r_{o2} \text{ for a current source (biased transistor) load}$
+ $Z_{out} = r_{o1} || (\frac{1}{g_{m2}} || r_{o2}) \text{ for a diode connected transistor load}$

### Factors affecting the gain
$A_V = - g_m R_D = - \sqrt{2\mu_n C_{ox} \frac{W}{L} I_D} R_D$
+ Temperature 
+ Supply Voltage
+ Process Variation
+ Signal Level ($I_D$ changes with $V_{GS}$)
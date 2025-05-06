# Razavi Electronics 2, Lec 03, MOS and Bipolar Cascode Amplifiers

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [MOS Cascode Amplifier](#mos-cascode-amplifier)
2. [Cascode Amplifier with Cascode Load](#cascode-amplifier-with-cascode-load)


---
## MOS Cascode Amplifier
### Two steps of voltage gain
![](/images/CascodeAmp1.png)
![](/images/CascodeAmp2.png)
+ a: Calcualte $G_m = g_{m2}$
+ b: Calcualte $R_{out} = (1+g_{m1}r_{o1})r_{o2} + r_{o1}$
+ $A_V = -g_{m2} [(1+g_{m1}r_{o1})r_{o2} + r_{o1}] \approx - g_{m1}r_{o1}\cdot g_{m2}r_{o2}$

### Quiz
![](/images/QuizR_x.png)
+ Due to $R_x \ll r_{o2}$ so the current $g_{m2}V_{in}$ prefers flow to $M_1$ way not the $r_{o2}$ way.

---
## Cascode Amplifier with Cascode Load
### Cascode Amplifier with Resistance Load
![](/images/CascodeReLoad.png)
+ Calculate $G_m = g_{m2}$
+ Calculate $R_{out} = R_D || [(1+g_{m1}r_{o1})r_{o2} + r_{o1}]$
+ $A_V = -g_{m2} R_D || [(1+g_{m1}r_{o1})r_{o2} + r_{o1}]$
### Cascode Amplifier with Current-Source Load
+ $A_V = -g_{m2} r_{o3} || [(1+g_{m1}r_{o1})r_{o2} + r_{o1}]$
### Cascode Amplifier with Cascode Load
![](/images/CascodeAmpCascodeLoad.png)
+ $A_V = -g_{m2} \{(1+g_{m3}r_{o3})r_{o4} + r_{o3}\} || \{(1+g_{m1}r_{o1})r_{o2} + r_{o1}\} \approx -g_{m2}  \{(g_{m3}r_{o3}r_{o4})  ||(g_{m1}r_{o1}r_{o2})\}$

### Question
![](/images/CascodeExp.png)
+ $A_V = - G_m R_{out, up} || R_{out, down}$
+ $G_m = g_{m2}$
+ $R_{out, up} = (1 + g_{m3}r_{o3})R_S + r_{o3}$
+ $R_{out, down} = (1 + g_{m1}r_{o1})r_{o2} + r_{o1}$

 
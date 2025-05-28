# Razavi Electronics 2, Lec 01, Cascode Current Sources

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Cascode Current Sources](#cascode-current-sources)


---
## Cascode Current Sources
+ Ideal Current Source: current is constant and independent of the voltage across 
+ Due to channel length modulation coefficient $\lambda > 0$ the CMOS in saturation region acts as a current source that its current is depentdent of the voltage across. (not flat )
+ And if the voltage across is lower than $V_{GS} - V_{TH}$, the CMOS leaves stauration region and goes to triode region.
+ In its small signal model, the finite output resistance $R_{out} = r_o$ 
### How do we improve this current source?
+ improve $R_{out} \to $ $r_o \uparrow $, so using degeneration 
+ $R_{out} = (1 + g_m r_o)R_S + r_o$, which $g_m r_o$ calls intrinsic gain 
+ The lowest $V_G$ to keep at saturation region is equal to $V_{GS} + I_DR_S -V_{TH} \uparrow$
+ So if $V_D \uparrow \to I_D\uparrow \to \text{lowest saturation voltage}\uparrow$
+ So using **cascode current source** to break up the ohm's law, just using CMOS $M_2$ replaces $R_S$
![](/images/CascodeCurrentSource.png)
    + $R_{out} = (1 + g_{m1} r_{o1})r_{o2} + r_{o1} \approx g_{m1} r_{o1}r_{o2}$ 
    + so the output resistance of cascode approximately equals to the intrinsic gain $g_{m1}r_{o1}$ times the output resistance of $M_2$

### Limitation of casacode current source?
+ Both MOS transistors must be in saturation region
+ $M_1$ is called output transitor, $M_2$ is called degenerating transistor, the source of $M_1$ has to connected to the drain of $M_2$ 

### Question: What happens to $R_{out}$ if double $W_1$ and $W_2$ and $I_D$ is constant? 
+ $R_{out} = g_{m1}r_{o1}r_{o2}$
+ $r_o = \frac{1}{\lambda I_D} \text{ with } I_D = \frac{1}{2}\mu_n C_{ox} \frac{W}{L}  (V_{GS} - V_{TH})^2$
+ $g_m = \sqrt{2\mu_n C_{ox}\frac{W}{L}I_D}$
+ so $R_{out} \to \sqrt{2}R_{out}$


 
# Razavi Electronics 2, Lec 02, MOS and Bipolar Cascode Current Sources, Intro. to Cascode Amplifiers

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [MOS & Bipolar Cascode Current Sources](#mos--bipolar-cascode-current-sources)
2. [P-Type Current Source](#p-type-current-source)
3. [Intro. to Cascode Amplifiers](#intro-to-cascode-amplifiers)

---
## MOS & Bipolar Cascode Current Sources
### Bipolar Cascode Current Sources
![](/images/BipolarCascodeCurrentSource.png)
+ Without degeneration: $R_{out} = r_o$
+ With degeneration: $R_{out} = (1 + g_{m1} r_{o1})(R_E || r_\pi) + r_{o1}$
+ Cascode: $R_{out} = (1 + g_{m1} r_{o1})(r_{o2} || r_{\pi_1}) + r_{o1}$

### Mixed MOS and Bipolar Cascode
![](/images/MixedCascode.png)
+ A: upper (M1), lower(Q2)
+ B: upper (Q2), lower(M1)
+ Assume $r_{o1} = r_{o2}$
+ $R_{outA} = (1 + g_{m1} r_{o1})r_{o2} + r_{o1} \approx g_{m1} r_{o1}r_{o2}$
+ $R_{outB} = (1 + g_{m2} r_{o2})(r_{o1} || r_{\pi_2}) + r_{o2} \approx g_{m2}r_{o2}(r_{o1}||r_{\pi_2})$

+ For a given biasing current, $g_{m, \text{MOS}} < g_{m, \text{bipolar}} \to g_{m1} < g_{m2}$
---
## P-Type Current Source
![](/images/P-TypeCascode.png)
+ A N-Type current source connects general circuits with GND
+ A P-Type current source connects positive supply with general circuits

---
## Intro. to Cascode Amplifiers
![](/images/G_m.png)
+ In general linear circuit, $G_m = \frac{I_{out}}{V_{in} }$
+ $R_{out} = \frac{V_x}{I_x}$
+ $\to A_V = \frac{V_{out}}{V_{in}} = - G_m R_{out}$
### Example
![](/images/G_mExp.png)
 
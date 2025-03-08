# Razavi Electronics 1, Lec 11, Full-Wave Rectifier 

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Full-Wave Rectifier](#full-wave-rectifier)




---
## Full-Wave Rectifier
### Basic Structure
+ Diode bridge: 4 diodes, the diode in the parallel sides have the same direction.
+ When $V_{in}$ is far postive, diodes $D_1$ and $D_3$ are on, $D_2$ and $D_4$ are off, $V_{out} = V_{in} - 2V_{D, on} $ is postive
+ When $V_{in}$ is far negative, diodes $D_2$ and $D_4$ are on, $D_1$ and $D_3$ are off, $V_{out} =  - V_{in} - 2V_{D, on}$ is postive

### Behavior with Load Cap. & Res.
+ With only capacitor, the $V_{out} > 0$ when the $V_{in} > 2V_{D, on}$, then go up to peak value $V_{peak} - 2V_{D, on}$ and keep unchanging
+ With only resistor, 
$$V_{\text{out}} = 
\begin{cases} 
\left| V_{\text{in}} \right| - 2V_{D,\text{on}} & \left| V_{\text{in}} \right| > 2V_{D,\text{on}} 
\\
0 & \left| V_{\text{in}} \right| \leq 2V_{D,\text{on}}
\end{cases}$$
+ With both capacitor and resistor, the capacitor discharge at $V_{peak} - 2V_{D, on}$, and charge at the point that $V_{out, Res} \geq V_{out, \text{Cap}}$

+ The amplitude of ripple(FWR): $\frac{V_{peak} - 2V_{D,on}}{R_1C_1}\cdot \frac{T_{in}}{2} $
+ The amplitude of ripple(HWR): $\frac{V_{peak} - V_{D,on}}{R_1C_1}\cdot T_{in} $
+ Example of Diode: Light Emitting Diode (LED)






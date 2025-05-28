# Razavi Electronics 1, Lec 43, Op Amp Circuits II

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Example Application](#example-application)
2. [Unity-Gain Buffer](#unity-gain-buffer)
3. [Integrator](#integrator)
4. [Differentiator](#differentiator)
5. [Voltage Adder](#voltager-adder)



---
## Example Application
![](/images/VoltageRegulator.png)
+ Voltage Regulator
    + If $V_{out}\uparrow \to V_{inv}\uparrow \to V_{G}\downarrow \to R_{on}\uparrow = \frac{1}{\mu_n\frac{W}{L}C_{ox}(V_{GS}-V_{TH})}\to V_{out}\downarrow$, a negative feedback

---
## Unity-Gain Buffer
![](/images/UnityGainBuffer.png)
+ A noninverting amplifier $A_V \approx 1 + \frac{R_2}{R_1}$, if $R_2 \to 0, R_1 \to \infty$
+ $\to A_V \approx 1$
+ The input impedance $\approx \infty \to $ can sense voltages without loading the circuit.
+ Its Thevevnin Equivalent Circuit:
    + $i_x = \frac{v_x + A_ov_x}{R_{out}} \to \frac{v_x}{i_x} = \frac{R_{out}}{A_o + 1}$
    + So it's  a very buffer  has very high $R_{in}$ and make the $R_{out}\downarrow$

---
## Integrator
![](/images/Integrator.png)
+ General Inverting Amplifier: $\frac{V_{out}}{V_{in}} \approx - \frac{Z_2}{Z_1}$
+ For integrator wenn $A_o $ is large: $\frac{V_{out}}{V_{in}} = - \frac{\frac{1}{C_1 S}}{R_1} = - \frac{1}{R_1C_1S}$ $\to$ Pole at origin
+ Circuit through $R_1 \approx \frac{V_{in}}{R_1}$, circuit through a capacitor $C\frac{dV}{dt}$
+ KCL: $\to - C_1 \frac{dV_{out}}{dt} = \frac{V_{in}}{R_1} \to V_{out} = - \frac{1}{R_1C_1} \int V_{in}dt$
### Example
![](/images/IntegratorExp.png)

+ What is the transfer function if $A_0$ is not very large:
    + $V_x = - \frac{V_{out}}{A_0}$
    + $\frac{V_{\text{in}} + \frac{V_{\text{out}}}{A_0}}{R_1} = -\frac{-\frac{V_{\text{out}}}{A_0} \frac{1}{C_1 s} - V_{\text{out}}}{\frac{1}{C_1S}}$
    + $\frac{V_{\text{out}}}{V_{\text{in}}} = \frac{-1}{\frac{1}{A_0} + \left(1 + \frac{1}{A_0}\right) R_1 C_1 s}$ $\to $ Pole not at origin (0)

+ **Unforunately, this integrator does not work in the lab!!**

---
## Differentiator 
![](/images/Differentiator.png)
+ $\frac{V_{out}}{V_{in}} = - \frac{R_1}{ \frac{1}{C_1 S}} = - R_1C_1S$
+  KCL: $\to C_1 \frac{dV_{in}}{dt} = -\frac{V_{out}}{R_1} \to V_{out} = - R_1C_1 \frac{dV_{in}}{dt}$

---
## Voltager Adder
![](/images/VoltageAdder.png)
+ $V_{out} = - R_F(\frac{V_{in1}}{R_1} + \frac{V_{in2}}{R_2})$
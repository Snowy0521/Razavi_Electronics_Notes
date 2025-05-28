# Razavi Electronics 1, Lec 42, Op Amp Circuits I

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Op Amp Basics](#op-amp-basics)
2. [Amplifiers Using Op Amps](#amplifiers-using-op-amps)



---
## Op Amp Basics
+ Two input terminals and one output terminal
+ Noninverting input $+$ and inverting input $-$
+ $V_{out} = (V_{noninv} - V_{inv})A_0$
![](/images/OpAmpInputOutputChar.png)
### Ideal Op Amp versus 741 versus Modern Integrated Op Amp
![](/images/OpAmpVersus.png)
+ If $V_{out} \approx \text{a few volts }, A_0 \approx 1000 \to V_{in1} - V_{in2} \approx \text{a few }mV$
+ If we can visualize a complex circuit as an Op Amp, the analysis becomes simpler.
![](/images/OpAmpSimpler.png)
---
## Amplifiers Using Op Amps
### Noninverting Amplifier
![](/images/NoninvertOpAmp.png)
+ Case I: $A_0 \to \infty$
    +  $V_{out} = (V_{in1} - V_{in2})A_0$
    + $V_{out}$ is finite, $V_{in1} - V_{in2}$ is very small and $A_0$ is very large $\to V_{in1} \approx V_{in2}$
    + $\frac{V_{out}}{R_1 + R_2} = \frac{V_{in}}{R_2}$
    + $\to \frac{V_{out}}{V_{in}} = 1 + \frac{R_1}{R_2}$
+ Case II: $A_0$ not very high
    + $V_x  = V_{out}\frac{R_2}{R_1 + R_2}$
    + $(V_{in} - V_{out}\frac{R_2}{R_1 + R_2})A_0 = V_{out}$
    + $\to \frac{V_{out}}{V_{in}} = \frac{A_0}{1 + \frac{R_2}{R_1 + R_2}A_0}$
    + $A_0$ : Open Loop Gain, $\frac{V_{out}}{V_{in}} = \frac{A_0}{1 + \frac{R_2}{R_1 + R_2}A_0}$: Closed Loop Gain
    + If $\frac{R_2}{R_1 + R_2}A_0 \gg 1 \to \frac{V_{out}}{V_{in}} \text{ relatively indepedent of } A_0$

#### Quiz
![](/images/OpAmpQuiz.png)
+ Due to $A_0$ is very large $\to V_{in} \text{ at noninverting input terminal}$
+ $V_{out} = \frac{V_{in}}{-g_mR_D} \to \frac{V_{out}}{V_{in}} = - \frac{1}{g_mR_D}$

### Inverting Amplifier 
![](/images/InvertOpAmp.png)
+ Case I: $A_0 \to \infty $
    + The voltage of noninverting input is zero so the inverting input must be close to zero $\to x \text{ is virtual GND}$
    + Current through $R_1 = \frac{V_{in} - V_x}{R_1} \approx \frac{V_{in}}{R_1}$
    + Assume input impedance of inverting input is very high, so the current go through $R_2$
    + KVL: $\frac{V_{in}}{R_1}R_2 = V_x(\approx 0) - V_{out}$
    + $\to \frac{V_{out}}{V_{in}} = - \frac{R_2}{R_1}$
    + Input Impedance $\approx R_1$

+ Case II: $A_0$ not very large
    + $V_x = \frac{V_{out}}{-A_0}$
    + KCL: $\frac{V_{in} + \frac{V_{out}}{A_0}}{R_1} = \frac{\frac{-V_{out}}{A_0} - V_{out}}{R_2}$
    + $\to \frac{V_{out}}{V_{in}} = \frac{-1}{\frac{R_1}{R_2} + \frac{1}{A_0}\frac{R_1+R_2}{R_1} }$
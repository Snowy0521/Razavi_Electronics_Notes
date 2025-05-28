
# Razavi Electronics 2, Lec 29, Application Examples of Feedback, Properties of Feedback Systems
This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Application Examples of Feedback](#application-examples-of-feedback)
2. [Summary of Feedback Concepts](#summary-of-feedback-concepts)
3. [Properties of Negative Feedback](#properties-of-negative-feedback)



 

---
## Application Examples of Feedback
+ Tow-Thomas Filter
+ Voltage Regulator
+ Paper: "Channel Selection at RF Using Miller Bandpass Filters" by Razavi

---
## Summary of Feedback Concepts
+ We sacrifice the open-loop gain to benefit from negative feedback
+ The feedback signal is a good copy(relica) of input signal
+ The $Y = \frac{U}{K}$ is a good copy of $X$ but with scaling factor. e.g., if $K = 0.1 \to Y = 10X$
+ The loop wants to make $Y$ a good (scaled) copy of $X$
+ If $k A_1 \gg 1 \to $ factors(Temperature, Supply Voltage, Frequency, Load Impedance) that cause $A_1$ to vary have less effect on the closed-loop gain

### Poor Man's Op Amp
![](/images/PoorManOpAmp.png)
+ $X - U = - (V_{in2} - V_{in1})$
+ $Y = A_1( X - U) = g_m R_D (V_{in2} - V_{in1})$

### Quiz
![](/images/QuizPoorManOpAmp.png)

---
## Properties of Negative Feedback
+ $\frac{Y}{X} = \frac{A_1}{1 + kA_1} \approx \frac{1}{K}, \text{if} KA_1 \gg 1$
+ Gain Desensitization $\frac{Y}{X}$ is less sensitive to temp., supply voltage, than $A_1$ is.
+ Bandwidth Extension: Greater Bandwidth for the close-loop system.
+ Modification of Input and Output Impedances.
+ Higher Linearity

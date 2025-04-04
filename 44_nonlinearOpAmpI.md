# Razavi Electronics 1, Lec 44, Nonlinear Op Amp Circuits, Op Amp Nonidealitites I

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Nonlinear Functions](#nonlinear-functions)
2. [Op Amp Nonidealities](#op-amp-nonidealities)



---
## Nonlinear Functions
### Precision Rectifier 
![](/images/PreciseRectifier.png)
+ For a simple rectifier, if the amplitude of $V_{in} < V_{D, \text{on}}$ is too small, the $V_{out} = 0$
+ So we need a precision rectifier to reduce the shift $V_{D, on}$

### Logrithmic Amplifier 
![](/images/LogrithmicAmplifier.png)
+ Current through $R_1 \approx \frac{V_{in}}{R_1} = I_{C1} = I_S \exp \frac{V_{BE}}{V_T}$ 
+ $V_{BE} = - V_{out} \to \frac{V_{in}}{R_1} = I_S \exp \frac{-V_{out}}{V_T} \to V_{out} = - V_T \ln\frac{V_{in}}{R_1I_S}$
+ If $V_{in} < 0$, output of op amp is not defined and died (saturated). so $V_{in} \geq 0 $ all the time.
+ What the bipolar is a PNP?
![](/images/PNPLogrithmicAmp.png)
    + $V_{in} \leq 0$ all the time
    + $V_{out} = V_T \ln\frac{-V_{in}}{R_1I_S}$


---
## Op Amp Nonidealities
+ Finite Gain
+ DC Offsets
![](/images/DCoffset.png)
    + An offset voltage ($V_{os}$) to make $V_{out} = 0$
    + $V_{os}$ is random 
    + $V_{os}$ can be placed in series with noninverting or inverting input terminal

![](/images/EffectOffsetAmp.png)
+ Input Bias Currents
+ Finite Speed 


 
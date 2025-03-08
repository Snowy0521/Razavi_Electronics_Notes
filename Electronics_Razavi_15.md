# Razavi Electronics 1, Lec 15, Transistor Biasing, Transconductance

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Simple Amp. Revisited](#simple-amp-revisited)
2. [Concept of Biasing](#concept-of-biasing)
3. [Concept of Transconductance](#concept-of-transconductance)




---
## Simple Amp. Revisited
+ $V_{out} = -I_C\cdot R_L = -R_L \cdot I_S(\exp(\frac{V_{BE}}{V_T}) -1)$
+ $I_S = 5 * 10^{-16} mA$, so for $V_{BE} = 10mA$, and requires a $V_{out} = 100mA$, after calculation,  $R_L = 4.25 * 10^{16}\Omega$, very impractical. so we can use biasing to increase $U_{BE} $
+ Due to the exponential function of $I_C$ and $U_{BE}$, the increment base on higher biasing is far larger than the base on lower biasing.
---
## Concept of Biasing
+ Provide proper voltage and current, so that the transistor can amplify.
+ Operating point: The bias values chosen for $V_{BE}$, $I_C$
+ A bipolar transistor can act as a voltage dependent current source => its collector current $I_C$ changes in response to its base-emitter voltage $U_{BE}$.
+ The operating point determines how the transitor responds.
+ Which operating point is **better**?, Case 1: $I_C = 1.7mA @ U_{BE}=750mV $ or Case 2: $I_C = 3.6mA @ U_{BE}=770mV $?
    + Case 2 is better due to strong response (better transconductance).


---
## Concept of Transconductance
+ $g_m = \left. \frac{dI_C}{dV_{BE}} \right|_{V_{CE} \, \text{const.}}$ with unit of siemens($S$)
* $g_m = \frac{d}{d_{BE}}(I_S\exp\frac{V_{BE}}{V_T} - 1) = \frac{I_S}{V_T}\exp\frac{V_{BE}}{V_T} \approx \frac{I_C}{V_T}$ 
+ if $I_C = 1 mA$ => $g_m = \frac{1mA}{26mV} \approx \frac{1}{25\Omega} = 0.04 S$
+ With no bias, $I_C = 0$ => $g_m = 0$ => no amplification
+ For amplification, need a certain $g_m$ => certain $I_C$ => certain $V_{BE}$
+ The tradeoff between $g_m$ and power consumption
+ $g_m$ calculation: $V_{CE}$ is constant, $V_{BE}$ is variable, determine $I_C$.

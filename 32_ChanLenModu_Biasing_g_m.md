# Razavi Electronics 1, Lec 32, Biasing, Transconductance

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Channel Length Modulation](#channel-length-modulation)
2. [Biasing](#biasing)
3. [Transconductance](#transconductance)





---
## Channel Length Modulation
+ As $V_{DS}\uparrow \to \text{channel length}:L\downarrow$
+ $I_D = \frac{1}{2}\mu_n C_{ox} \frac{W}{L}  (V_{GS} - V_{TH})^2(1 + \lambda V_{DS})$, where $\lambda$ is channel-length modulation coefficient.
--- 
## Biasing
+ To make sure the transistor operates in right saturation region.
+ Need to bias the transistor by creating proper current and terminal voltages.
+ So that the device can amplify the signal.
+ This MOSFET "converts" a voltage to a current, it acts like a $V/I$ converter $\to$ Transconductor 
---
## Transconductance
+ Concept of transconductance $g_m = \frac{dI_D}{dV_{GS}}$ with unit $\frac{1}{\Omega}, S(\text{siemens})$
+ with $I_D = \frac{1}{2}\mu_n C_{ox} \frac{W}{L}  (V_{GS} - V_{TH})^2(1 + \lambda V_{DS})$
+ $g_m = \mu_n C_{ox} \frac{W}{L}  (V_{GS} - V_{TH})(1 + \lambda V_{DS})$
+ $g_m = \frac{2I_D}{V_{GS} - V_{TH}}$
+ $g_m = \sqrt{2 I_D \, \mu_n C_{ox} \, \frac{W}{L}}$


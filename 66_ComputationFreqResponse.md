
# Razavi Electronics 2, Lec 21, Computation of Frequency Response, Frequency Response of Common-Emitter/Source Stages
This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [General Procedure for Computation of Freq. Response](#general-procedure-for-computation-of-freq-response)
2. [Frequency Response of Common-Emitter/Commmon-Source Stage](#frequency-response-of-common-emittercommmon-source-stage)



---
## General Procedure for Computation of Freq. Response
1. Draw the circuit
2. Draw all of the device capcitances
3. Remove or merge capacitors
4. Compute the transfer function, $H(S)$
5. $|H(s = jw)| \to \text{plot}$
6. Alternative for 4 and 5 (wenn transfer function is complicate): Find the poles by inspection 
---
## Frequency Response of Common-Emitter/Commmon-Source Stage
![](/images/FreqCECS.png)
+ The difference between Bipolar and MOSFET is Bipolar has $r_\pi$, the MOSFET has $r_\pi = \infty$, others are same.

![](/images/FreqMOSFETexp2.png)
![](/images/ResponseFreqCE.png)
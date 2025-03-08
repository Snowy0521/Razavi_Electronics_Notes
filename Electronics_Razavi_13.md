# Razavi Electronics 1, Lec 13, Bipolar Transistor Structure & Operation
This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Structure and Symbol of Bipolar Transistor](#structure-and-symbol-of-bipolar-transistor)
2. [Bipolar Transistor Operation](#bipolar-transistor-operation)




---
## Structure and Symbol of Bipolar Transistor
+ Three sections (N-P-N or P-N-P), here we focus on NPN first.
+ Asymmetric doping, bottom section($n^+$) is heavily doped (more frei electrons), its called Emitter($E$)
+ The up section(n) is collector($C$), and the mittel section is called base($B$)
+ Active Forward Bias/Region 
    + The pn-junction between $B$ and $E$ is forward biased
    + The pn-junction between $B$ and $C$ is zero or reverse biased
    + The $B$ must be more postive than $E$ by $$V_{D, on} \approx (700, 800)mV$$
    + The $C$ must be more postive than $B$ or zero different.
+ Base region is very thin and the distance between two pn-junctions are very short



---
## Bipolar Transistor Operation
+ Base emitter voltage: $V_{BE} = 0.8V$
+ $V_{CB} = V_{CE} - V_{BE} \geq 0$ => $V_{CE} \geq V_{BE} = 0.8 V$
+ Concept of carrier injection
    + Inject electrons to depletion region on the P side(electrons) of reverse bias PN-Junction
    + the electrons due to electric field are pushed to N side(holes), absorded by N-section and battery.
+ so electrons from $E$ travel through base($B$) and injected in P side of depletion region and travel to $C$ 
+ so equivalently, the current is flowing from collector $C$ to emitter $E$

### Question: By what mechanism do electrons flow through the base: drift or diffusion?
 + Base region is thin and sustains little voltage => neligible drift current
 + The carrier(electrons) density between $E$ and depletion region make a diffusion 

### What happens if $V_{BE}\uparrow?$
+ **more electrons, higher current ${I_{CE}\uparrow}$**
+ $V_{BE}\uparrow, I_{CE}\uparrow$
+ $I_{CE} = I_S(\exp\frac{V_{BE}}{V_T}) - 1$
---

# Razavi Electronics 1, Lec 24, Biasing Techniques I

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Examples of Degenerated Current Sources](#examples-of-degenerated-current-sources)
2. [Simple Biasing Techniques](#simple-biasing-techniques)






---
## Examples of Degenerated Current Sources
+ ![Examples of Degenerated Current Sources](/images/ExamplesDegeneratedCurrentSources.png)

---
## Simple Biasing Techniques
+ We donot need a battery for each terminals, just use resistive divider. but what happens to the input impedance?
    + $R_{in} = r_\pi||R_1||R_2$, $R_1||R_2$ should be preferably much greater than $r_\pi$.

+ How about the base current $I_B$?
    + $I_B \ll \frac{V_{CC}}{R_1 + R_2}$ to reduce sensitivity.
    + ![](/images/BiasingCEbipolar.png)

+ How do we interface this circuit with the preceding stage?
    + Design preceding stage for $V_{out} \approx 0.8 V$ and connect directly. (dc coupling)
    + Using ac coupling, a capacitor between preceding stage and the following stage for different dc voltage, the capacitor make no interaction between them.

+ How do we choose a capacitor?
    + $Z_C = \frac{1}{jwC}$
    + a good capacitor means even at lower frequency, it acts like a reasonable short circuit.
    + A reasonable short circuit means it has **much lower impedance** than the $R_{in} = r_\pi||R_1||R_2$

+ Design Procedure for simple Biasing 
    + We have $I_C$ in mind, then we determine $I_B$ by divided it of factor $\beta$
    + We can pick $\frac{V_{CC}}{R_1 + R_2} \approx 10I_B \gg I_B $ and $V_{BE} = \frac{R_2}{R_1 + R_2}V_{CC} \approx 0.8V$

+ Problem of Supply Sensitivity
    + Suppose $V_{CC}\uparrow$ by $5\% \to V_{BE}\uparrow $ by $5\%$
    + If $V_{BE} = 800mV \to \Delta V_{BE} = 40mV$
    + $I_C \uparrow $ by $\exp\frac{40mV}{26mV} = 4.65$ fold, its hugh and we cannot tolerate them.
    + Using CE-Stage with Degeneration to solve it.



    
    

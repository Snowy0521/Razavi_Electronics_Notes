# Razavi Electronics 1, Lec 14, Bipolar Transistor Characteristics, Intro. to Biasing

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Basic Properties of Bipolar Transistors](#basic-properties-of-bipolar-transistors)
2. [Terminal Currents](#terminal-currents)
3. [Concept of Bias](#concept-of-bias)




---
## Basic Properties of Bipolar Transistors
+ $I_C = I_S(\exp(\frac{V_{BE}}{V_T}) - 1)$
+ $I_S = \frac{A_E \cdot q \cdot n_i^2 \cdot D_n}{W_BN_B}$, where $A_E$ is emitter area, $W_B$ is base width, $N_B$ is the doping in base
+ How much does $I_C$ change if $V_{BE}$ increases by $60mV$? ($V_{CE}$ is constant)
    + By factor of 10
+ In most cases, $I_C \approx I_S\exp(\frac{V_{BE}}{V_T})$ => $V_{BE} = V_T\ln \frac{I_C}{I_S}$

### Example: We double the area of a transistor and decrease its base-emitter voltage by $60mV$, what the change in the collector current?
+  factor of 5 reduction in the current

+ What the characteristic of $I_C$ and $V_{CE}$?
    + A constant value of $I_C$, it changes not with $V_{CE}$
    + so we can put the bipolar transistor into a black box, due to its $I_C$ donot change with $V_{CE}$, so its an **ideal current source**.
    + The $I_C$ increases with $V_{BE}$, so this bipolar transistor is a **voltage dependent current source**.

---
## Terminal Currents
+ $I_C \approx I_S\exp(\frac{V_{BE}}{V_T})$
+ The number of holes from $I_{B}$ is proportional to the number of electrons of $I_{C}$.
+ $I_B \propto I_C: I_C = \beta I_B, \beta \gg 1: (50, 200)$, where $\beta$ is current gain.
+ $I_B = \frac{I_S}{\beta}\exp(\frac{V_{BE}}{V_T})$
+ $I_E = I_B + I_C = \frac{\beta+1}{\beta}I_S\exp(\frac{V_{BE}}{V_T})$ accoding KCL

### Example: A bipolar transistor has a collector current of 1mA and $I_S = 10^{-16}A$, How much is $V_{BE}$? ($V_T$ is 26mV@roomTemp)
+ $V_{BE} = V_T\ln \frac{I_C}{I_S} = 778 mV$
+ If $\beta = 50$, $I_B = \frac{I_C}{\beta} = 20 \mu A$

---
## Concept of Bias
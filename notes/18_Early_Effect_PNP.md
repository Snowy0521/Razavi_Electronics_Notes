# Razavi Electronics 1, Lec 18, PNP Transistor

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Inclusion of Early Effect in Small-Signal Model](#inclusion-of-early-effect-in-small-signal-model)
2. [PNP Transistor](#pnp-transistor)




---
## Inclusion of Early Effect in Small-Signal Model
+ Official method of small-signal model derivation
    1. Assume the transistor is biased at a certain operating point.
    2. Apply a voltage change between two terminals and measure the resulting current changes.
    3. Model the current changes by proper electric devices.

+ $g_m = \frac{d}{d_{BE}}(I_S\exp\frac{V_{BE}}{V_T})(1 + \frac{V_{CE}}{V_A}) = \frac{I_S}{V_T}\exp\frac{V_{BE}}{V_T} (1 + \frac{V_{CE}}{V_A}){V_T} \approx \frac{I_C}{V_T}$, where $V_A$ is Early Voltage.

+ ![Small Signal Model for Bipolar Transistor with Early Effect](/images/SmallSignalModelBipolarEarlyEffect.png)

+ If $V_{CE} < V_{BE}$, the bipolar transistor in saturation region due to both forward bias junction. The saturation region should be avoided.

+ ![Example of Bipolar Transistor with Early Effect](/images/EarlyEffectBipolarExample.png)
---
## PNP Transistor
+ ![Bipolar PNP Symbol](/images/BipolarPNPSymbol.png)
+ ![](/images/3RegionsBipolar+PNPLargeSignalModel.png)

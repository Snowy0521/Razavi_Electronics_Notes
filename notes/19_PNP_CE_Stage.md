# Razavi Electronics 1, Lec 19, Evolution of Amplifiers

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Small-Signal Model of PNP Transistor](#small-signal-model-of-pnp-transistor)
2. [Introduction to Amplifiers](#introduction-to-amplifiers)
3. [Common-Emittler Topology](#common-emittler-topology)




---
## Small-Signal Model of PNP Transistor
+ Identical to small-signal model of npn transistor
+ ![Small Signal Model PNP-Bipolar](/images/SmallSignalModelPNPBipolar.png)
+ The voltage $V_{\pi}$ has positive at the base and negative terminal at the emitter, regardless what type of transitor it is.
---
## Introduction to Amplifiers
+ Design Procedure
    + Select a topology
    + Create proper bias conditions for all transistors
    + Analyze the small-signal properties of the amplifier and see if they are satisfactory.

+ Amplifier Characteristics
+ $\text{Voltage Gain}: A_V = \frac{\text{Output Swing}}{\text{Input Swing}}$
+ Power Consumption: bias currents drain the battery.
+ Amplifier has a voltage dependent current source converts voltage to current, first $V/I$ conversion, then $I/V$ conversion.
---
## Common-Emittler Topology
+ Problem with the topology only $R_L$, the device is dead and in saturation region
    + ![saturation region](/images/BipolarSaturation.png)
    + $V_{out} = V_{CE} = -1V$
+![common emitter topology of bipolar transistor](/images/CommonEmitterBipolar.png)
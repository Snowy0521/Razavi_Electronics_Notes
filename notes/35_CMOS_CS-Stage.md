# Razavi Electronics 1, Lec 35, Common-Source Stage I

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [CMOS Technology](#cmoscomplementary-mos-technology)
2. [Introduction to CMOS Amplifiers](#introduction-to-cmos-amplifiers)
3. [The Common-Source Topology](#the-common-source-topology)





---
## CMOS(Complementary-MOS) Technology
+ In NMOS, the terminal between source and drain, which one has lower potential, which acts as source.
+ In PMOS, the terminal between source and drain, which one has higher potential, which acts as source.

### Radar Operation Application
+ Transmitter (TX) has an oscillator for generating wave, a PA(power amplifier) and an antenna for transmitting wave
+ Receiver (RX) has an antenna for receiving wave, a LNA (low-noise amplifier) and processing unit for measuring speed and distance
--- 
## Introduction to CMOS Amplifiers
+ Amplifier Design Procedure:
    1. Select an amplifier topology.
    2. Bias the transistor(s) to obtain proper values for $g_m$, $r_o$...
    3. Determine the characteristics of the circuit.
+ Amplifier Characteristics:
    1. Gain, Voltage Gain $A_V$
    2. Power Dissipation 
    3. ...
---
## The Common-Source Topology
+ A NMOS transistor combine with a resitor $R_D$ with it's Drain Terminal 
+ Input applied to gate, output sensed at drain.
![](/images/CS-Stage_SmallSignal.png)
+ $A_V = -g_m R_D$

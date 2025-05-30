# Razavi Electronics 1, Lec 6, Diode Models

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Diode Models](#diode-models)
2. [Reverse Breakdown](#reverse-breakdown)
3. [Circuits Examples](#circuits-examples)
4. [Bluetooth Receiver](#bluetooth-receiver)

---
## Diode Models
+ Constant Voltage Model
    + Approximation:
        * if $V_D < V_{D, on}$, diode off, $I_D = 0$
        * if $V_D >= V_{D, on}$, diode on, $\frac{dI_D}{dt} = +\infty$, resistance $R = 0$
        * $V_{D, on}$ in range of $(700, 800)mV$

+ An Ideal Diode Model 
    + $V_{D, on} = 0$

---
## Reverse Breakdown
+ Reverse voltage $V_R$ large enough, causes large reverse current $I_R$.
+ Damage to diode 
---
## Circuits Examples
+ [See video tutorial](https://www.youtube.com/watch?v=EnA9m7TOaoI&list=PLyYrySVqmyVPzvVlPW-TTzHhNWg1J_0LU&index=6&ab_channel=BehzadRazavi%28LongKong%29)

--- 
## Bluetooth Receiver
+ Low-Noise amplifier to amplify the small signal 
+ FM Demodulator to decode the low frequency information signal from high frequency carrier signal 
+ A/D Converter 
+ Processing 

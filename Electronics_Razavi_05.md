# Razavi Electronics 1, Lec 5

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [PN-Junction in Forward Bias](#pn-junction-in-forward-bias)
2. [Modeling the PN-Junction](#modeling-the-pn-junction)
3. [Reverse Breakdown](#reverse-breakdown)
4. [Quiz](#quiz)

---
## PN-Junction in Forward Bias
+ For a battery with forward bias voltage $V_F$, positive of battery connects to p-side, negative of battery connects to n-side.
+ electrons are pushed from n-side to p-side, holes are pushed from p-side to n-side, causes current can go on indefinitely.
+ The equation of forward bias current $I_{D}=I_{S}\left(exp\frac{V_{D}}{V_{T}}-1\right)$, where $I_S$ is reverse saturation current and $V_T = \frac{kT}{q}$
+ When $V_D$ is negative and its absolute value more large than $V_T$, then $I_D \approx -I_S$, that why call $I_S$ reverse saturation current (very very small).
    * $I_S = A \cdot q \cdot n_i^2 \cdot (\frac{D_n}{N_aL_n} + \frac{D_p}{N_dL_p} )$, where A is cross section area of junction, $n_i$ is intrinsic density of electrons and holes, $L_n$ and $L_p$ are diffusion lengths.

+ When $V_D$ is postive and its value more large than $V_T$, then $I_D \approx I_S \cdot e^\frac{V_D}{V_T}$, neglect the 1.

+ Diode: A two-terminal device that carries current when its voltage is positive and no current when its voltage is negative.
    + Positive: Anode
    + Negative: Cathode

+  Typical forward-bias voltages for diodes are in the range of $700-800 mV$



---
## Modeling the PN-Junction
+ Exponential Model: $I_D = I_S \cdot e^\frac{V_D}{V_T}$
    + the exponential function is not efficient to represent the diode in circuit by hand-on calculating.

---
## Reverse Breakdown






--- 
## Quiz
1. What the value of voltage in two terminal of diode, wenn the diode is connected forward bias with current source $I_1$?
+ According the equation $I_D \approx I_S \cdot e^\frac{V_D}{V_T}$, the voltage $V_D = V_T \ln \frac{I_D}{I_S}$

+ If $I_S = 10 ^ {-16} A$ and we measure a forware-bias current of $1mA$, what voltage is applied to the diode?
    + $V_D = V_T \ln \frac{I_D = 1mA}{I_S=10^{-16}A} = 778 mV$

+ How much should the voltage increase to raise the current by a factor of 10?
    + $V_{D1} = V_T \ln \frac{I_{D1}}{I_S} $
    + $V_{D2} = V_T \ln \frac{I_{D2}}{I_S} $
    + $V_{D2} - V_{D1} = V_T \ln \frac{I_{D2}}{I_{D1}}$
    + so, for 10 times increasing in current, we need to increase the voltage by $V_T \ln 10 \approx 60 mV$
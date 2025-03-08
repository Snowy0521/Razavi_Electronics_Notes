# Razavi Electronics 1, Lec 4, PN Junction in Equilibrium and Reverse Bias

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [PN-Junction in Equilibrium](#pn-junction-in-equilibrium)
2. [PN-Junction in Reverse Bias](#pn-junction-in-reverse-bias)
3. [Application: Bluetooth](#application-bluetooth)
4. [Quiz](#quiz)

---
## PN-Junction in Equilibrium
+ $J_{drift} = (\mu_n n + \mu_p p)E \cdot q$
+ $J_{diffusion} = (D_n \frac{dn}{dx} - D_p \frac{dp}{dx})q$ 
+ Equilibrium condition:
    + Diffusion current of electrons = Drift current of elctrons
    + Diffusion current of holes = Drift current of holes => $D_p \frac{dp}{dx} = \mu_p \cdot p\cdot E$
+ After integrate both sides:
$\int_{P_n}^{P_p} D_p \frac{dp}{p} = \mu_p \int_{x_1}^{x_2} E dx$, where ${P_n} = \frac{n_i^2}{N_d}$ and ${P_p = N_a}$ are the density of holes in n-side and p-side, the $x1$ and $x2$ are the left side and right side of depetion region.
+ leveaging the equation of $V_{AB} = -\int_{B}^{A} E  dx$ => $D_p \ln \frac{P_p}{P_n} = \mu_p (V_{x_1} - V_{x_2})$
+ leveaging the Einstein's relation $\frac{D}{\mu} = \frac{kT}{q}$ => Built-in Voltage $V_0 = V_{x_1} - V_{x_2} = \frac{kT}{q} \ln \frac{N_a N_d}{n_i^2}$, where $\frac{kT}{q}$ = 26mV@300k
+ Same $V_0$ expression is obtained if the electron currents are considered
+ If $N_a$ and $N_d$ are on the order of $10^{16}/cm^3$, $V_0 \approx 26 \cdot \ln \frac{10^{32}}{10{20}} \approx 720 mV$, so typical values of $V_0$ are from $700$ to $800 mV$
+ We cannot measure $V_0$ from outside
    
--- 
## PN-Junction in Reverse Bias
+ For a battery with reverse bias voltage $V_R$, positive of battery connects to n-side,
negative of battery connects to p-side.
+ some electrons from n-side remove to postive of battery, some holes go to negative of battery, cause depletion region **wider**.
+ leveaging equation $C = \frac{{\epsilon_0 A}}{d}$, in reverse bias, the $d\uparrow$, so $C\downarrow$
+ its called electronically-variable capacitor "varactor":
    + $C_j = \frac{C_{j0}}{\sqrt{1 - \frac{V_R}{V_b}}}$, which $C_j$ is capacitance of varactor, $V_R$ must be reverse bias (negative)
    + So, the PN-Junction in reverse bias can be used in oscillator to generate signal with different level of  frequency.


---
## Application: Bluetooth
+ Wireless communication between two devices such as laptop and printer.
+ The transmission rate of laptop is around $1 Mb/s$
+ But it has a very small antenna, a rate $2.4$ GHz is needed.
+ So an oscillator between them using Frequency Modulation(FM) carry information and achieve high frequency.
+ A power amplifier is needed to oppose signal degeneration.

--- 
## Quiz
1. Is there an electric field outside the depletion region?
    + no, the electric field only exists in depletion region, not outside.
    + Gauss's law: the amount of electric field is proportional to the charge enclosed by the surface.
    + In the edge of depetion region, the charge are zero due to postive ions and negative ions.
    + no electric flux, no electric field


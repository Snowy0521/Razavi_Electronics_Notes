# Razavi Electronics 1, Lec 2, Doping, Drift

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Doping](#doping)
2. [Movement of Charge](#movement-of-charge)
3. [Quizs](#quizs)



---
## Doping
### n-type and p-type semiconductors
+ If we add $N_d$(d for donor) donor atoms, then the density of free electrons is equal to $N_d/cm^3$
+ $n:$ density of free electrons
+ $p:$ density of holes
+ For pure Si: $n = p = n_i$ => $n*p = n_i ^2$
+ For doped Si: $n*p = n_i ^2$
### modified carrier densities
* For n-type Si: $n$ approx. $N_d$, so $p = 
        \frac{n_i^2}{N_d}
    $, so amount of holes becomes very small.
* For p-type Si(substitude with boron), majority carriers are holes, miniority carriers are electrons
    * Add $N_a$(a for acceptor) boron atoms per $cm^3$
    + $p = N_a$
    + $np = n_i^2$ => $n = \frac{n_i^2}{N_a}$





 


---
## Movement of Charge (Carrier Transport)

### Drift
+ The velocity ($v$ with unit of $m/s$) of electrons is proporational to electric field ($E$) $v \propto E$, $v = \mu_n E$
    + $\mu_n = 1350 (m^2/(Vs))$ is electron mobility
    + $ E = \frac{V_B}{L} $

    * $ \text{Total charge} = v \cdot W \cdot h \cdot n \cdot q $

    * $|I| = \mu_n \frac{V_B}{L} \cdot W \cdot h \cdot n \cdot q $

    * $R = \frac{L}{\mu_n \cdot W \cdot h \cdot n \cdot q} = \frac{1}{\mu_n \cdot  n \cdot q} \frac{L}{A} $ with (Eq. $R = \rho \frac{L}{A}$)=> $\rho = \frac{1}{\mu_n \cdot  n \cdot q}$

    * Current Density $J_n = \frac{I}{A = W \dot h} =  \mu_n \cdot E \cdot n \cdot q [A/cm^2]$ 

    * Generall, the total current density (Drift) $J_{drift} = (\mu_n \cdot n + \mu_p \cdot p)E \cdot q$
        - $E$: Electric field.
        - $V_B$: Applied voltage across the Si piece .
        - $L$: Length of the material (distance between two electrodes).
        - $v$: Drift velocity of charge carriers.
        - $W$: Width of the sample.
        - $h$: Height (or thickness) of the sample.
        - $n$: Number of charge carriers per unit volume (carrier concentration).
        - $q$: Charge of each carrier (elementary charge, \( e = 1.602 \times 10^{-19} \, C \)).
        - $\mu_n$: Mobility of charge carriers (electrons).
        - $I$: Electric current flowing through the Si piece.
        - $R$: Resistance.



---
## Quizs
1. What happens to n and p in n-type Si as T increases?
+ for n-type =>  $n = N_d$, $p = \frac{n_i^2}{N_d}$
+ so the number of free electrons ($n$) approximate keep constant due to the number of donor atoms is constant.
+ the number of holes($p$) rises rapidly with temperature
+ Sum up, as T increases, majority carriers keep constant, miniority carriers increase rapidly.
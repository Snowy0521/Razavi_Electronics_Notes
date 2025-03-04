# Razavi Electronics 1, Lec 1

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Introduction](#introduction)
2. [Seminconductor Physics Basics](#seminconductor-physics-basics)
3. [Questions](#questions)



---

## Introduction
+ Basic electric components such as resistor, capacitor, and indutor are two terminal, thus difficult to build useful circuits.
+ With other electronic components such as diode, bipolar transistor, MOS transistor, and op amp we can build more complex and useful circuits.

+ we will going to the internal of those electronic components.
    * For capacitor, 
    $
        i = C\frac{dV}{dt}
    $
    * For other components such as diode, what mathematical expression?
    * what the circuits with those components?
        + Diode circuits
        * Bipolar circuits
        + Mos circuits
        * op amp based circuits

+ Antenna example
    * transmitter:
        + Equation of wave frequency ($f$), wavelength($\lambda$) and speed of light ($c = 3*10^8 m/s$)
        $$
            \lambda = \frac{c}{f}
        $$
        + For half-wavelength antenna, the relationship of Antenna length($L$) and $\lambda$
        $
            L = \frac{\lambda}{2}
        $
        + For quarter-wavelength:
        $
            L = \frac{\lambda}{4}
        $
        * It means, lower frequency audio signal in range of($20 Hz$ to $20 kHz$) suit not for the size of antenna. what we going do?
        * so we need a carrier with higher frequency such as $1GHz$
            + A modulator combine low frequency information signal with carrier 
        * A power amplifier between modulator with antenna increases power for long distance transmission.
        * An oscillator generates the periodic carrier signal.
    
    * receiver
        + An antenna
        + An low noise amplifier 
        + A speaker 



---
## Seminconductor Physics Basics
### General Concepts
* valence elctrons in:   
    + sodium: 1 (unstable)
    + neon: 8 (stable)
    + silicon: 4 (semi-stable)

* Concept of Bandgap Energy
    * As temperature goes up, the density of free elctrons in Si increases.
    + The bandgap energy means the energy an electron needs to be free from bond of atom
    +  pure silicon aka intrinsic Si is a poor conductor due to poor amount of free electrons
    + For Si, $T=300k$, $n_i$(density of free electrons) approx equal to $10^{10}$ electrons per $cm^3$

* Concept of Holes
    * when an electron is gone due to high thermal energy, the bond is missing an electron, we call its a hole
    * positive charge associated to hole, negative charge associated to electrons
    * In different times, free electrons can moved between each bonds to fill the holes, make it look like holes travel and carries conducation.
    * The density of holes is equal to density of electrons 

### Doping
+ Add some boron(3 electrons) or phosphorus(5 electrons) in pure silicon piece, it is doping 

 

---

## Questions
1. Where do change carriers come from?
    + increases the thermal energy, temperature
2. What types of charge carriers do we have?
    + electrons
    + holes
3. How can we modify the density of charge carriers?
    + doping 
4. How do charge carriers move?

5. Why are holes slower than electrons?
    + Movement of holes is based on release and trap mechanisms.
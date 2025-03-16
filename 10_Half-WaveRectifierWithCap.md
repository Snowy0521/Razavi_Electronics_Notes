# Razavi Electronics 1, Lec 10, Half-Wave Rectifier with Different Loads

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Half-Wave Rectifier with Smoothing Cap.](#half-wave-rectifier-with-smoothing-cap)
2. [Full-Wave Rectifier](#full-wave-rectifier)



---
## Half-Wave Rectifier with Smoothing Cap.
+ replace the output resistor with a capacitor.
+ At the peak voltage of sinusiod input, the $V_{out} = V_{peak} - V_{D, on}$, then the $V_{out}$ keeps so on due to the capacitor cannot discharge.
+ Issues:
    + Reverse voltage across diode $D_1$ is $2V_{peak} - V_{ D,on}$
+  Role of ${R_1}$ in the original circuit with diode no cap.?
    + when no resistor and diode is off, we do not know what is $V_{out}$, because the $V_{out}$ can be zero only zero current through a finite impedance.
+ Cam we plot input-output characteristic for the rectifier with capacitor?
    + $I = C \frac{dV}{dt}$, we do not know I/V characteristic without time response.

+ How about half-wave rectifier with cap. and load (resistor)?
    + Diode $D_1$ turns off after the peak voltage.
    + If we have a capacitor that is charged and a resistor is connected to it, the resistor voltage will decay exponentially util to nex periodic diode is on and charge the cap. again. it called ripple.
    + The ripple can cause noise and must be minimized.
    + If ripple is small => decay lasts about $T_{in}$(the period of the input from peak to peak)

+ The circuit of resistor $R_1$ and capacitor $C_1$ im parallel
    + the voltage $V_{out}$ duration is $V_{out} = V_1 \exp \frac{-t}{\tau = R_1C_1}$
    + if $t << \tau$ => $V_1\exp \frac{-t}{\tau} \approx V_1 (1 - \frac{t}{\tau})$
    + so for the half-wave rectifier, $V_{out} = (V_{peak} - V_{D,on})(1 - \frac{t}{\tau})$
    + The amplitude of ripple: $V_{out}(t = 0) - V_{out}(t = T_{in}) = (V_{peak} - V_{D,on})\frac{T_{in}}{\tau} = \frac{V_{peak} - V_{D,on}}{R_1C_1f_{in}} $

  









# Razavi Electronics 1, Lec 27, Emitter Followers

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Emitter Follower Topology](#emitter-follower-topology)
2. [Basic Properties](#basic-properties)



---
## Emitter Follower Topology
+ ![](/images/EmitterFollower.png)
+ It's called Common Collector Stage in some old books
+ with $V_A = \infty$ , $A_V = \frac{v_{out}}{v_{in}} = \frac{R_E}{\frac{1}{g_m} + R_E}$
+ In generall, $A_V = \frac{\text{Resistance tied between emitter and GND}}{\text{Resistance tied between emitter and GND} + \frac{1}{g_m}}$

### Questions
+ Do these results changes if we insert a resistor in the collector?
    + No, no effect to the equation derivation

+ A cascaded Emitter Follower with CE-Stage, what is the $A_V$?
    + ![](/images/CascadeEmitterFollowerCE.png)
    + $A_V = \frac{V_{out}}{V_{in}} = \frac{V_{out}}{V_{x}} \frac{V_{x}}{V_{in}}$
    + $\frac{V_{x}}{V_{in}} = \frac{R_E || r_{\pi2}}{R_E || r_{\pi2} + \frac{1}{g_{m1}}}$
    + $\frac{V_{out}}{V_{x}} = -g_{m2}R_C$

+ A cascaded Emitter Follower with CB-Stage, what is the $A_V$?
    + ![](/images/CascadeEmitterFollowerCB.png)
    + $\frac{V_{x}}{V_{in}} =\frac{R_E || \frac{1}{g_{m2}}}{R_E || \frac{1}{g_{m2}} + \frac{1}{g_{m1}}}$
    + $\frac{v_{out}}{v_{in}} = g_{m2}R_C$
---
## Basic Properties
+ $R_{in} = r_\pi + (\beta + 1)R_E$
+ $R_{out} = \frac{1}{g_m}||R_E$
    + $v_\pi = -v_x$, $-\frac{v_x}{r_\pi} - g_mv_x + i_x = 0 \to \frac{v_x}{i_x} \approx \frac{1}{g_m}$
    

### Example 
+ What the gain for an Emitter Follower with a resistor $R_B$ at base terminal
    + ![](/images/EmitterFollowerWithR_B.png)
    + $\frac{v_x}{v_{in}} = \frac{r_\pi + (\beta + 1)R_E}{r_\pi + (\beta + 1)R_E + R_B} \approx \frac{\frac{1}{g_m} + R_E}{\frac{1}{g_m} + R_E + \frac{R_B}{\beta + 1}}$
    + $\frac{v_{out}}{v_x} = \frac{R_E}{R_E + \frac{1}{g_m}}$
    + $\frac{v_{out}}{v_{in}} = \frac{R_E}{\frac{1}{g_m} + R_E + \frac{R_B}{\beta + 1}}$
    + $R_{in} = R_B + r_\pi + (\beta + 1)R_E$
    + $R_{out} = R_E || (\frac{1}{g_m} + \frac{R_B}{\beta + 1})$
    

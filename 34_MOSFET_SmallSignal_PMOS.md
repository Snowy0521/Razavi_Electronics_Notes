# Razavi Electronics 1, Lec 34, MOS Small-Signal Model, PMOS Device

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [More on Large-Signal and Small-Signal Models](#more-on-large-signal-and-small-signal-models)
2. [Inclusion of Channel-Length Modulation](#inclusion-of-channel-length-modulation)
3. [PMOSFETs](#pmosfets)





---
## More on Large-Signal and Small-Signal Models
### Small-Signal Models of Const. Souces
+ **Constant Voltage Souce** is a zero voltage source in the small signal model because its voltage change zero with time
+ A zero voltage source equivalent to a wire. **Short circuit**
+ In same way, a **constant current source** changes zero with time, its a zero current source, equivalent to an **open circuit**.

![](/images/MOSFET_small_signal_channel_length_mod.png)
![](/images/MODFET_channel_length_mod_ro.png)
+ $r_o = \frac{1}{\lambda I_D} \text{ with } I_D = \frac{1}{2}\mu_n C_{ox} \frac{W}{L}  (V_{GS} - V_{TH})^2$
--- 
## Inclusion of Channel-Length Modulation
### Example
$V_{GS} = 1.2 V, V_{DS} = 1 V, \mu_n C_{ox} = 100 \mu A/V^2, \frac{W}{L} = 10, V_{TH} = 0.5V, \lambda = 0.2 V^{-1}$ was is the small-signal model?
+ $V_{DS} > V_{GS} - V_{TH} \to \text{Saturation Region}$
+ $g_m = \mu_n C_{ox}\frac{W}{L}(V_{GS} - V_{TH}) = 0.7 mS = \frac{1}{1.43 k\Omega}$
+ $r_o = \frac{1}{\lambda I_D} \text{ with } I_D = \frac{1}{2}\mu_n C_{ox} \frac{W}{L}  (V_{GS} - V_{TH})^2 \to r_o = 20.4 k\Omega$
+ $A_V = g_m r_o \approx 14 \gg 1$



---
## PMOSFETs
![](/images/MOSFET_PNP.png)
+ $V_G < V_S, V_{TH} < 0, V_D < V_S$
+ $V_{SD} \geq V_{SG} - |V_{TH}| \to $ Saturation region, $I_D = - \frac{1}{2}\mu_n C_{ox} \frac{W}{L}  (V_{SG} - |V_{TH}|)^2(1 + \lambda V_{SD}), \lambda > 0$
+ $V_{SD} < V_{SG} - |V_{TH}| \to $ Triode region, $I_D \approx \mu_n c_{ox}\frac{W}{L}(V_{SG}-|V_{TH}|)V_{SD}$

![](/images/PMOS_small_signal_model.png)

![](/images/Inverter_small_signal_model.png)
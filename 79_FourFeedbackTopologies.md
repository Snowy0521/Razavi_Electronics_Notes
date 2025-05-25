
# Razavi Electronics 2, Lec 34, Four Feedback Topologies, Voltage-Voltage (Shunt-Series) Feedback
This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Four Feedback Topologies](#four-feedback-topologies)
2. [Voltage-Voltage (Shunt-Series) Feedback](#voltage-voltage-shunt-series-feedback) 



 

---
## Four Feedback Topologies
![](/images/FourFeedbackTopologies.png)

---
## Voltage-Voltage (Shunt-Series) Feedback
![](/images/ShuntSeriesFeedback.png)
![](/images/ShuntSeriesFeedback2.png)
+ Shunt means parallel
+ Ideal input and output impedance
    1. A voltage amplifier $A_1$ wants sense voltage source and donot disturb it, the $Z_{A_1, in} \to \infty$
    2. The voltage amplifier acts as a voltage source so it's $Z_{A_1, out} \to 0$
    3. The feedback network $K$ wants measure/sense the output voltage as a voltage meter, so it's $Z_{K, in} \to \infty$
    4. The feedback network $K$ returns its voltage to input voltage source as a voltage source, so $Z_{K, out} \to 0$
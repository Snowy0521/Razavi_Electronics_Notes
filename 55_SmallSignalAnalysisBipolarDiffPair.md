

# Razavi Electronics 2, Lec 10, Small-Signal Analysis of Bipolar Differential Pair 

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Summary of Diff. Pair Operation](#summary-of-diff-pair-operation)
2. [Small-Signal Analysis](#small-signal-analysis)



---
## Summary of Diff. Pair Operation
+ If  $|V_{in1} - V_{in2}|$ is large, all of the tail current is "steered" to one side $\to$ "current-steering" circuits.
+ If $V_{in1} - V_{in2}$ and $V_{CM, in}$ goes up and down $\to$ the current and voltages do not change.
+ If $|V_{in1} - V_{in2}| \ll 2 V_T \to \text{slope} = \frac{-R_CI_{EE}}{2V_T}$


### Quiz: Can this current amplify?
+ If $ \text{slope} = \frac{-R_CI_{EE}}{2V_T} > 1$ the answer will be yes. 
![](/images/DiffPairAmp.png)

---
## Small-Signal Analysis 
### Lemma
+ If $V_{in1}$ and $V_{in2}$ change by equal and opposite amounts and the change is small, then the tail node voltage does not change.
![](/images/lemma1.png)
![](/images/lemma2.png)
### Actual Small-Signal Model
+ Differential gain : $A_V = \frac{V_X - V_Y}{V_{in1} - V_{in2}} = - g_mR_C$
+ With $g_m = \frac{I_{EE}}{2V_T} \to A_V = - \frac{R_CI_{EE}}{2V_T}$
![](/images/SmallSignalModel.png)
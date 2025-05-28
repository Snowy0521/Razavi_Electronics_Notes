# Razavi Electronics 2, Lec 44, Bode's Rules, Stability Condition, Circuit Examples. 

This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents

1. [Bode's Rules](#bodes-rules)
2. [Stability Condition](#stability-condition)
3. [Circuit Examples](#circuit-examples)


 
--- 
## Information Points
+ If the open-loop system satisfies $KH$($jw_0$ ) = -1, then the closed-loop system is unstable.
+ Even if X = 0. the system still oscillates if $KH(jw_0 )$ = -1.
+ If $|KH(jw_0)|>1$ and $\angle KH(j\omega_0) = 180^\circ$, the system is also unstable. 
+ $K$ usually has no phase shift, so $\angle KH(j\omega_0) \approx \angle H(j\omega_0)$


---
## Bode's Rules
![](/images/BodeRules.png)
![](/images/BodesRulesExp.png)
---
## Stability Condition
![](/images/StabilityCondition.png)
+ For stability: Gain Crossover Frequency < Phase Crossover Frequency
---
## Circuit Examples
![](/images/StabilityExp.png)

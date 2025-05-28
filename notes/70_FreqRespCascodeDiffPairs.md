
# Razavi Electronics 2, Lec 25, Output Imp. of Followers, Freq. Resp. of Cascodes and Diff. Pairs, ft
This is my note for the electronics from razavi, I hope I can keep going it!!!

---

## Table of Contents
1. [Output Impedance of Followers](#output-impedance-of-followers)
2. [Freq. Response of Cascodes](#freq-response-of-cascodes)
3. [Freq. Response of Diff. Pairs]()
4. [The Transit Frequency, $f_T$]()




---
## Output Impedance of Followers
![](/images/OutputImpFollower.png)
### The bode's rules:
+ When we reach a zero $w_z$, the slope deflects up by 20 dB per decade
+ When we reach a pole $w_p$, the slope deflects down by 20 dB per decade

![](/images/OutputImpPlotFollower.png)
+ Case II is a more realistic case and in this case, we can treat the source follower as active inductor due to its impedance goes up with higher frequency.
---
## Freq. Response of Cascodes
![](/images/FreqCascode.png)
---
## Freq. Response of Diff. Pairs
![](/images/FreqDiffPair.png)
+ Can be treated as common source amplifier.
---
## The Transit Frequency, $f_T$
![](/images/f_TAnalysisUnityFreq.png)
![](/images/f_TUnityFreq.png)
### Example: How we maximize $f_T$?
$f_T = \frac{\sqrt{2\mu_n C_{ox} \frac{W}{L} I_D}}{2\pi C_{GS}}$
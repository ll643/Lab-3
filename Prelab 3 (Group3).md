Lynn Li (ll643) and Allison Tran (ant42)
Group 3
Prelab 3

#Question 1
$$ANC_{cayuga}=1.6meq/L$$
$$ANC_{wolf}=70\mu{eq}/L$$
```
from aguaclara.core.units import unit_registry as u
u.define('equivalent = mole = eq')
import aguaclara.research.environmental_processes_analysis as epa
from scipy import optimize
def ANC_zeroed(pHguess, ANC):
  return ((epa.ANC_open(pHguess) - ANC).to(u.mol/u.L)).magnitude
def pH_open(ANC):
  return optimize.brentq(ANC_zeroed, 0, 14,args=(ANC))
pH_Cayuga=pH_open(1.6*u.meq/u.L)
pH_Wolf=pH_open(70*u.mueq/u.L)

```
#Question 2
Givens:
pH=3.2
The pH of the influent is very low so: $$ANC=-[H^+]=-10^{-14}/[OH^-]$$
$$pOH=14-pH=14-3.2=10.8$$
$$[OH^{-1}]=10^{-pH}=10^{-10.8}$$
$$\Rightarrow-[H^+]=-10^{-14}/10^{-10.8}=-6.31*10^{-4}=ANC_{in}$$

#Question 3
[H+] is not a conservative species because it reacts with other species in the atmosphere.

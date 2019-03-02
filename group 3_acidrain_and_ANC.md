# Lab 3 (Acid Rain and Acid Neutralizing Capacity+)
##### Lynn Li (ll643): hours spent = 9
##### Allison Tran (ant42): hours spent = 9
#####  Group 3
##### Due 03/01/2019

# Introduction and Objectives
The overall goal of these two lab experiments was to model the acidification and remediation of a lake. In order to accomplish this, we created a simulation in which a "lake" received acid input meant to represent acid rain, and then collected and tested the pH of several samples from this simulation in order to find the acid neutralizing capacity (ANC). Acid rain is a real-world issue that affects water supplies for both humans and the environment; this issue is becoming more pertinent as humans are increasing their fossil fuel consumption since "acid precipitation results from the combustion of fossil fuels which produce oxides of sulfur and nitrogen that react in the earth’s atmosphere to form sulfuric and nitric acid emissions" (Lab Manual). We hoped that by simulating this phenomenon on a smaller scale we would be able to study the physical and chemical effects of acidification and come up with a remedying solution that could be applied to the bigger problem. In order for this lab to succeed, we had to acidify our lake model in increments over specified time intervals, measure the pH of our lake samples, and use Gran plot analysis to create titration curves through which we would be able to determine the ANC values. Additionally, this lab provided us with an opportunity to practice specific lab techniques such as pipetting precisely, setting up various tubing systems, and calibrating and using a pH probe.

### Acid Rain Equations

$\left[{OH}^{{-}} \right] = \frac{K_w}{\left[H^+\right]}$

$pOH=14-pH$

$[OH^{-1}]=10^{-pH}=10^{-7}$

$\Rightarrow-[H^+]=-10^{-14}/10^{-7}=-110^{-7}mol/L$

${ANC\; }={\; }\left[{HCO}_{{3}}^{{-}} \right]+{\; 2}\left[{CO}_{{3}}^{{-2}} \right]+\left[{OH}^{{-}} \right]{\; -}\left[{H}^{+} \right]$

$ANC=\frac{P_{CO_2} K_H }{\alpha_0 } (\alpha_1 +2\alpha_2 ) + \frac{K_w }{\left[H^+ \right]} - \left[H^+ \right]$

$ANC_{out} \; =\; ANC_{in} \; \cdot \; \left(1\; -\; {\mathop{e}\nolimits^{-t/\theta \; \; }} \right)+\; ANC_{0} \; \cdot \; {\mathop{e}\nolimits^{-t/\theta \; }}$

$\theta = V/Q$

### ANC+ equations

${F_1} = \frac{{{V_S} + {V_T}}}{{{V_S}}}{\text{[}}{{\text{H}}^ + }{\text{]}}$

$ANC=\frac{V_e N_t }{V_s }$

$CO_3^{2-}+H^+ \Rightarrow HCO_3^-$

$HCO_3^-+H^+ \Rightarrow H_2CO_3 $

# Procedures
The first part of this lab involved monitoring the pH of a "lake" or a reservoir of water as acid rain was being deposited into the reservoir in specified increments. An acidic feed solution was used to mimic acid rain and was connected to a peristaltic pump, which pumped the feed solution into a lake basin with an initial ANC. The lake was consistently drained with a tube to maintain a constant lake volume of 4 liters. A pH probe in the lake basin, calibrated prior to beginning the experiment, collected pH measurements in one second intervals through ProCoDA. Notes were added to this data to mark the 0, 5, 10, and 20 minute intervals, and samples of the water were collected at each interval as well. These samples were to be used for the second part of the lab. Prior to pumping, 1mL of bromocresol green indicator solution and 623mg of NaHCO3 (ANC) were added to the lake. At the end of the 20 minutes of acid deposition, we measured the flow rate coming out of the beaker and the final volume of the lake. We then emptied the lake and repeated the same experiment, except this time we doubled the initial amount of NaHCO3 added (1.246g).

In the second part of the lab, we used ProCoDa to determine the ANC of the samples we collected in the first part of the lab. Before starting, we tested the accuracy of the Gran plot analysis in ProCoDA to ensure that it would accurately measure the acid neutralizing capacity (ANC) of a sample. To do this, we titrated a 50 mL sample of reverse osmosis water (ANC = 0 meq/L) with 0.250000mL of 0.05N HCl and collected pH measurements. We then used the data collected to plot a titration curve. The error producced was less than 0.1 meq/L (equal to an error of 0.1 mL titrant) which verified that using the Gran technique on ProCoDa would accurately measure the ANC of a sample. We used this same technique to determine the ANC of the five acid rain samples collected in the previous part of the lab. Samples with an initial pH of less than 4.5 did not need to be tested. Instead, on these samples we used Equation 45 (given in the lab manual) to solve for the ANC. For solutions with a pH greater than 4.5, we titrated 50 mL of each sample with 0.250000mL increments of 0.05N HCl using pipetting techniques, and collected sufficient pH measurements in order to use Gran plot analysis to determine the ANC of the samples. pH measurements were logged after the lake stabilized from the individual increments of HCl.

# Results and Discussion
### Graphs
![Figure 1](https://github.com/ll643/Lab-3/blob/master/group3_lab3_figure1.png)

Figure 1: Plot of pH vs Hydraulic Residence Time as acid rain is being added to a lake

![Figure 2](https://github.com/ll643/Lab-3/blob/master/group3_lab3_figure2.png)

Figure 2: Plot of ANC (conservative, closed, and open) vs Hydraulic Residence Time as acid rain is being added to a lake

![Figure 3](https://github.com/ll643/Lab-3/blob/master/group3_lab3_figure3.png)

Figure 3: Plot of pH vs Hydraulic Residence Time as acid rain is being added to a lake with twice the initial ANC amount

![Figure 4](https://github.com/ll643/Lab-3/blob/master/group3_lab3_figure3.png)

Figure 4: Plot of ANC (conservative, closed, and open) vs Hydraulic Residence Time as acid rain is being added to a lake with twice the initial ANC amount

![Figure 5](https://github.com/ll643/Lab-3/blob/master/group3_lab3_figure5.png)

Figure 5: Plot of pH vs Titrant Volume as increments of HCl are being added to a lake

![Figure 6](https://github.com/ll643/Lab-3/blob/master/group3_lab3_figure6.png)

Figure 6: Gran Plot of Gran Function vs Titrant Volume as HCL is being added to the sample of lake water from t=0

![Figure 7](https://github.com/ll643/Lab-3/blob/master/group3_lab3_figure7.png)

Figure 7: Plot of ANC vs Hydraulic Residence Time of all the ANCs calculated from the five titrations along with the ANC curves from Figure 2

### Acid rain
Through our initial acid rain experiment, we were able to generate Figure 1 and 2 which shows that pH decreases exponentially with hydraulic residence time as acid rain is being added to it. Similarly ANC also decreases exponentially with hydraulic residence time except open ANC which decreases past a hydraulic residence time of 1.25 but before then is at a constant pH. We were also able to show that by doubling the initial ANC of the lake (from 0.623g of NaCO3 to 1.246g of NaCO3), the lake is better at buffering the acid rain. Based off of the figures produced (Figure 3 and Figure 4), we can see that the final pH of the lake after 20 mins with the extra ANC (pH around 6) is much higher than the final pH of the lake after 20 mins with the normal dosage of ANC (pH around 4). Nonetheless, pH and ANC still decreases with hydraulic residence time no matter the starting ANC amount.
### ANC+
After performing the second part of the ANC lab, we were able to generate titration curves and gran plots with the data that was generated through ProCoDa. These are available for the lake samples from t=0, 5, 10, 15, and 20. On Figure 5, the blue line marks the cutoff where the dominant reaction is generating bicarbonate. The red line marks the cutoff where the dominant reaction is generating carbonic acid. To the right of the red line is the region where no significant reactions are occurring. From Figure 6, we can see that the Ve (equivalent volume) is 1.7149822076069936 which was calculated from the linear regression model. This is almost the exact number that was generated from ProCoDa which is 1.714982. Looking at Figure 7, we can see that the measured ANC values agree with the conservative ANC model. The curve generated by the experimental ANC values mimics the Conservative ANC curve.

##### Question 1: What do you think would happen if enough NaHCO3 were added to the lake to maintain an ANC greater than 50μeq/L for 3 residence times with the stirrer turned off? How much NaHCO3 would need to be added?

If enough NaHCO3 was added to the lake to maintain an ANC greater than 50μeq/L for 3 residence times with the stirrer turned off, the lake would be able to withstand the acid rain for a longer time before it reached its buffering threshold and surrendered to acidification. However, because the lake is not being stirred, the NaHCO3 would sink to the bottom of the lake and the top of the lake would still become acidified. Visually, this change would cause the lake to stay blue longer before it started to become a clear yellow/green color.

##### Question 2: What are some of the complicating factors you might find in attempting to remediate a lake using CaCO3? Below is a list of issues to consider: extent of mixing, solubility of CaCO3 (find the solubility and compare with NaHCO3), and density of CaCO3 slurry (find the density of CaCO3)
One of the complicating factors that we might find in attempting to remediate a lake using CaCO3 is the extremely low solubility of CaCO3 in pure water (15mg/L) which would make it difficult to dissolve therefore making it not as effective of a remediating agent. In addition its solubility is variant with the temperature of the water (it is inversely proportional to temperature). In contrast, NaHCO3 is extremely water-soluble no matter the temperature of the water. However, it is important to note that due to this discrepancy, CaCO3 could potentially be more soluble than NaHCO3 if we are using cold water. Another complicating factor we must take into consideration is that fact that CaCO3 as a slurry is denser than NaHCO3 (2.74 g/cm3 vs 2.2g/cm3) and therefore would be more difficult to mix thoroughly throughout the lake. These factors should be kept in mind when deciding on a remediation process with CaCO3, as calcium carbonate is more selectively soluble and denser than NaHCO3.

# Appendix
|     Attribute | Value    |   
|--------------:|----------|
|pH of "Rain"   |     3    |
|Volume of Lake |4 liters  |
|Flow           |161ml/30s |
|Pump Rate      |267 mL/min|
|Initial NaHCO3 |623 mg    |
|Bromocresol Green|  1  mL |
### Acid Rain
##### First Experiment:
```python
#pH vs Hydraulic Residence Time
from aguaclara.core.units import unit_registry as u
import aguaclara.research.environmental_processes_analysis as epa
from scipy import optimize
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
data_file_path="https://raw.githubusercontent.com/ll643/Lab-2/master/group3_acidrain_data.tsv"
df = pd.read_csv(data_file_path,delimiter='\t')
array = np.array(df)
V = 4*(u.quarts)
V = V.to(u.L)
Q = (161*(u.mL))/(30*(u.s))
Q = Q.to(u.L/u.s)
theta = (V/Q)
time = (array[:,0]*(u.day)-0.60090697*(u.day))#0.60090697 is time 0
time = time.to(u.s)
hydraulic_residence_time = (time/theta).to(u.dimensionless)
pH = array[:,1]
plt.figure()
plt.plot(hydraulic_residence_time, pH,'-')
plt.xlabel('Hydraulic Residence Time (dimensionless)')
plt.ylabel('pH of Lake')
plt.title('pH of Lake vs. Hydraulic Residence Time')
plt.show() #this is the plot for pH vs time

#ANC graphs
Mass_NaHCO3 = 0.623*(u.g)
molar_mass_NaHCO3 = 84.007*(u.g/u.mol)
mol_NaHCO3 = Mass_NaHCO3/molar_mass_NaHCO3
Conc_NaHCO3 = mol_NaHCO3/V
ANC_0 = Conc_NaHCO3
ANC_in = -0.001*(u.eq/u.L)
ANC_con = (ANC_in*(1-np.exp(-hydraulic_residence_time)))+(ANC_0*np.exp(-hydraulic_residence_time))
ANC = ANC_0*np.exp(-hydraulic_residence_time)
Closed_ANC = epa.ANC_closed(pH,ANC)
Open_ANC = epa.ANC_open(pH)
plt.plot(hydraulic_residence_time, ANC_con, label='Conservative ANC') #conservative ANC
plt.plot(hydraulic_residence_time, Closed_ANC, label = 'Closed ANC') #closed ANC
plt.plot(hydraulic_residence_time, Open_ANC, label = 'Open ANC') #open ANC
plt.xlabel('Hydraulic Residence Time (dimensionless)')
plt.ylabel('ANC (eq/L)')
plt.title('ANC vs. Hydraulic Residence Time')
plt.legend()
plt.show()#this is the plot of all three ANC types vs time
```
##### Second experiment:
```python
#pH vs Hydraulic Residence Time
data_file_path="https://raw.githubusercontent.com/ll643/Lab-2/master/group3_acidrain_data2.tsv"
df = pd.read_csv(data_file_path,delimiter='\t')
array = np.array(df)
V = 4*(u.quarts)
V = V.to(u.L)
Q = (161*(u.mL))/(30*(u.s))
Q = Q.to(u.L/u.s)
theta = (V/Q)
time = (array[:,0]*(u.day)-0.60090697*(u.day))#0.60090697 is time 0
time = time.to(u.s)
hydraulic_residence_time = (time/theta).to(u.dimensionless)
pH = array[:,1]
plt.figure()
plt.plot(hydraulic_residence_time, pH,'-')
plt.xlabel('Hydraulic Residence Time (dimensionless)')
plt.ylabel('pH of Lake')
plt.title('pH of Lake vs. Hydraulic Residence Time')
plt.show() #this is the plot for pH vs time

#ANC Graphs
Mass_NaHCO3 = 1.246*(u.g)
molar_mass_NaHCO3 = 84.007*(u.g/u.mol)
mol_NaHCO3 = Mass_NaHCO3/molar_mass_NaHCO3
Conc_NaHCO3 = mol_NaHCO3/V
ANC_0 = Conc_NaHCO3
ANC_in = -0.001*(u.eq/u.L)
ANC_con = (ANC_in*(1-np.exp(-hydraulic_residence_time)))+(ANC_0*np.exp(-hydraulic_residence_time))
ANC = ANC_0*np.exp(-hydraulic_residence_time)
Closed_ANC = epa.ANC_closed(pH,ANC)
Open_ANC = epa.ANC_open(pH)
plt.plot(hydraulic_residence_time, ANC_con, label='Conservative ANC') #conservative ANC
plt.plot(hydraulic_residence_time, Closed_ANC, label = 'Closed ANC') #closed ANC
plt.plot(hydraulic_residence_time, Open_ANC, label = 'Open ANC') #open ANC
plt.xlabel('Hydraulic Residence Time (dimensionless)')
plt.ylabel('ANC (eq/L)')
plt.title('ANC vs. Hydraulic Residence Time')
plt.legend()
plt.show()#this is the plot of all three ANC types vs time
```
### ANC+
```python
#pH vs Titrant Volume Graph
from aguaclara.core.units import unit_registry as u
u.define('equivalent = mole = eq')
import aguaclara.research.environmental_processes_analysis as epa
from scipy import optimize
from scipy import stats
from aguaclara.core import utility as ut
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
Gran_data = 'https://raw.githubusercontent.com/ll643/Lab-3/master/group3_ANC_time0.xls'
V_titrant, pH, V_Sample, Normality_Titrant, V_equivalent, ANC = epa.Gran(Gran_data)
fig, ax = plt.subplots()
ax.plot(V_titrant,pH,'r')
plt.xlabel('Volume of Titrant (mL)')
plt.ylabel('pH')
ax.annotate('$ H^+ + HCO_3^-\Rightarrow H_2CO_3$', xy=(1.11, 5.64551), xytext=(1.5, 7), arrowprops=dict(facecolor='red', shrink=0.05),)
ax.annotate('$ H^+ + CO_3^{2-} \Rightarrow HCO_3^-$', xy=(0.1, 7), xytext=(0, 5.7), arrowprops=dict(facecolor='blue', shrink=0.05),)
plt.axvline(x=0.251764,color='b')
plt.axvline(x=2,color='red')
#ax.annotate('equivalent volume', xy=(1.433219, 2.8), xytext=(1.4, 4), arrowprops=dict(facecolor='red', shrink=0.10),)
plt.title('pH vs Titrant Volume')
plt.show() #Titrant Graph

#Gran Plot of t=0
def F1(V_sample,V_titrant,pH):
  return (V_sample + V_titrant)/V_sample * epa.invpH(pH)
F1_data = F1(V_Sample,V_titrant,pH)
N_good_points = 3
slope, intercept, r_value, p_value, std_err = stats.linregress(V_titrant[-N_good_points:],F1_data[-N_good_points:])
intercept = intercept*u.mole/u.L
slope = slope*(u.mole/u.L)/u.mL
V_eq = -intercept/slope
ANC_sample = V_eq*Normality_Titrant/V_Sample
print('The r value for this curve fit is', ut.round_sf(r_value,5))
print('The equivalent volume was', ut.round_sf(V_eq,2))
print('The acid neutralizing capacity was',ut.round_sf(ANC_sample.to(u.meq/u.L),2))
x=[V_eq.magnitude,V_titrant[-1].magnitude ]
y=[0,(V_titrant[-1]*slope+intercept).magnitude]
plt.plot(V_titrant, F1_data,'o')
plt.plot(x, y,'r')
plt.xlabel('Titrant Volume (mL)')
plt.ylabel('Gran Function (mole/L)')
plt.legend(['data'])
plt.title('Gran Plot at t=0')
plt.show()

#Experimental ANC vs Previous ANC Graph
data_file_path="https://raw.githubusercontent.com/ll643/Lab-2/master/group3_acidrain_data.tsv"
df = pd.read_csv(data_file_path,delimiter='\t')
array = np.array(df)
V = 4*(u.quarts)
V = V.to(u.L)
Q = (161*(u.mL))/(30*(u.s))
Q = Q.to(u.L/u.s)
theta = (V/Q)
time = (array[:,0]*(u.day)-0.60090697*(u.day))#0.60090697 is time 0
time = time.to(u.s)
hydraulic_residence_time = (time/theta).to(u.dimensionless)
pH = array[:,1]
Mass_NaHCO3 = 0.623*(u.g)
molar_mass_NaHCO3 = 84.007*(u.g/u.mol)
mol_NaHCO3 = Mass_NaHCO3/molar_mass_NaHCO3
Conc_NaHCO3 = mol_NaHCO3/V
ANC_0 = Conc_NaHCO3
ANC_in = -0.001*(u.eq/u.L)
ANC_con = (ANC_in*(1-np.exp(-hydraulic_residence_time)))+(ANC_0*np.exp(-hydraulic_residence_time))
Closed_ANC = epa.ANC_closed(pH,ANC_0)
Open_ANC = epa.ANC_open(pH)
Time =  np.array([0,5,10,15,20])*(u.min)
Time = Time.to(u.s)
V = 4*(u.quarts)
V = V.to(u.L)
Q = (161*(u.mL))/(30*(u.s))
Q = Q.to(u.L/u.s)
theta = (V/Q)
Hydraulic_Residence_Time = (Time/theta).to(u.dimensionless)
ANC = np.array([0.001715,0.000873,0.000272,-0.000049,-0.000435 ])*(u.eq/u.L)
plt.plot(Hydraulic_Residence_Time, ANC, label = 'Experimental ANC') #ANC determined experimentally
plt.plot(hydraulic_residence_time, ANC_con, label='Conservative ANC') #conservative ANC
plt.plot(hydraulic_residence_time, Closed_ANC, label = 'Closed ANC') #closed ANC
plt.plot(hydraulic_residence_time, Open_ANC, label = 'Open ANC') #open ANC
plt.xlabel('Hydraulic Residence Time (dimensionless)')
plt.ylabel('ANC (eq/L)')
plt.title('ANC vs. Hydraulic Residence Time')
plt.legend()
plt.show()
```

# Conclusions
From these two labs we were able to see the effects of acidification on a lake with initial ANC both visually and quantitatively. At the beginning of the experiment, the lake was a clear blue color, but as the amount of acid rain in the lake became to accumulate the lake lost its pretty color and went clear before it became a greenish yellow color. Quantitatively we see from Figure 1 that pH levels dropped exponentially from the beginning of the experiment, but as the lake reached its ANC threshold the decline became more steep. When the initial ANC was doubled, we observed that the lake was able to withstand the acid rain much better. The curvature of Figure 4 is less steep than that of Figure 1. Due to minor leaking, the curves produced are not very smooth; there are some anomaly data points. However, the general shape of the curve can be easily identified. Through the titration process we were able to accurately generate data through ProCoDa which then allowed up to create titration curves and gran plots. ProCoDa also provided us with ANC information about our lake samples that we were able to plot and match to our Conservative ANC curve from the first acid rain lab. Regardless of the bumps in the road, we successfully achieved our experimental objectives and collected sufficient data that allowed for through analysis.

# Suggestions/Comments
Overall, this was a super educational and enjoyable lab! We liked how along the way visually we were able to see if we were doing the lab correctly. As a whole, the lab was quite easy to complete; however, setting up the lab and using ProCoDa accurately was confusing. Specifically with ProCoDa, we had to redo the first two titrations multiple times because we did not know which buttons to correct and ProCoDa would plot extra points which skewed the Gran Plots and produced inaccurate ANC values. We think it would have been helpful if on the first day of lab we were given a tutorial of how to use the various lab equipment and given a basic tutorial of how to use ProCoDa. There are other minor set up details that could have been clearer. For example, we did not know that there was a clamp for the pH probe so we just tapped it to the side of our lake. We think that all of the set up confusion can be easily fixed with an extra diagram or two of the whole set up along with more detailed instructions.

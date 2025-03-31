---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
title: A Story About Crime in San Francisco
--- 

### Introduction

This short data story explores **patterns in vehicle thefts** across San Francisco between *2003 and 2024*.  
The dataset comes from the *San Francisco Police Department*, and includes details such as:

- Time and date of each incident  
- Geographic coordinates  
- Police district  
- Crime category

Our focus is on understanding:

-  *When* cars are most likely to be stolen  
-  *Where* thefts are most common  
-  How trends have shifted over time

###  Monthly Trends Over Time


As shown below, vehicle thefts were **very high in the early 2000s**, with some months reaching nearly *1,800 incidents*.  
Around *2006*, thefts began a steady decline — possibly due to:

- Better car anti-theft systems  
- Improved urban surveillance  
- City policy changes  

From *2020 onward*, there's a slight rise again, perhaps related to COVID-19 disruptions or economic shifts.


![Time series chart](/assets/output.png)

*Figure 1: Vehicle Theft in San Francisco shown in Monthly trends*

### Where Cars Get Stolen


The map below shows **theft density by police district**. The worst-hit districts are:

- **Bayview**  
- **Southern**  
- **Mission**

In contrast, districts like **Richmond**, **Park**, and **Ingleside** appear significantly safer.  
This could be due to differences in parking layouts, density, or other social/economic factors.

<iframe src="assets/vehicle_thefts_map.html" width="100%" height="600px"></iframe>
*Figure 2: Map of San Francisco showing theft density by police districts*

###  When Cars Get Stolen



The plot below shows thefts by hour of the day. We see a very clear pattern:

- Thefts are **lowest between 3–6 a.m.**
- They **rise steadily throughout the day**
- And they **peak between 5–9 p.m.**

This might correspond to people parking after work, running errands, or attending events — leaving vehicles unattended during higher-risk hours.


<iframe src="assets/boke_plot.html" width="100%" height="600px" frameborder="0"></iframe>

*Figure 3: Bokeh plot of thefts in San Francisco for every hour of the day*

###  Conclusion

Vehicle thefts in San Francisco have **changed dramatically over the past 20 years**.  
This short data story shows:

-  A *major decline* in thefts from 2003 to 2014  
-  *Geographic hotspots* that remain consistently high-risk  
-  *Time-of-day patterns* that suggest when cars are most vulnerable

Understanding these patterns is helpful for:

- Citizens looking to reduce risk  
- Policymakers targeting patrols  
- Anyone interested in how data reveals city dynamics


<div>
  <!-- This is where we will embed the Bokeh plot later -->
</div>

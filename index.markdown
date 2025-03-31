---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
title: A Story About Car Theft Crimes in San Francisco
--- 

## Introduction

This short data story explores patterns in vehicle thefts across San Francisco between *2003 and 2024*.  
The dataset comes from the *San Francisco Police Department*, and includes details such as:

- Time and date of each incident  
- Geographic coordinates  
- Police district  
- Crime category

Our focus is on understanding when vehicles are most likely to be stolen, where vehicle thefts are most common and how trends have shifted over time.

##  Monthly Trends Over Time

The first thing we wanted to explore was how vehicle thefts evolved over time. By looking at the monthly trends from 2003 to 2024, we were able to get a clear overview of when car thefts were most frequent, and how patterns shifted over the years
As shown below, vehicle thefts were high in the early 2000s, peaking in 2005 with nearly 1,800 incidents.
Starting around 2006, thefts began a steady decline. Our group discussed several possible reasons for this trend, including improvements in car anti-theft systems, enhanced urban surveillance, or internal policy changes within the city.

While vehicle thefts steadily declined after the mid-2000s, our data shows a slight uptick beginning in 2020. This recent rise aligns with national trends highlighted by the [Council on Criminal Justice](https://counciloncj.org/trends-in-carjacking-what-you-need-to-know/), which observed increases in carjackings across major U.S. cities, including San Francisco, during the pandemic years. Experts suggest that this may be linked to COVID-19 disruptions, economic stressors, and a breakdown in routine policing and community structures.

![Time series chart](/assets/output.png)

*Figure 1: Vehicle Theft in San Francisco shown in Monthly trends*

## Where Cars Get Stolen

Using police district boundaries and crime data from 2003 to 2024, we created a choropleth map showing the number of vehicle thefts per district. Each district is shaded based on the total number of incidents.
The map below shows theft density by police district. The worst-hit districts are:

- Ingleside  
- Bayview
- Mission

In contrast, districts like Park, Richmond and Central appear significantly safer.  
This could be due to differences in parking layouts, density, or other social/economic factors. 


<iframe src="assets/vehicle_thefts_map.html" width="100%" height="600px"></iframe>
*Figure 2: Map of San Francisco showing theft density by police districts*

##  When Cars Get Stolen



The plot below shows thefts by hour of the day. We see a very clear pattern:

- Thefts are lowest between 3–6 a.m.
- They rise steadily throughout the day
- And they peak between 5–9 p.m.

This might correspond to people parking after work, running errands, or attending events — leaving vehicles unattended during higher-risk hours.


<iframe src="assets/boke_plot.html" width="100%" height="600px" frameborder="0"></iframe>

*Figure 3: Bokeh plot of thefts in San Francisco for every hour of the day*

##  Conclusion

Vehicle thefts in San Francisco have **changed dramatically over the past 20 years**.  
This short data story shows:

-  A *major decline* in thefts from 2003 to 2014  
-  *Geographic hotspots* that remain consistently high-risk  
-  *Time-of-day patterns* that suggest when cars are most vulnerable

Understanding these patterns is helpful for:

- Citizens looking to reduce risk  
- Policymakers targeting patrols  
- Anyone interested in how data reveals city dynamics

## Contributors

<ul>
  {% for person in site.authors %}
    <li>
      {{ person.name }} —
      <a href="mailto:{{ person.email }}">{{ person.email }}</a>
      {% if person.github %}
        | <a href="https://github.com/{{ person.github }}">GitHub</a>
      {% endif %}
    </li>
  {% endfor %}
</ul>
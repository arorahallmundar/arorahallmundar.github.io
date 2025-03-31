---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
title: A Story About Vehicle Theft Crimes in San Francisco
--- 

## Introduction

This data story explores patterns in vehicle thefts across San Francisco between 2003 and 2024, using open data from the [San Francisco Police Department](https://datasf.org/opendata/). The dataset includes information on the time, location, and police district of each reported incident.

Our goal is to understand when and where vehicle thefts are most common, and how those patterns have changed over time. The project connects to broader discussions around predictive policing, a practice that uses crime data to anticipate future incidents. For more background, see [this article](https://www.science.org/content/article/can-predictive-policing-prevent-crime-it-happens) on predictive policing used in our class. By using visualizations, we aim to uncover meaningful trends in the data, offering insights into how thefts fluctuate month to month, which areas are most affected, and what time of day cars are most at risk.


##  Monthly Trends Over Time

We start by exploring how vehicle thefts change over time. By looking at monthly trends from 2003 to 2024, we get a clear overview of when vehicle thefts are most frequent and how patterns shift over the years. As shown below, thefts are particularly high in the early 2000s, peaking in 2005 with nearly 1,800 incidents. Starting around 2006, they begin a steady decline.

This decline aligns with national trends. A [New York Times article](https://www.nytimes.com/2014/08/12/upshot/heres-why-stealing-cars-went-out-of-fashion.html) links the drop in thefts to improvements in car security, such as electronic immobilizers and smart keys, which make newer vehicles much harder to steal. While the article focuses on New York, these technologies were adopted nationwide and likely contributed to similar reductions in San Francisco. Additional factors may include enhanced urban surveillance and local policy changes.

While thefts continue decreasing into the 2010s, our data shows a slight uptick beginning in 2020. This rise mirrors national patterns highlighted by the [Council on Criminal Justice](https://counciloncj.org/trends-in-carjacking-what-you-need-to-know/), which reports an increase in carjackings during the pandemic years — including in San Francisco. Experts suggest this may be linked to COVID-19 disruptions, economic stress, and shifts in routine policing or community dynamics.

![Time series chart](/assets/output.png)

*Figure 1: Vehicle Theft in San Francisco shown in Monthly trends*

## Where Cars Get Stolen
Now that we've looked at overall trends over time, let's take a closer look at where vehicle thefts are happening. By mapping the number of thefts across police districts in San Francisco, we can identify which areas have been most affected. Each district is shaded based on the total number of incidents.

The map below shows theft density by police district. The worst-hit districts are:

- Ingleside  
- Bayview
- Mission

In contrast, districts like Tenderloin, Park, Richmond and Central appear significantly safer.  
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

Vehicle thefts in San Francisco have changed dramatically over the past 20 years.  
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
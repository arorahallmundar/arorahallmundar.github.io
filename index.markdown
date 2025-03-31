---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
title: A Story About Vehicle Theft Crimes in San Francisco
--- 
Authors: 
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
Now that we've looked at overall trends over time, we take a closer look at where vehicle thefts are happening. By mapping the number of thefts across police districts in San Francisco, we can identify which areas are most affected. Each district is shaded based on the total number of incidents from 2003 to 2024.

The map below shows that Ingleside, Bayview, and Mission are the worst-hit districts, with the highest number of reported thefts. In contrast, areas like Tenderloin, Park, Richmond, and Central appear significantly safer. These differences could reflect a range of local factors. According to the FBI’s Variables Affecting Crime report, it’s difficult to make meaningful comparison about crime rates between places without considering broader social and institutional factors.


<iframe src="assets/vehicle_thefts_map.html" width="100%" height="600px"></iframe>
*Figure 2: Map of San Francisco showing theft density by police districts*

##  When Cars Get Stolen

After identifying where vehicle thefts are most common, we shift our focus to when they are most likely to occur throughout the day. The Bokeh plot below shows that vehicle thefts are relatively low in the early morning hours but rise throughout the day, peaking in the evening. While many sources mention that thefts often occur at night, our findings suggest that incidents are most frequent just before that, during the evening period. Some factors that come first to mind are people parking their cars after work, running errands, or attending events, leaving vehicles unattended during evenings. More research would be needed to fully explain this pattern, but it highlights how local trends may differ from general assumptions.


<iframe src="assets/boke_plotnew.html" width="100%" height="600px" frameborder="0"></iframe>

*Figure 3: Bokeh plot of thefts in San Francisco for every hour of the day*

##  Conclusion

Over the past 20 years, vehicle thefts in San Francisco have followed clear and meaningful patterns. Our analysis shows a major decline in thefts beginning around 2006, likely influenced by improvements in car security, surveillance, and policy changes. However, this long-term drop is interrupted by a noticeable rise after 2020, reflecting broader national trends linked to the pandemic and its disruptions.

We also find that thefts are not evenly distributed across the city and certain districts remain persistent hotspots. In addition, thefts tend to occur more often during the evening hours, when vehicles are more likely to be left unattended and it's darker outside. These insights offer a brief overview of how vehicle theft crime in San Francisco has evolved, and how data can help us understand the conditions that shape it.

## Contributors
Since one group member was responsible for pushing updates to the website, we decided to work closely together on all aspects of the project. We didn’t divide tasks, but instead collaborated throughout the assignment.

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
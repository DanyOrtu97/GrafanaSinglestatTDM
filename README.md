# Singlestat Panel - TDM modified version
Authors
Daniele Ortu, Gabriele Merlin
University of Cagliari 

###################
Native  SingleStat Panel
###################

Read more about it here:
[http://docs.grafana.org/reference/singlestat/](http://docs.grafana.org/reference/singlestat/)
Copyright 2018 © Kenji Noguchi / Verizon Digital Media Services
Copyright 2018 © Grafana Labs

###################
Modified version of SingleStat Panel
###################

SingleStatTDM is a modified version Grafana’s native singlestat panel. It is a part of TDM project, (link: http://www.tdm-project.it/) , initiative born thanks to the collaboration between CRS4 and the University of Cagliari.
In this case, the goal was to show your current consumption with your average consumption, your maximum and minimum and also show your average consumption put in relation to the consumption of a given area.

Limits of native panel
The original singlestat did not allow to obtain all dynamic value, the only dynamic value was the average (inserted through query), while the maximum, the minimum and the threshold values were inserted through the interface (statically).

What’s new
This version of SingleStat Panel allows to insert 4 queries to manage data on Panel. This query allows to obtain all dynamic values:
first query: retrieve the main value of panel
second query: retrieve maximum value
third and four query: retrieve average values or other significant comparison values

A legend has also been added for better understanding and the legend labels can be modified through the interface.


###################
Setup on Grafana(Windows)
###################

To use this plugin inside Grafana it is necessary to download it, unzip it and insert it into Grafana installation folder: grafana-5.4.2 -> data -> plugins 
To configure it on Grafana you need the support to a database as Influxdb or similar. After database configuration, the query must be entered as in the old plugin, but in this modified plugin 4 queries are needed.


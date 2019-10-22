# Singlestat Panel - TDM modified version

This plugin is part of the TDM project (http://www.tdm-project.it) and it has been presented during the STAG 2019 scientific conference (http://stag2019.crs4.it) with the poster "Design and Implementation of a Visualization Tool for the in-depth Analysis of the Domestic Electricity Consumption".

## Native  SingleStat Panel

Read more about it here:
[http://docs.grafana.org/reference/singlestat/](http://docs.grafana.org/reference/singlestat/)
Copyright 2018 © Kenji Noguchi / Verizon Digital Media Services
Copyright 2018 © Grafana Labs

### Limits of native panel

The original singlestat did not allow to obtain all dynamic value, the only dynamic value was the average (inserted through query), while the maximum, the minimum and the threshold values were inserted through the interface (statically).

## Modified version of SingleStat Panel

SingleStatTDM is a modified version Grafana’s native singlestat panel. The goal was to show your current consumption with your average consumption, your maximum and minimum and also show your average consumption put in relation to the consumption of a given area.

## What’s new?

This version of SingleStat Panel allows to insert 4 queries to manage data on Panel. This query allows to obtain all dynamic values:
first query: retrieve the main value of panel
second query: retrieve maximum value
third and four query: retrieve average values or other significant comparison values

A legend has also been added for better understanding and the legend labels can be modified through the interface.


## Setup on Grafana (Windows)

To use this plugin inside Grafana it is necessary to download it, unzip it and insert it into Grafana installation folder: grafana-5.4.2 -> data -> plugins 
To configure it on Grafana you need the support to a database as Influxdb or similar. After database configuration, the query must be entered as in the old plugin, but in this modified plugin 4 queries are needed.

## Authors
Daniele Ortu, Gabriele Merlin, Gianmarco Cherchi and Riccardo Scateni 

University of Cagliari, Italy

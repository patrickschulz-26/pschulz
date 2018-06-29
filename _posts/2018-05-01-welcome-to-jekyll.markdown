---
title:  "Avalanche Prediction Model"
date:   2018-05-01 15:04:23
categories: [Python]
tags: [Python]
---
This is a Python based application that takes in historical weather data from winter 2017/2018 and elevation data taken by NASA's Shuttle Radar Topgraphy Misson (SRTM) and creates an risk analysis of any region in the greater Salt Lake City area on any date in the winter season. It contains a command line GUI for the user to imput the name of the area along with four latitude and longitude bounds and outputs a interactive 2D and 3D map for the user to see where the safest area is to ski. An example for Park City, Utah for April 1, 2018 in 3D is seen below:

![helpfulImg](https://github.com/patrickschulz-26/website/blob/master/assets/ava2D.png?raw=true)

the example for 2D is seen below:

![helpfulImg](https://github.com/patrickschulz-26/website/blob/master/assets/ava3D.png)

The engine of this program is broken up into three seperate parts. Part one works on taking elevation data given from the SRTM and finding the specific angle of every 40 meter section of the region. Part two creates a snowpack model, an eveluation of each layer of snow, by using the Scipy ordinary diffrental equations module in addition with all the the weather data for all days starting from the begining of the season. The third part of this engine cross referances the snowpack model with the specific angle at each point. This part then adds an extra stress variable for a skiier going down the face of the region. From this data the specific risk of an avalanche from a skier can be found.

Updates for this program will be coming. These updates will include global historical data so the program can be run anywhere with out limitations. In addition a gradent risk anylysis will be implimented for better user experience.

Check out the on my [github][git] for more info about this project and other.

[git]:      https://github.com/patrickschulz-26


---
layout: archive
title: "Coding"
permalink: /coding/
author_profile: true
---
In the age of Large Language Models or Artificial "Intelligences" like ChatGPT4 I have slowly started to develop an interest in writing code - primarily R and Python - particularly because after playing around with GPT4 I figured that I could probably save some time on my project if I had a bunch of 1s and 0s doing some of the work for me. As Bill Gates probably said: "Work smarter - not harder". 

However, being born in 1990, coding in any way, shape or form was never part of my primary (or secondary) school curriculum. And coming from a hard humanities background it wasn't part of my university education either. So, even If I've tried to learn a bit of coding for years I never managed to get started. But with the aid of GPT4, I was suddenly able to write code that actually *did* something. And here is a few (poor) examples at that - nonetheless it's code that I've actively used for my own research. 

**[mni_analyser.py](https://github.com/jhj-proteomics/mni_analyser)**

For my PhD, I had to sample several zooarchaeological remains for ZooMS analysis. However, my main concern was to avoid sampling the same individual twice. To avoid that I wanted to develop a simple script that could take the information in a zooarchaeological dataset and automatically identify which sample IDs were likely to represent bone elements from a single individual. However, to do so, I had to develop a second script that generated a theoretical zooarchaeological dataset to use in the script. 

**[assemblage_generator.py](https://github.com/jhj-proteomics/assemblage_generator)**

To test mni_analyser.py I developed a script that would "simulate" a theoretical Viking Age zooarchaeological assemblage of ovicaprines, cattle and pigs. The script generates between 50 and 500 sample IDs in the relative numbers one would expect to observe on an average Danish Viking Age site (~30 % ovicaprines, ~30 % cattle and ~40 % pig). The ratios were calculated from the average prevalence of ovicaprines, cattle and pigs from 18 Danish sites dated to the Viking Age. 

**Notes**

All of my scripts are available from GitHub and you are free to use and modify them as you see fit. They are very much still a work in progress and might not suit everyone's needs. 


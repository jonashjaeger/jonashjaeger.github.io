---
layout: archive
title: "Coding"
permalink: /coding/
author_profile: true
---
In the wake of large language models and AI's like ChatGPT-4 I started to slowly develop an interest in coding - particularly because I figured that it would be great use of my time to spend a few hours writing some code if it could save me many hours of work. However, coming from a humanities background as well as being born a decade or two too soon to have coding being part of the elementary school curriculum, writing code has never been part of *my* curriculum. 

And even if I've wanted to learn how to code for years I never managed to get started. However, with the aid of GPT-4 coding suddenly became accessible even to me and while GPT-4 does most of the hard work I am able to write a basic script in R or Python by now. 

**[mni_analyser.py](https://github.com/jhj-proteomics/mni_analyser)**

For my PhD, I had to sample several zooarchaeological remains for ZooMS analysis. However, my main concern was to avoid sampling the same individual twice. To avoid that I wanted to develop a simple script that could take the information in a zooarchaeological dataset and automatically identify which sample IDs were likely to represent bone elements from a single individual. However, to do so, I had to develop a second script that generated a theoretical zooarchaeological dataset to use in the script. 

**[assemblage_generator.py](https://github.com/jhj-proteomics/assemblage_generator)**

To test mni_analyser.py I developed a script that would "simulate" a theoretical Viking Age zooarchaeological assemblage of ovicaprines, cattle and pigs. The script generates between 50 and 500 sample IDs in the relative numbers one would expect to observe on an average Danish Viking Age site (~30 % ovicaprines, ~30 % cattle and ~40 % pig). The ratios were calculated from the average prevalence of ovicaprines, cattle and pigs from 18 Danish sites dated to the Viking Age. 

**Notes**

All of my scripts are available from GitHub and you are free to use and modify them as you see fit. They are very much still a work in progress and might not suit everyone's needs. 


---
layout: archive
title: "Coding"
permalink: /coding/
author_profile: true
---
In the age of Large Language Models or Artificial "Intelligences" like ChatGPT4 I have slowly started to develop an interest in writing code - primarily R and Python - particularly because after playing around with GPT4 I figured that I could probably save some time on my project if I had a bunch of 1s and 0s doing some of the work for me. As Bill Gates probably said: "Work smarter - not harder". 

However, being born in 1990, coding in any way, shape or form was never part of my primary (or secondary) school curriculum. And coming from a hard humanities background it wasn't part of my university education either. So, even If I've tried to learn a bit of coding for years I never managed to get started. But with the aid of GPT4, I was suddenly able to write code that actually *did* something. And here is a few (poor) examples at that - nonetheless it's code that I've actively used for my own research. 

**[mni_analyser.py](https://github.com/jhj-proteomics/mni_analyser)**

For my PhD, I had to sample several zooarchaeological remains for ZooMS analysis. However, my main concern was to avoid sampling the same individual twice. To avoid that I wanted to develop a simple script that could take the information in a zooarchaeological dataset and automatically identify which sample IDs were likely to represent bone elements from a single individual. However, to do so, I had to develop a second script that generated a theoretical zooarchaeological dataset to use in the script which became assemblage_generator.py.

**[assemblage_generator.py](https://github.com/jhj-proteomics/assemblage_generator)**

To test mni_analyser.py I developed a script that would "simulate" a theoretical Viking Age zooarchaeological assemblage of ovicaprines, cattle and pigs. The script generates between 50 and 500 sample IDs in the relative numbers one would expect to observe on an average Danish Viking Age site (~30 % ovicaprines, ~30 % cattle and ~40 % pig). The ratios were calculated from the average prevalence of ovicaprines, cattle and pigs from 18 Danish sites dated to the Viking Age. 

**[rename4platemapTSV.py](https://github.com/jhj-proteomics/rename4platemapTSV)**

This script renames .tsv files created using mzxml2tsv.py according to a .csv file of the corresponding MALDI plate map.

The script requires a "clean" plate map in .csv format. And with "clean" I mean that the plate map should only contain the individual placement of spots and their corresponding names. Not the "coordinate" rows (fx 1-24) or columns (A-P).

Samples spotted in triplicate (or more) will be named [samplename_1.tsv] for the first spot, [samplename_2.tsv] for the second spot and [samplename_3.tsv] for the third and so on.

**[rename4platemapTXT.py](https://github.com/jhj-proteomics/rename4platemapTXT)**

This script renames .txt files created using mzxml2txt.py according to a .csv file of the corresponding MALDI plate map.

The script requires a "clean" plate map in .csv format. And with "clean" I mean that the plate map should only contain the individual placement of spots and their corresponding names. Not the "coordinate" rows (fx 1-24) or columns (A-P).

Samples spotted in triplicate (or more) will be named [samplename_1.txt] for the first spot, [samplename_2.txt] for the second spot and [samplename_3.txt] for the third and so on.

**[mzxml2tsv.py](https://github.com/jhj-proteomics/mzxml2tsv)**

This script reads mass spec data in .mzXML format and converts each spectrum to separate .tsv files which can be read using mMass v.5.5.0 or run through Bacollite.

**[mzxml2txt.py](https://github.com/jhj-proteomics/mzxml2txt)**

This script reads mass spec data in .mzXML format and converts each spectrum to separate .txt files which can be read using mMass v.5.5.0 or run through Bacollite.

**[ProteoLinguistics.py](https://github.com/jhj-proteomics/ProteoLinguistics)**

Have you ever contemplated the potential of individual proteins concealing patterns or messages within their amino acid sequences? While these molecules don't carry deliberate messages, the exploration of such patterns can offer an intriguing lens into molecular biology.

With rigorous methodology and the integration of computational tools, I've developed (in collaboration with ChatGPT-4) a robust script. This script processes .fasta files, commonly sourced from databases like UniProt, by cross-referencing them against a comprehensive English dictionary. The outcomes of this analysis are systematically compiled into a .csv file, offering a structured yet fascinating perspective on coincidental linguistic patterns in protein sequences.

For users with an extensive collection of .fasta files, our script is optimized to handle batch processing of an entire directory. However, should you require a singular file analysis, some modifications to the script will be necessary.

This repository houses both the script and the wordlist. The onus of procuring the .fasta files for investigation remains with the user, adding an element of research initiative.

I invite you to delve into this confluence of linguistics and molecular biology.

Happy analyzing!

**Notes**

All of my scripts are available from GitHub and you are free to use and modify them as you see fit. They are very much still a work in progress and might not suit everyone's needs. 


---
title: "SemViz"
subtitle: Semantic Visualization of Scientific Data
layout: page
---

# Exploration and Discovery of the Covid-19 Literature through Semantic Visualization

##### Jingxuan Tu, Marc Verhagen, Kyeongmin Rim, Kelley Lynch, Peter Anick, Nikhil Krishnaswamy, James Pustejovsky (Brandeis)
##### Keith Suderman, Nancy Ide (Vassar)
##### Brent Cochran (Tufts)
###### Contact: [jamesp@brandeis.edu](mailto:jamesp@brandeis.edu)
---

We are developing semantic visualization techniques in order to enhance  exploration and enable discovery over large datasets of complex networks of relations. <i>Semantic visualization</i> is a method of enabling exploration and
discovery over large datasets of complex networks by exploiting the
semantics of the relations in them.  This involves (i) NLP to extract
named entities, relations and knowledge graphs from the original data;
(ii) indexing the output and creating representations for all relevant
entities and relations that can be visualized in many different ways,
e.g., as wordclouds, heat maps, graphs, etc.; (iii) applying parameter
reduction operations to the extracted relations, creating "relation
containers," or functional entities that can also be visualized using
the same methods, allowing the visualization of multiple relations,
partial pathways, and exploration across multiple dimensions.  Our
hope is that this will enable the discovery of novel inferences over
relations in complex data that otherwise would go unnoticed. 
We have applied this to analysis of the recently released [Covid-19 dataset](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge). 

We have also developed an NLP Question Answering system called the [Covid-QA System](http://services.lappsgrid.org/eager/ask), based on our [Language Application Grid](https://galaxy.lappsgrid.org/) platform within the [Galaxy](https://galaxyproject.org/) environment. 

 

* [Semantic Visualization](http://morbius.cs-i.brandeis.edu:23762/app/kibana#/dashboard/51bf2350-79d4-11ea-84c5-0f2dcbb991c3) of Heng Ji's [Blender Lab](http://blender.cs.illinois.edu/covid19/)  Covid-19 [Knowledge Graphs](http://blender.cs.illinois.edu/covid19/) from University of Illinois.
  * This shows the semantic visualization of the relations in the Covid-19 dataset encoded by Ji's group as knowledge graphs, between chemical-gene, chemical-disease, and gene-disease. In addition, parameter reduction has been performed on some relations, in order to illustrate heatmaps encoding relations between relations. For example, by encoding a known chemical as a specific gene inhibitor class, this class can be cross correlated with diseases  known to interact with just the chemical. This provides a capability for generating inferences over groups or classes of gene or chemical types and their behaviors. 
  
* [Semantic Visualization](http://morbius.cs-i.brandeis.edu:23762/app/kibana#/dashboard/2b613e90-7cf0-11ea-8a44-496b85e05ba5) of Harvard Protein-protein-causal-assertions (PPCA) [dataset](http://ndexbio.org/#/network/a8c0decc-6bbb-11ea-bfdc-0ac135e8bacf)
  * This demonstrates several visualizations over data extracted from 9,000 of the 52,000 articles in the CORD-19 dataset by multiple machine reading systems including [REACH](http://agathon.sista.arizona.edu:8080/odinweb/) (University of Arizona) and Sparser ([Smart Information Flow Technologies](https://www.sift.net/)). Extracted events were assembled by the Integrated Network and Dynamical Reasoning Assembler (INDRA), developed at Harvard Medical School: https://indralab.github.io.


* [LAPPSGrid](http://www.lappsgrid.org/) [Covid-QA System](http://services.lappsgrid.org/eager/ask)
  * The Language Applications (LAPPS) Grid AskMe document retrieval service provides sophisticated, customizable search capabilities over 14,000 full text articles related to COVID-19 research. The COVID data currently include all articles from the [CORD-19 dataset](https://pages.semanticscholar.org/coronavirus-research), eliminating duplicates, empty article files, etc. Searches over PubMed, PMC, bioRxiv and medRxiv will be available soon. Updates will be done weekly or when new data warrants.

 

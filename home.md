
# Exploration and Discovery of the Covid-19 Literature through Semantic Visualization

##### Jingxuan Tu, Marc Verhagen, Kyeongmin Rim, Kelley Lynch, Peter Anick, Nikhil Krishnaswamy, James Pustejovsky ([Brandeis](https://www.brandeis.edu/computer-science/))
##### Keith Suderman, Nancy Ide (Vassar)
##### Brent Cochran (Tufts)
###### Contact: [jamesp@brandeis.edu](mailto:jamesp@brandeis.edu)
---

We are developing semantic visualization techniques in order to enhance  exploration and enable discovery over large datasets of complex networks of relations. *Semantic visualization* is a method of enabling exploration and
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
We have applied this to analysis of the recently released [CORD-19 dataset](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge){:target="_blank"}. 

We have also developed an NLP Question Answering system called the [Covid-QA System](http://services.lappsgrid.org/eager/ask){:target="_blank"}, based on our [Language Application Grid](https://galaxy.lappsgrid.org/){:target="_blank"} platform within the [Galaxy](https://galaxyproject.org/){:target="_blank"}. 

 

* [Semantic Visualization](http://morbius.cs-i.brandeis.edu:23762/app/kibana#/dashboard/51bf2350-79d4-11ea-84c5-0f2dcbb991c3){:target="_blank"} of Heng Ji's [Blender Lab](http://blender.cs.illinois.edu/covid19/){:target="_blank"} Covid-19 [Knowledge Graphs](http://blender.cs.illinois.edu/covid19/){:target="_blank"} from University of Illinois.
  * This shows the semantic visualization of the relations in the CORD-19 dataset encoded by Ji's group as knowledge graphs, between chemical-gene, chemical-disease, and gene-disease. In addition, parameter reduction has been performed on some relations, in order to illustrate heatmaps encoding relations between relations. For example, by encoding a known chemical as a specific gene inhibitor class, this class can be cross correlated with diseases  known to interact with just the chemical. This provides a capability for generating inferences over groups or classes of gene or chemical types and their behaviors. 
  <a href="https://www.semviz.org/Blender/" target="_blank">Information on navigating the Blender dashboard</a>.

* [Semantic Visualization](http://morbius.cs-i.brandeis.edu:23762/app/kibana#/dashboard/2b613e90-7cf0-11ea-8a44-496b85e05ba5){:target="_blank"} of Harvard Protein-protein-causal-assertions (PPCA) [dataset](http://ndexbio.org/#/network/a8c0decc-6bbb-11ea-bfdc-0ac135e8bacf){:target="_blank"}.
  * This demonstrates several visualizations over data extracted from 9,000 of the 52,000 articles in the CORD-19 dataset by multiple machine reading systems including [REACH](http://agathon.sista.arizona.edu:8080/odinweb/){:target="_blank"} (University of Arizona) and Sparser ([Smart Information Flow Technologies](https://www.sift.net/){:target="_blank"}). Extracted events were assembled by the Integrated Network and Dynamical Reasoning Assembler ([INDRA](https://indralab.github.io){:target="_blank"}), developed at Harvard Medical School. <a href="https://www.semviz.org/INDRA-PPI/" target="_blank">Information on navigating the Harvard dashboard</a>.

* [LAPPSGrid](http://www.lappsgrid.org/){:target="_blank"} [Covid-QA System](http://services.lappsgrid.org/eager/ask){:target="_blank"}
  * The Language Applications (LAPPS) Grid AskMe document retrieval service provides sophisticated, customizable search capabilities over 14,000 full text articles related to COVID-19 research. The data currently include all articles from the [CORD-19 dataset](https://pages.semanticscholar.org/coronavirus-research){:target="_blank"}, eliminating duplicates, empty article files, etc. Searches over PubMed, PMC, bioRxiv and medRxiv will be available soon. Updates will be done weekly or when new data warrants.

---
 
This research is supported in part by grants from: DARPA grant
 FA8750-18-2-0016; DARPA grant W911NF-15-C-0238; DTRA grant
 DTRA-16-1-0002; NSF grant 1811402; and  Andrew W. Mellon  Foundation grants G-1901-06505 and G-1810-06248.
 
 <div style="text-align:center"><a href="https://www.brandeis.edu"><img src="{{ 'img/brandeis-logo-stacked-seal-blue-digital.png' | relative_url }}" width="240"/></a></div>
 

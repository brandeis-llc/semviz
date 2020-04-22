---
layout: post
title: Harvard PPI dataset viz Dashboard
subtitle: Placeholder
---

This dashboard demonstrates the visualization of the events that were assembled 
by the Integrated Network and Dynamical Reasoning Assembler ([INDRA](https://indra.readthedocs.io/en/latest/index.html)). 
All the PPI events were divided into 16 categories (full list can be found [here](https://indra.readthedocs.io/en/latest/modules/statements.html#)). 
Furthermore, from a high level, to enhance the biological understanding of the proteins involved in these events, 
we categorize the PPI events into 2 meta groups, namely `Modification` and `RegulateActivity`. Protein agents in `Modification` can be labeled as `Subject` protein or `Object` protein, 
while those in `RegulateActivity` can be labeled as `Enzyme` protein or `Substrate` protein.

## Description of Visualization Pins

### Containers Word Cloud

This word cloud shows the frequency of various gene/protein containers extracted from PPCA dataset. 
For example, `apoptotic process Activator` is a list of proteins that are found to be able to activate `apoptotic process`. Similarly, `EIF2S1 Phosphorylator` contains a list of proteins that are found to have phosphorylation with some other genes.

### Enzymes Word Cloud
This word cloud shows the frequency of proteins that can be the enzymes in the `Modification` relation.

### Subjects Word Cloud
This word cloud shows the frequency of proteins that can be the subjects in the `RegulateActivity` relation.

### Subject-Object Interactions 
This heat map shows the co-occurrence of subject and object proteins. 
For example, if we take the intersection block of the fourth row and second column, 
we can get `DDX58` and `Interferon`. It means this pair of proteins can express one or more types of `RegulateActivity` relations.

### Enzyme-Substrate Interactions
This heat map shows the co-occurrence of enzymes and substrate. 
For example, if we take the intersection block of the second row and first column, 
we can get `EIF2AK2` and `EIF2S1`. It means this pair of proteins can express one or more types of `Modification` relations. 
The first row shows the frequency of `Modification` relations that have substrates only.

### Subject-Object Interactions - Activation
This one is similar to _Subject-Object Interactions_ except that the relation can only be `Activation`.

### Subject-Object Interactions - Inhibition
This one is similar to _Subject-Object Interactions_ except that the relation can only be `Inhibition`.

### Container-Object Interactions
This heat map shows the co-occurrence of protein containers and subject proteins. 
For example, if we take the first column, it shows Interferon could be `JAK activator` and `STAT Activator`, etc.

### Keyword-Journal Relations
This heat map shows the co-occurrence of a keyword in abstract with the journal names. 
For example, if our keyword is `Coronavirus`, we can get this keyword appears 149 times in articles published on `PLoS One`.

### Authors Word Cloud
This word cloud shows the authors of the articles that have been archived into COVID-19 dataset.

### Journal Publish Time Bar Chart
This bar chart shows the publish time of articles in each year and each month.

## Interactive Navigation Examples

- Click `EIF2S1 Phosphorylator` on _Containers Word Cloud_ → _Enzymes Word Cloud_ will 
tell you the members of this container → Keep adding more filters or clear for another navigation.
- Click the intersection of `Coronavirus` and `Virology` in _Keyword - Journal Relations_ → all the other pins will be updated. We can find `David A. Brian` from _Authors Word Cloud_, `SARS-CoV Palmitoylators` from _Containers Word Cloud_, etc. that are related to coronavirus.
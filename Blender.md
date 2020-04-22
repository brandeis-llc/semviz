---
layout: page
title: Blender Covid Visualization   
subtitle:  Navigating the Dashboard
---

This dashboard shows the semantic visualization of the relations in the CORD-19 
dataset encoded by Ji’s group as knowledge graphs, between chemical-gene, 
chemical-disease, and gene-disease. In addition, parameter reduction has been 
performed on some relations, in order to illustrate heatmaps encoding relations 
between relations. 53 fine-grained chemical-gene interaction types have been 
identified, and the interaction types are also combined with three actions to 
form the whole relation. 
For better visualization we do the following mapping to the three actions:
- Increase: ++
- Decrease: --
- Affect:   ->

## Description of Visualization Pins

### Chemical Word Cloud
This word cloud shows the frequency of various kinds of chemicals.

### Gene Word Cloud
This word cloud shows the frequency of various kinds of genes. 

### Chemical-Gene Interactions
This heat map shows the co-occurrence of chemical and gene per type of interaction. 
We can see several sub-heat maps and each one show one type of interaction.
For example, if we take the first sub-heatmap and the intersection block of the first row and first column, 
we can get `dorsomorphin` and `NOG`. It means dorsomorphin increases cotreatment of NOG.

### Chemical-Disease Interactions
This heat map shows the co-occurrence of chemical and disease. 
For example, if we take the intersection block of the first row and first column, 
we can get `Nifedipine` and `Hypertension`. It means there is some relation between the chemical Nifedipine and the disease Hypertension.

### Gene-Disease Interactions
This heat map shows the co-occurrence of gene and disease. 
For example, if we take the intersection block of the first row and first column, 
we can get `ERBB2` and `Breast Neoplasms`. It means there is some relation between the gene ERBB2 and the disease Breast Neoplasms.

### Container-Disease Interactions
This heat map shows the relation between gene container and disease per organism. 
There are two sub-heat maps. The one on the left shows the relations found in Home sapiens, 
while the one on the right shows the relations found in Mus musculus.
For example, if we take the first sub-heatmap and the intersection block of the fifth row and first column, 
we can get `++MAPK3 Phosphorylator` and `Prostatic Neoplasms`. It means the genes that have phosphorylation on
++MAPKS have some relation with the disease Prostatic Neoplasms. This allows us to demonstrate the "chained" relations
through parameter reduction.

## Interactive Navigation Examples
- Click `bisphenol A` on _Chemical Word Cloud_ → all the other pins will be updated. 
For example _Chemical-Gene Interactions_ will show us the interactions between bisphenol A and genes per type of interaction. 
_Container-Disease Interactions_ will show us the relation between diseases and gene containers that have a member called bisphenol A → 
Keep adding more filters or clear for another navigation.

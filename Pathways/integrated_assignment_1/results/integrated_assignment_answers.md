---
layout: post2
permalink: /PNAOD_integrated_assingment_1_2016/
title: Pathway and Network Analysis of -Omics Data 2016 Integrated Assignment
header1: Pathway and Network Analysis of -Omics Data 2016
header2: Integrated Assignment Part 1
image: CBW_pathway_icon.jpg
---

**This work is licensed under a [Creative Commons Attribution-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0/deed.en_US). This means that you are able to copy, share and modify the work, as long as the result is distributed under the same license.**

# Pathway and Network Analysis Integrated Assignment: Answers to questions and Screenshots

By Veronique Voisin


The results are stored in this [folder](https://github.com/bioinformaticsdotca/HT-Biology_2017/tree/master/Pathways/integrated_assignment_1/results).

## g:Profiler

**Question**: What is the most significant GO:term? What is the p-value for this GO:term 

**Answer**: extracellular matrix organization: p-value of 1.70e-09 


**Question**: Is this p-value already corrected for multiple testing? What type of correction is used for your current analysis? 

**Answer**: yes, it is already corrected for multiple hypothesis testing. I set the Significance threshold box to  "Benjaminin-Hochberg FDR". 

**g:Profiler png output**  
![INA1](https://github.com/bioinformaticsdotca/HT-Biology_2017/blob/master/Pathways/img/INA1.png?raw=true)

Re-run the analysis with User p-value threshold set to 0.0001. **Question**: What has been changed?
**Answer:** Only the gene-set with pvalue equal or less than 0.0001 are displayed. The list is reduced compared to the results obtained with the default settings. 

Ordered query: **Question**: Do you seen any changes in the output in comparison to the analysis of the unordered gene list (PART 2) **Answer** Although some terms are similar, their pvalues changed as well as the number of term genes used to calculate the pvalue.

**EnrichmentMap input panel** 

![INA2](https://github.com/bioinformaticsdotca/HT-Biology_2017/blob/master/Pathways/img/INA2.png?raw=true)

## GSEA

**GSEA input panel**  
![INA1](https://github.com/bioinformaticsdotca/HT-Biology_2017/blob/master/Pathways/img/INA3.png?raw=true)
 
** GSEA EnrichmentMap input panel** 

![INA2](https://github.com/bioinformaticsdotca/HT-Biology_2017/blob/master/Pathways/img/INA4.png?raw=true)

## DATASET2

## PART1 REACTOME FI

Pathway enrichment on the whole network. **Question** What is the pathway with the lowest (best) FDR?
** Answer**

Cluster the network and perform pathway enrichment on the network. **Question** How many clusters did the analysis retrieve? 



---
layout: workshop_main_7day
permalink: /high-throughput_biology_2017
title: HT-Biology
header1: Workshop Pages for Students
header2: High-Throughput Biology - From Sequence to Networks 2017
image: /site_images/CBW-CSHL-graphic-square.png
keywords: Experience in cloud computing and data visualization tools, analyze DNA- and RNA- sequence reads, evaluate sequence read quality
description: Course covers the key bioinformatics concepts and tools required to analyze DNA- and RNA- sequence reads using a reference genome.
instructors: Jared Simpson, Florence Cavalli, Mahieu Bourgey, Malachi Griffith, Fouad Yousif, Obi Griffith, Jüri Reimand, Veronique Voisin, Robin Haw, Quaid Morris, Micheal Hoffman
length: 7 days
---

# Welcome <a id="welcome"></a>

Welcome to High-Throughpyt Biology: From Sequence to Networks.  

The course schedule can be found [here](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_schedule).

If you have questions or comments, visit the workshop [Q&A forum](https://noteapp.com/CSHL2017).

We value your feedback.  Please complete [our survey](https://goo.gl/forms/Lpt0g1PVvs9cRSUb2).  

***

# Pre-Workshop Materials <a id="preworkshop"></a>

## Laptop Setup Instructions

Instructions to setup your laptop can be found [here](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_laptop_setup).

## Pre-workshop Tutorials

1) **R Preparation tutorials**: You are expected to have completed the following tutorials in **R** beforehand. The tutorial should be very accessible even if you have never used **R** before.

* The [CBW R tutorial](http://bioinformatics-ca.github.io/CBW_R_Tutorial/)
* [Quick and Dirty Guide to **R**](http://ww2.coastal.edu/kingw/statistics/R-tutorials/text/quick&dirty_R.txt)  
* The [R Tutorial](http://www.cyclismo.org/tutorial/R/) up to and including 5. Basic Plots
* The [R command cheat sheet](../../resources/R_Short-refcard.pdf)

2) **UNIX Preparation tutorials**:  

* [UNIX Bootcamp](https://github.com/griffithlab/rnaseq_tutorial/wiki/Unix-Bootcamp)
* Tutorials #1-3 on [UNIX Tutorial for Beginners](http://www.ee.surrey.ac.uk/Teaching/Unix/)  
* [Unix Cheat sheet](http://www.rain.org/~mkummel/unix.html) 

3) [Sequencing Terminology](http://www.ncbi.nlm.nih.gov/projects/genome/glossary.shtml)

4)  **Cytoscape Preparation tutorials**: Complete the [introductory tutorial to Cytoscape](http://opentutorials.cgl.ucsf.edu/index.php/Portal:Cytoscape3)

* Introduction to Cytoscape3 - User Interface

* Introduction to Cytoscape3 - Welcome Screen

* Filtering and Editing in Cytoscape 3

###  Pre-workshop Readings  

  Before coming to the workshop, read these:
  
  * [Using cloud computing infrastructure with CloudBioLinux, CloudMan, and Galaxy](http://www.ncbi.nlm.nih.gov/pubmed/22700313)
  
  * [Integrative Genomics Viewer (IGV): high-performance genomics data visualization and exploration](http://www.ncbi.nlm.nih.gov/pubmed/22517427)
  
  * [Genome structural variation discovery and genotyping](http://www.ncbi.nlm.nih.gov/pubmed/21358748)
  
  * [A survey of sequence alignment algorithms for next-generation sequencing](http://www.ncbi.nlm.nih.gov/pubmed/20460430)
  
  * [Genotype and SNP calling from next-generation sequencing data](http://www.ncbi.nlm.nih.gov/pubmed/21587300)
  
  * [Differential gene and transcript expression analysis of RNA-seq experiments with TopHat and Cufflinks](http://www.ncbi.nlm.nih.gov/pubmed/22383036)
  
  * [ENCODE RNA-Seq Standards](https://genome.ucsc.edu/ENCODE/protocols/dataStandards/ENCODE_RNAseq_Standards_V1.0.pdf)
  
  * [Methods to study splicing from high-throughput RNA sequencing data](http://www.ncbi.nlm.nih.gov/pubmed/24549677)
  
  * [Differential analysis of gene regulation at transcript resolution with RNA-seq](http://www.ncbi.nlm.nih.gov/pubmed/23222703)
  
  * [A comprehensive assessment of RNA-seq accuracy, reproducibility and information content by the Sequencing Quality Control Consortium](http://www.ncbi.nlm.nih.gov/pubmed/25150838)
  
  * [Recurrent chimeric RNAs enriched in human prostate cancer identified by deep sequencing](http://www.ncbi.nlm.nih.gov/pubmed/21571633)
  
  * [iRegulon: From a Gene List to a Gene Regulatory Network Using Large Motif and Track Collections](http://www.ncbi.nlm.nih.gov/pubmed/25058159)
  
  * [The GeneMANIA prediction server: biological network integration for gene prioritization and predicting gene function](http://www.ncbi.nlm.nih.gov/pubmed/20576703)
  
  * [GeneMANIA Prediction Server 2013 Update](http://www.ncbi.nlm.nih.gov/pubmed/23794635)
  
  * [How to visually interpret biological data using networks](http://www.ncbi.nlm.nih.gov/pubmed/19816451)
  
  * [g:Profiler--a web-based toolset for functional profiling of gene lists from large-scale experiments](http://www.ncbi.nlm.nih.gov/pubmed/17478515)
  
  * [g:Profiler--a web server for functional interpretation of gene lists (2011 update)](http://www.ncbi.nlm.nih.gov/pubmed/21646343)
  
  * [Gene set enrichment analysis: a knowledge-based approach for interpreting genome-wide expression profiles](http://www.ncbi.nlm.nih.gov/pubmed/16199517)
  
  * [Expression data analysis with reactome](http://www.ncbi.nlm.nih.gov/pubmed/25754994)  

***

# Logging into the Amazon Cloud <a id="amazon_cloud"></a>
 
* We have set up 30 instances on the Amazon cloud - one for each student. In order to log in to your instance, you will need a security certificate. If you plan on using Linux or Mac OS X, please download [this certificate](http://cbwmain.dyndns.info/private/CBWNY.pem). Otherwise if you plan on using Windows (with Putty and Winscp), please download [this certificate](http://cbwmain.dyndns.info/private/CBWNY.ppk).

* Detail instructions can be found [here](https://bioinformaticsdotca.github.io/AWS_setup).

# Day 1 <a id="day1"></a>

## Welcome

*<font color="#827e9c">Ann Meyer</font>*

## Module 1: Introduction to High-throughput Sequencing

*<font color="#827e9c">Jared Simpson</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1Z9a1f2yXh1vb2pns3tukOdcUbOmtc9p9/view?usp=sharing)

[Recording](https://youtu.be/jibOh1xqtSs)

## Module 2: Data Visualization

*<font color="#827e9c">Florence Cavalli</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1snsoqquDgJ8o7fg8TsIGNHvE2cRqskyP/view?usp=sharing)

[Recording](https://youtu.be/6KDfuRyoTik)

[Lab Practical](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module2_lab)

## Module 3: Genome Alignment

*<font color="#827e9c">Mathieu Bourgey</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1WE2VDPpWp6g01EEUueMGJ4BPEhtPZBW7/view?usp=sharing)

[Recording](https://youtu.be/cGo1DWSxuC0)

[Lab Practical: Connecting to the Cloud](http://bioinformaticsdotca.github.io/AWS_setup)

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/17RZT3rgA-WYUmIC-P432og0GWzUSYvnb/view?usp=sharing)  

* We have set up 30 instances on the Amazon cloud - one for each student. In order to log in to your instance, you will need a security certificate. If you plan on using Linux or Mac OS X, please download [this certificate](http://cbwmain.dyndns.info/private/CBWNY.pem). Otherwise if you plan on using Windows (with Putty and Winscp), please download [this certificate](http://cbwmain.dyndns.info/private/CBWNY.ppk).

[Lab Practical](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module3_lab)  
[Lab Practical on GitHub](https://github.com/mbourgey/CBW_HTseq_module3/blob/master/README.md)

***

# Day 2 <a id="day2"></a>

## Module 4: Small-Variant Calling and Annotation

*<font color="#827e9c">Mathieu Bourgey</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1QdL4jgNXF5GC9WoHtZ25O_zab8KdqJeU/view?usp=sharing)

[Recording](https://youtu.be/oIiGfrrXP34)

[Lab Practical](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module4_lab)  
[Lab Practical on GitHub](https://github.com/mbourgey/CBW_HTseq_module4/blob/master/README.md)

## Module 5: Structural Variant Calling

*<font color="#827e9c">Mathieu Bourgey</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1xlBr1spRZvRCs6a4H45bCek_T1FZHTbo/view?usp=sharing)

[Recording](https://youtu.be/XBedpQ3F5e0)

[Lab Practical](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module5_lab)  
[Lab Practical on GitHub](https://github.com/mbourgey/CBW_HTseq_module5/blob/master/README.md)  

## Module 6: De Novo Assembly

*<font color="#827e9c">Jared Simpson</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1YjOOm7RZQxeh0igW23xVl9WhLXO4o9jw/view?usp=sharing)

[Recording](https://youtu.be/tukKgTeaBTU)

[Lab Practical](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module6_lab)

[Supplemental](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module6_lab_supplement)

## Integrated Assignment

[Integrated Assignment](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_IA_HTBio_lab)

***

# Day 3 <a id="day3"></a>

**Day 3 and Day 4 refer to content in the [RNA-Seq wiki](https://github.com/griffithlab/rnaseq_tutorial/wiki).**

## Module 7: Introduction to RNA Sequencing Analysis

*<font color="#827e9c">Malachi Griffith</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1Ldp6qrAMy0NVCCAu5cueT4YFq0VArORH/view?usp=sharing)

[Recording](https://youtu.be/YzkTc6VNNjo)

### Lab Practical

[Lab practical](https://drive.google.com/a/bioinformatics.ca/file/d/1g1p3FH9bmWtAagAf07z6RIh1azlBoFZK/view?usp=sharing)

  [Installation](https://github.com/griffithlab/rnaseq_tutorial/wiki/Installation)
  
  [Reference Genomes](https://github.com/griffithlab/rnaseq_tutorial/wiki/Reference-Genome)
  
  [Annotations](https://github.com/griffithlab/rnaseq_tutorial/wiki/Annotation)
  
  [Indexing](https://github.com/griffithlab/rnaseq_tutorial/wiki/Indexing)
  
  [Data](https://github.com/griffithlab/rnaseq_tutorial/wiki/RNAseq-Data)
  
  [Data QC](https://github.com/griffithlab/rnaseq_tutorial/wiki/PreAlignment-QC)


## Module 8: RNA-seq Alignment and Visualization

*<font color="#827e9c">Fouad Yousif</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1I_Mb27hLQOkpc5diZxY5vXcn0A5GEpSl/view?usp=sharing)

[Recording](https://youtu.be/RxqWuC_I1p0)

### Lab Practical

[Lab Practical](https://drive.google.com/a/bioinformatics.ca/file/d/1lXr2hCVg0sizDganGlcMmEOv8a1PRG5v/view?usp=sharing)

  [Adapter Trim](https://github.com/griffithlab/rnaseq_tutorial/wiki/Adapter-Trim)
  
  [Alignment](https://github.com/griffithlab/rnaseq_tutorial/wiki/Alignment)
  
  [IGV](https://github.com/griffithlab/rnaseq_tutorial/wiki/IGV-Tutorial)

  [Alignment Visualization](https://github.com/griffithlab/rnaseq_tutorial/wiki/PostAlignment-Visualization)
  
  [Alignment QC](https://github.com/griffithlab/rnaseq_tutorial/wiki/PostAlignment-QC)

## Integrated Assignment

*<font color="827e9c">Fouad Yousif</font>*

Paper: [Recurrent chimeric RNAs enriched in human prostate cancer identified by deep sequencing](http://www.ncbi.nlm.nih.gov/pubmed/21571633)

[Assignment Questions](https://github.com/griffithlab/rnaseq_tutorial/wiki/Integrated-Assignment)

[Assignment Answers](https://github.com/griffithlab/rnaseq_tutorial/wiki/Integrated-Assignment-Answers)  


***

# Day 4 <a id="day4"></a>

## Module 9: Expression and Differential Expression

*<font color="#827e9c">Obi Griffith</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1dL3lwl65ocKEagYoqkFDlJaEFTUg8I61/view?usp=sharing)

[Recording](https://youtu.be/7mRXZ1EuyYo)

### Lab Practical

[Lab Practical](https://drive.google.com/a/bioinformatics.ca/file/d/1b5YS60Yi48ZwS7bm4bnZjFyn1AR0f-99/view?usp=sharing)

 [Expression](https://github.com/griffithlab/rnaseq_tutorial/wiki/Expression)
 
 [Differential Expression](https://github.com/griffithlab/rnaseq_tutorial/wiki/Differential-Expression)
 
 [DE Visualization](https://github.com/griffithlab/rnaseq_tutorial/wiki/DE-Visualization)

## Module 10: Reference Free Alignment

*<font color="#827e9c">Malachi Griffith</font>* 

[Kallisto](https://github.com/griffithlab/rnaseq_tutorial/wiki/Kallisto)  

## Module 11: Isoform Discovery and Alternative Expression

*<font color="#827e9c">Malachi Griffith</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1bwYZvoAb_R9OgL93Fag_rGp5UHEOmfwP/view?usp=sharing)

[Recording](https://youtu.be/fs-FEdBYpMY)

### Lab Practical

[Lab Practical](https://drive.google.com/a/bioinformatics.ca/file/d/1_8P8z_se3O5nn8rQ0cCS5YP_2NH3l-z0/view?usp=sharing)

  [Ref Guided](https://github.com/griffithlab/rnaseq_tutorial/wiki/Reference-Guided-Transcript-Assembly)
  
  [De novo](https://github.com/griffithlab/rnaseq_tutorial/wiki/de-novo-Transcript-Assembly)
  
  [Merging](https://github.com/griffithlab/rnaseq_tutorial/wiki/Transcript-Assembly-Merge)
  
  [Differential Splicing](https://github.com/griffithlab/rnaseq_tutorial/wiki/Differential-Splicing)
  
  [Splicing Visualization](https://github.com/griffithlab/rnaseq_tutorial/wiki/Transcript-Assembly-Visualization)

## Integrated Assignment

[Assignment Questions](https://github.com/griffithlab/rnaseq_tutorial/wiki/Integrated-Assignment)  

[Assignment Answers](https://github.com/griffithlab/rnaseq_tutorial/wiki/Integrated-Assignment-Answers)  

## Keeping Up-to-date with RNA-Seq Analysis Developments

For additional resources, tutorials, future directions, and more please refer to the [RNA-seq wiki](http://www.rnaseq.wiki/)

***

# Day 5 <a id="day5"></a>

## Module 12: Introduction to Pathway and Network Analysis

*<font color="#827e9c">Jüri Reimand</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1wjNo1v5ou5xCtxXbxtsr6WBDjvySlKh-/view?usp=sharing)

[Recording](https://youtu.be/PqH8yR97DUY)

## Module 13: Finding Over-Represented Pathways

*<font color="#827e9c">Jüri Reimand</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1DtW2HCuMypb4GiT1Pk8JvnFFv_s1odIw/view?usp=sharing)

[Recording](https://youtu.be/bArrgs4lUjg)

### Lab practical: Enrichment-Based Analysis - Performing ORA
  *<font color="#827e9c">Jüri Reimand and Veronique Voisin</font>*

[Introduction](https://drive.google.com/a/bioinformatics.ca/file/d/1Rro2qwEuAAWego2undL89NYTaI5OHbuU/view?usp=sharing)

gProfiler

[Exercise 1](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module13_lab_2)  
  
[Precomputed results for exercise 1](https://github.com/bioinformatics-ca/bioinformatics-ca.github.io/raw/master/2016_workshops/pathways/module2_lab/gprofiler_results_mesenchymal.txt)   

GSEA
[Exercise 2](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module13_lab_1)  

[Precomputed results for Exercise 2](https://github.com/bioinformatics-ca/bioinformatics-ca.github.io/raw/master/2016_workshops/pathways/module2_lab/Mesen_vs_Immuno_edgeR.GseaPreranked.1465326037884.zip)  


## Module 14: Network Visualization and Analysis with Cytoscape

*<font color="#827e9c">Veronique Voisin</font>* 

[Lecture Part 1](https://drive.google.com/a/bioinformatics.ca/file/d/1qSWv5jHx-RHXuvtcmpAhR3E6k67jEjqJ/view?usp=sharing)  

[Lecture Part 2](https://drive.google.com/a/bioinformatics.ca/file/d/1G6Y6_53SwxumlNXsLb-MgbGUhEdrApxH/view?usp=sharing)  

[Recording](https://youtu.be/FStbZ8q8-5Q)

### Lab practical: Cytoscape Demo, Enrichment Map
  *<font color="#827e9c">Veronique Voisin</font>*


[Exercise 1](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module14_lab_1)  
  
[Exercise 2](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module14_lab_2)  

***

# Day 6 <a id="day6"></a>

## Module 15: More Depth on Network and Pathway Analysis

*<font color="#827e9c">Robin Haw</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/13UF43mGulKVjdkNh4dSUyzUQVdf_ARn5/view?usp=sharing)

[Recording](https://youtu.be/eBswO29PR8A)

### Lab practical: *De Novo* Subnetwork Clustering Analysis in Reactome

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1svhoYrhkY9btl10ib3DZWqvfTwR5QVmX/view?usp=sharing)  

[Lab Practical](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module15_lab) 

[Lab answers](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module15_lab_answers)  

## Module 16: Gene Function Prediction

*<font color="#827e9c">Quaid Morris</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1eN3IoWWn8HV2Oz4zAP7EYmKRi9dIu_U4/view?usp=sharing)   

[Recording](https://youtu.be/X23PlnOjzRc)

[Lab Practical](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module16_lab)  

## Integrated Assignment
[Integrated Assignment](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_path_integrated_assignment)

[Integrated Assignment Answers](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_path_integrated_assignment_answers)

***

# Day 7 <a id="day7"></a>

## Module 17: Regulatory Network Analysis

*<font color="#827e9c">Michael Hoffman</font>* 

[Lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1KtQ8Co4CG6sFkFC520V2VO3J7DFjUYnl/view?usp=sharing)

[Recording](https://youtu.be/WEHrbjK49l4)

#### Lab practical: iRegulon

*<font color="#827e9c">Veronique Voisin</font>*

[Lab lecture](https://drive.google.com/a/bioinformatics.ca/file/d/1jmIKs9xfyJcB_hmr9xgkjJB0C_CN8A2U/view?usp=sharing)  

[Lab practical](https://bioinformaticsdotca.github.io/high-throughput_biology_2017_module17_lab)  

[Precomputed results cys file](https://github.com/bioinformatics-ca/bioinformatics-ca.github.io/raw/master/2016_workshops/pathways/module6_lab/prostate_cancer_genemania_network.cys) and [Precomputed results irf file](https://github.com/bioinformatics-ca/bioinformatics-ca.github.io/raw/master/2016_workshops/pathways/module6_lab/iregulon_results.irf)  

To use the precomputed results:  

1) launch Cytoscape 

2) open the "prostate_cancer_genemania_network.cys" file 

3) go to App > iRegulon > 'Load results from the iregulon_results.irf file'  
  
[Download a zip file of the git repo here](https://github.com/bioinformaticsdotca/HT-Biology_2017/archive/master.zip)  



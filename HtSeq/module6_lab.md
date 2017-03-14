---
layout: tutorial_page
permalink: /high-throughput_biology_2017_module6_lab
title: HT-Biology Lab 6
header1: Workshop Pages for Students
header2: High-Throughput Biology - From Sequence to Networks Module 6 Lab
image: /site_images/CBW-CSHL-graphic-square.png
home: https://bioinformaticsdotca.github.io/high-throughput_biology_2017
---

# Genome Assembly for short and long reads

by [Jared Simpson](https://simpsonlab.github.io)

## Introduction

In this lab we will perform de novo genome assembly of a bacterial genome and a segment of the human genome. We will walk through a genome assembly starting with data quality control, through to building contigs and analysis of the results. At the end of the lab you will know:

1) How to perform basic quality checks on the input data
2) How to run a short read assembler on Illumina data
3) How to run a long read assembler on Pacific Biosciences or Oxford Nanopore data
4) How to compare the results of multiple assemblies

## Data Sets

In this lab we will use two data sets to demonstrate genome assembly. The first data set consists of sequencing reads for the bacteria Escherichia coli. E. coli is a great data set for getting starting on genome assembly as it is a small genome (4.6 Mbp) with relatively few repeats, and a very high quality reference. We have provided Illumina, PacBio and Oxford Nanopore reads for this genome. The second data set is a 5Mbp segment of the human genome. The human genome is much more repetitive than the E. coli genome, and is heterozygous, which makes assembly much more challenging. We've selected a 5Mbp segment of chromosome 20 for this exercise. Just like for E. coli we've provided Illumina, PacBio and Oxford Nanopore reads. Note that we're using a segment of the genome as trying to assemble the entire 3Gbp genome would take too long for this tutorial. When performing a real assembly you should expect the assembly to take much longer and require more memory.

## Data Preparation

First, lets create and move to a directory that we'll use to work on our assemblies:

```
mkdir -p ~/workspace/HTseq/Module6
cd ~/workspace/HTseq/Module6
```

For convenience, lets make symbolic links to the data sets that we'll work with. Run this command from the terminal, which will find all of the sequencing data sets we provided (using the `ls` command) and make a symlink of those files in your current working directory.


```
ls ~/CourseData/HT_data/Module6/* | xargs -i ln -s {}
```

If you run `ls` you should be able to see the input data sets.

## Data Quality Control

In the lecture we heard about many factors that may result in a poor assembly: not having enough coverage, very high repeat content, very high heterozygosity, etc. In this section of the lab we will use the [sga preqc](https://academic.oup.com/bioinformatics/article/30/9/1228/237596/Exploring-genome-characteristics-and-sequence) program to explore our data set before starting the assembly. We have two E. coli Illumina data sets - one at 15x coverage and one at 50x coverage. This will allow us to explore the effect of sequencing coverage on the results of our assembly.


First build an FM-index of the two E. coli Illumina data sets:

```
sga index -t 4 -a ropebwt ecoli.illumina.15x.fastq
sga index -t 4 -a ropebwt ecoli.illumina.50x.fastq
```

Next, we can run `sga preqc` to run the calculations and generate the PDF report. NOTE: these commands take about an hour to run. Rather than running them, you can download the finished report here: LINK TODO.

```
sga preqc -t 4 ecoli.illumina.15x.fastq > ecoli.illumina.15x.preqc
sga preqc -t 4 ecoli.illumina.50x.fastq > ecoli.illumina.50x.preqc
python sga-preqc-report.py ecoli.illumina.15x.preqc ecoli.illumina.50x.preqc
```

Open the PDF report and try to interpret the results. Was the genome size estimated correctly? What differences do you notice between the 15x and the 50x datasets?

## E. coli Genome Assembly with Short Reads

Now we'll assemble the E. coli 50x Illumina data using the [spades](http://bioinf.spbau.ru/spades) assembler. spades will automatically select values for its parameters (like the k-mer size) making it particularly easy to use:

```
spades.py -o ecoli-illumina-50-spades/ -t 4 --12 ecoli.illumina.50x.fastq
```

This should take about 15 minutes to run.

One of the first quality checks on the assembly is the total size and contiguity of the contigs. We want our assemblies to be /complete/; most of the genome should be assembled into contigs. We also want our assemblies to be /contiguous/; long contigs are better than short contigs as they give us more information about the structure of the genome. We'll use `abyss-fac` to calculate how complete and contiguous our assembly is. Typically there will be a lot of short "leftover" contigs when running the assembly consisting of repetitive or low-complexity sequence, or reads with a very high error rate. We don't want to include these in our statistics so we'll only use contigs that are at least 500bp in length:

```
abyss-fac.pl -t 500 ecoli-illumina-50-spades/contigs.fasta
```

The N50 statistic is the most commonly used measure of assembly contiguity. N50 of x means that 50% of the assembly is represented in contigs x bp or longer. What is the N50 of the spades assembly? What percentage of the genome was assembled in contigs 500bp or larger?

## E. coli Genome Assembly with Long Reads

Now, we'll use long sequencing reads to assemble the E. coli genome. Long sequencing reads are better at resolving repeats and typically give much more contiguous assemblies. Long reads have a much higher error rate than short reads though, so we need to use a different assembly strategy. In this tutorial, we'll use the [canu](https://github.com/marbl/canu) assembler to assemble the PacBio and Oxford Nanopore data.

```
canu gnuplotTested=true -p ecoli-pacbio-canu -d ecoli-pacbio-auto genomeSize=4.6m -pacbio-raw ecoli.pacbio.25x.fastq
```

Assembling the nanopore data set is similar:

```
canu gnuplotTested=true -p ecoli-nanopore-canu -d ecoli-nanopore-auto genomeSize=4.6m -nanopore-raw ecoli.nanopore.25x.fasta
```

## Assessing the accuracy of an assembly

The accuracy of the genome assembly is determined by how many misassemblies (large-scale rearrangements) and consensus errors (base substitutions, insertions or deletions) the assembler makes. To calculate the accuracy of an assembly typically requires the use of a reference genome. We will use the [QUAST](http://quast.bioinf.spbau.ru/) software package to assess the accuracy of the assemblies. Run QUAST on your three E. coli assemblies:

```
TODO
```

Now, also run it on the PacBio and nanopore assemblies:

```
TODO
```

Using the report generated by QUAST, determine which of the assemblies was a) the most complete b) the most contiguous and c) the most accurate.

## Improving the Accuracy of the Long Read Assemblies

As PacBio and Nanopore reads have a higher error rate than Illumina reads it is quite common to use the Illumina data to improve the accuracy of the long read assemblies. We'll use [Pilon](https://github.com/broadinstitute/pilon) to do this here:

```
TODO
```

After running pilon on the PacBio and nanopore assemblies, re-run Quast. Did the accuracy improve? How does the Illumina-corrected assembly compare to the Illumina-only assembly?

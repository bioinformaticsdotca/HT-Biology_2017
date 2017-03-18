---
layout: post2
permalink: 
title: Informatics for High-Throughput Sequencing Data 2017 Integrative Assignment
header1: Informatics for High-Throughput Sequencing Data 2017
header2: Integrative Assignment
image: CBW_High-throughput_icon.jpg
---


-----------------------

**This work is licensed under a [Creative Commons Attribution-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0/deed.en_US). This means that you are able to copy, share and modify the work, as long as the result is distributed under the same license.**

-----------------------

# CBW HT-seq Integrative Assignment

 
Written originaly by Mathieu Bourgey, edited by Florence Cavalli


### Task
We will perform the same analysis as in Module 2 but using the mother and father samples i.e sample NA12891 and NA12891.

```bash
Files are in the following directory of the cloud instance: ~/CourseData/HT_data/Module3/

 * raw_reads/NA12891_CBW_chr1_R1.fastq.gz
 * raw_reads/NA12891_CBW_chr1_R2.fastq.gz
 * raw_reads/NA12892_CBW_chr1_R1.fastq.gz
 * raw_reads/NA12892_CBW_chr1_R2.fastq.gz
```


### Environment setup

```
#set up
export SOFT_DIR=/usr/local/
export WORK_DIR=~/workspace/HTseq/Integrative_Assignment/
export TRIMMOMATIC_JAR=$SOFT_DIR/Trimmomatic-0.36/trimmomatic-0.36.jar
export PICARD_JAR=$SOFT_DIR/picard/picard.jar
export GATK_JAR=$SOFT_DIR/GATK/GenomeAnalysisTK.jar
export BVATOOLS_JAR=$SOFT_DIR/bvatools/bvatools-1.6-full.jar
export REF=$WORK_DIR/reference/


rm -rf $WORK_DIR
mkdir -p $WORK_DIR
cd $WORK_DIR
ln -s ~/CourseData/HT_data/Module3/* .

```
Task list:

1. Check read QC

2. Trim unreliable bases from the read ends

3. Align the reads to the reference

4. Sort the alignments by chromosome position

5. Realign short indels

6. Fixe mate issues (optional)

7. Recalibrate the Base Quality

8. Generate alignment metrics


Discussion/Questions:

1. Explain the purpose of each step

2. Which software tool can be used for each step 

The full commands can be downloaded here [solution] (https://bioinformatics-ca.github.io/images/commands_parents.sh)




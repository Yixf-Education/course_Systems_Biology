# 测序数据的质量控制与预处理 

## 实验目的
1. 掌握测序数据的FASTQ格式。
2. 熟悉FastQC等质量控制工具的使用方法。
3. 熟悉FASTX-Toolkit等质量控制工具的使用方法。
4. 熟悉Galaxy的使用方法。
5. 了解FastQC输出结果的含义。

## 实验材料
1. [sample.fastq](https://github.com/bioinformatics-core-shared-training/cruk-bioinf-sschool/blob/gh-pages/Day1/qa/sample.fastq)
2. [sample2.fastq](https://github.com/bioinformatics-core-shared-training/cruk-bioinf-sschool/blob/gh-pages/Day1/qa/sample2.fastq)

## 实验工具
1. [Galaxy](https://usegalaxy.org/)
2. [FastQC](http://www.bioinformatics.babraham.ac.uk/projects/fastqc/)
3. [FASTX-Toolkit](http://hannonlab.cshl.edu/fastx_toolkit/)

## 实验步骤

## 参考资料
* [FastQC Help](http://www.bioinformatics.bbsrc.ac.uk/projects/fastqc/Help/)
* [fastqc_sweave.pdf](https://github.com/bioinformatics-core-shared-training/cruk-bioinf-sschool/blob/gh-pages/Day1/fastqc_sweave.pdf)
* [QC results](https://github.com/bioinformatics-core-shared-training/cruk-bioinf-sschool/tree/gh-pages/Day1/qa/results)




---

## SNP-Seq pipeline

1. Upload data
2. Convert Fastq file to sanger sequences
3. FASTQ Summary Statistics
4. FASTQ Quality control
5. Quality filter
6. Alignment with BWA
7. SAM to BAM format conversion
8. Variants calling with Mpileup
9. Bcftools view
10. Extract workflow from history

1. FastQC
2. Mapping with	BWA
3. Quality Assessment/Quality Control
4. GATK	Phase 1: Data Pre-­‐processing	
5. INDEL Realignment
6. Base	Quality	Recalibration
7. GATK	Phase 2: Variant Discovery	
8. GATK	Phase 3: Preliminary Analysis
9. Variant Recalibration
10. Variant Annotation




## Exome-Seq Analysis
1. Quality Control
2. Alignment (BWA)
3. Mark PCR Duplicates
4. Local Realignments Around Indels
5. Quality Recalibration
6. SNP calling
7. Annotation

Indels within reads often lead to false positive SNPs at the end of sequence reads.
To prevent this artifact, “local realignment around indels” is done using local re-
alignment tools from the Genome Analysis Tool Kit, set as Galaxy tools.


## RNASeq Analysis
1. Upload Data
2. Fastq Groomer
3. Alignment with TopHat
4. Find Significant Changes
5. Find Significant Changes

1. Mapping with Tophat	
2. Computing differential expression with cuffdiff	
3. Cuffdiff visuaalization with CummeRbund

## ChIP-seq analysis
1. Data upload
2. Map with bowtie
3. Identify peaks bound with MACS
4. Find genes that overlap or are close to the peaks

1. Quality Control
2. Mapping
3. Peak-calling
4. Assign peaks to genes
5. Between Cell line comparison


The RNA-seq pipeline “Tuxedo” consists of the TopHat spliced read mapper, that internally uses  Bowtie or Bowtie 2 short read aligners, and several Cufflinks tools that allows one to assemble transcripts, estimate their abundances, and tests for differential expression and regulation in RNA-Seq samples.








[TOC]

---

# Coming of age: ten years of next-generation sequencing technologies
**Sara Goodwin,	John D. McPherson	& W. Richard McCombie**
*Nature Reviews Genetics 17, 333–351 (2016), doi:10.1038/nrg.2016.49, Published online 17 May 2016*

标签（空格分隔）： NGS review paper

---

# Abstract
Since the completion of the human genome project in 2003, extraordinary progress has been made in genome sequencing technologies, which has led to a decreased cost per megabase and an increase in the number and diversity of sequenced genomes. An astonishing complexity of genome architecture has been revealed, bringing these sequencing technologies to even greater advancements. Some approaches maximize the number of bases sequenced in the least amount of time, generating a wealth of data that can be used to understand increasingly complex phenotypes. Alternatively, other approaches now aim to sequence longer contiguous pieces of DNA, which are essential for resolving structurally complex regions. These and other strategies are providing researchers and clinicians a variety of tools to probe genomes in greater depth, leading to an enhanced understanding of how genome sequence variants underlie phenotype and disease.

# Subject terms
 - DNA sequencing
 - Genome
 - Genomics
 - Next-generation sequencing

---

# Introduction
Starting with the discovery of the structure of DNA, great strides have been made in understanding the complexity and diversity of genomes in health and disease. A multitude of innovations in reagents and instrumentation supported the initiation of the Human Genome Project. Its completion revealed the need for greater and more advanced technologies and data sets to answer the complex biological questions that arose; however, limited throughput and the high costs of sequencing remained major barriers. The release of the first truly high-throughput sequencing platform in the mid-2000s heralded a 50,000-fold drop in the cost of human genome sequencing since the Human Genome Project and led to the moniker: next-generation sequencing (NGS). Over the past decade, NGS technologies have continued to evolve — increasing capacity by a factor of 100–1,000 — and have incorporated revolutionary innovations to tackle the complexities of genomes. These advances are providing read lengths as long as some entire genomes, they have brought the cost of sequencing a human genome down to around US$1,000 (as reported by Veritas Genomics)5, and they have enabled the use of sequencing as a clinical tool.

Although exciting, these advancements are not without limitations. As new technologies emerge, existing problems are exacerbated or new problems arise. NGS platforms provide vast quantities of data, but the associated error rates (~0.1–15%) are higher and the read lengths generally shorter (35–700 bp for short-read approaches) than those of traditional Sanger sequencing platforms, requiring careful examination of the results, particularly for variant discovery and clinical applications. Although long-read sequencing overcomes the length limitation of other NGS approaches, it remains considerably more expensive and has lower throughput than other platforms, limiting the widespread adoption of this technology in favour of less-expensive approaches. Finally, NGS is also competing with alternative technologies that can carry out similar tasks, often at lower cost (Box 1); it is not clear how these disparate approaches to genomics, medicine and research will interact in the years to come.

This Review evaluates various approaches used in NGS and how recent advancements in the field are changing the way genetic research is carried out. Details of each approach along with its benefits and drawbacks are discussed. Finally, various emerging applications within this field and its exciting future are explored.
 
##　Box 1: Alternative genomic strategies
There are other technologies that either compete with or complement next-generation sequencing (NGS). This section outlines these technologies and their relationship with NGS.

### DNA microarrays
DNA microarrays have been used for genetic research since the early 1980s122 (see the figure, part a). In DNA microarrays, single-stranded DNA (ssDNA) probes are immobilized on a substrate in a discrete location with spots as small as 50 μm123. Target DNA is labelled with a fluorophore and hybridized to the array. The intensity of the signal is used to determine the number of bound molecules.
Microarrays are used in many applications. Single-nucleotide polymorphism (SNP) arrays identify common polymorphisms associated with disease and phenotypes, including cardiovascular disease124, cancer125, 126, 127, pathogens128, 129, ethnicity130, 131 and genome-wide association study (GWAS) analysis132, 133. Additionally, lower-resolution arrays are used to identify structural variation, copy number variants (CNVs) and DNA–protein interactions134, 135, 136, 137. Expression arrays measure expression levels by measuring the amount of gene-specific cDNA138.

Microarrays remain widely used in genomic research. They are used to identify SNPs at costs far below NGS routines. This is also true for expression studies, in which arrays inexpensively measure expression levels of thousands of genes. Variations in hybridization and normalization are problematic, leading some people to recommend RNA sequencing (RNA-seq) over gene expression microarrays139.

### NanoString
Similar to microarrays, the nCounter Analysis System from NanoString relies on target–probe hybridization (see the figure, part b). Probes target a gene of interest; one probe is bound to a fluorophore 'barcode' and the other anchors the target for imaging. The number and type of each barcode is counted. NanoString is unique in that the probes are labelled molecules that are bound together in a discrete order, which can be changed to create hundreds of different labels.

nCounter applications are similar to those of microarrays and quantitative PCR (qPCR; see below), including gene expression analysis145, 146, CNV and SNP detection147, 148, and fusion gene detection149. This approach provides exceptionally high resolution, less than one copy per cell145, far below microarrays and approaching TaqMan in sensitivity. Unlike most NGS applications, neither template enrichment nor reverse transcription are required. Around 800 targets can be read at a time, far below either microarrays or NGS.

### qPCR
Real-time qPCR utilizes the PCR reaction to detect targets of interest (see the figure, part c). Gene-specific primers are used and the target is detected either by the incorporation of a double-stranded DNA (dsDNA)-specific dye or by the release of a TaqMan FRET (fluorescence resonance energy transfer) probe through polymerase 5′−3′ exonuclease activity.

Developed in the early 1990s140, qPCR is widely used in both clinical and research settings for genotyping141, gene expression analysis142, CNV assays143 and pathogen detection144. qPCR is extremely rapid and robust, which is beneficial for point-of-care applications. Its high sensitivity and specificity make it the gold standard for clinical gene detection with several US Food and Drug Administration (FDA)-approved tests. The number of simultaneous targets that can be detected is in the hundreds rather than the thousands for microarrays and NGS. This method also requires primers and/or probes designed for specific targets.

### Optical mapping
Optical mapping combines long-read technology with low-resolution sequencing (see the figure, part d). Originally a method for ordering restriction enzyme sites150 through digestion and size separation, this technology now uses fluorescent markers to tag particular sequences within DNA fragments that are up to ~1 Mb long. The results are imaged and aligned to each other, and/or a reference, to map the locations of the probes relative to each other.

A central application of this technology is the generation of genome maps that are used in de novo assembly and gap filling94, 151. This technology can be used to detect structural variations that are up to tens of kilobases in length94, 152. Haplotype blocks that are several hundred kilobases in size can also be resolved153.

Optical mapping can either be an alternative to NGS or a complementary approach. As an alternative, it provides a low-cost option for understanding structural and copy number variation, but it does not provide base-level resolution. As a complementary technology, optical mapping improves de novo genome assemblies by providing a long-range scaffold on which to align short-read data.

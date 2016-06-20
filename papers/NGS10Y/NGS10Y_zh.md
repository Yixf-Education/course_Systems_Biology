
[TOC]

---

# 高通量测序（NGS）的这10年
**Sara Goodwin,	John D. McPherson	& W. Richard McCombie**
*Nature Reviews Genetics 17, 333–351 (2016), doi:10.1038/nrg.2016.49, Published online 17 May 2016*

标签： 高通量测序 综述　文献

---

# 简介
美国冷泉港实验室联合加州大学戴维斯分校的研究人员在国际著名评论型综述杂志Nature Reviews Genetics（影响因子41）上发表了一篇评论型综述。该综述对高通量测序的技术原理以及各平台的优势比较和实践应用进行了深入浅出的分析。

# 摘要
随着人类基因组计划（human genome project ）在2003年顺利完成，基因组测序技术取得了长足的进步，这直接导致了每兆基因组成本的大幅下降以及检测的基因组数量越来越多。人们对基因组的复杂性深感震惊，这也引导着测序技术的进一步发展。最近的一些突破性技术使得测序技术在更短的时间内可以获得更多的数据量。与之对应的是，还有一些技术的进步使得单条序列的测序读长变得更长——这对解析结构性的复合区段是极其必要的。这些进展给科研人员以及医疗诊断人员提供了一个绝佳的平台使得人们对基因组变异导致的表型变化以及疾病发生有了进一步的了解。

# 主题词
- DNA测序
- 基因组
- 基因组学
- 高通量测序

---

# 介绍
自从DNA的双螺旋结构被人们解析开始，人们在探究健康与疾病的基因组的复杂性与差异性上做出了巨大的努力。为了支持人类基因组计划的顺利进行，人们在仪器和试剂上做出了巨大的改进。该计划的完成使得人们强烈的意识到人们需要更多更好的技术与数据分析能力来回答随之而来的一系列生物学问题。然而，通量的限制以及居高不下的测序成本成为了人们进一步了解基因组的一道坎。2000年之后推出的高通量测序平台很好地解决了这个问题，人类基因组测序的成本直接因此下降50000倍，并且由此产生了一个新的名词：下一代测序（next-generation sequencing，NGS）。在过去的十年中，NGS技术不停的在进步——测序的数据量增加了100-1000倍。这些技术上的进展使得人们甚至可以在一条read上读出整条基因组序列。根据Veritas Genomics的数据，人类基因组测序的成本也已经下降到1000美元/人。不仅如此，该技术已经广泛在临床诊断上得到应用。

但是，尽管NGS技术非常重要，却并非完美。与NGS技术一道出现的是该技术带来的一系列问题。NGS可以提供海量的数据量，但是其质量却有待提高（有报道，NGS在序列拼接过程中，错误率在0.1-15%范围内），并且NGS的序列读长普遍较低（每条read的长度在35-700bp之内，这比普通的Sanger测序要短），这意味着需要更严格复杂的序列拼接。尽管长读长测序可以克服NGS的这一大弱点，但相对而言，成本较高并且通量较低，这也限制了该技术的进一步应用。最后，NGS同时还和其他的技术之间存在着竞争的关系，这些技术普遍成本偏低（Box 1）。在接下来的几年中，这些不同的技术在基因组学、医学和科学研究中将何去何从还是个未知数。

This Review evaluates various approaches used in NGS and how recent advancements in the field are changing the way genetic research is carried out. Details of each approach along with its benefits and drawbacks are discussed. Finally, various emerging applications within this field and its exciting future are explored.
 
 ---
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

![Alternative genomic strategies](http://static.zybuluo.com/yixf/2wqwl2b9ql4lk2krisb9oc3l/box1.jpg)
---

# 短读长（read）的NGS测序
## 测序模版克隆法生成综述
短读长测序方法包含两种：边连接边测序（sequencing by ligation, SBL）以及边合成边测序（sequencing by synthesis, SBS）。在SBL方法中，带有荧光基团的探针与DNA片段杂交并且与临近的寡核糖核酸连接从而得以成像。人们通过荧光基团的发射波长来判断碱基或者其互补碱基的序列。SBS方法通常使用聚合酶，诸如荧光基团或者离子浓度变化的信号，暗示着一个核苷酸在链的延伸过程中被插入其中。绝大多数的SBL和SBS方法，DNA都是在一个固体的表面上被克隆。一个特定区域内成千上万个拷贝的DNA分子可以增加信号和背景信号的区分度。大量的平行同样对上百万的reads的读取大有帮助，每个平行只有唯一的DNA模板。一个测序平台可以同时从上百万的类似反应中读取数据，因此可以同时对上百万的DNA分子进行测序。

产生模板的克隆有几个方法：基于磁珠（bead-based），固相介质（solid-state）以及DNA微球技术（DNA nanoball）（图1）。DNA模板产生的第一步就是样本DNA的片段化，接着是连接到一个为了克隆和测序而设计的接头上。在磁珠法的准备过程中，一个接头和寡核糖核酸片段互补并且固定在珠子上（图1a）。DNA模板通过使用油包水PCR（emulsion PCR，emPCR）得以扩增。单个珠子上被克隆得到的DNA片段可以达到上百万个。这些珠子可以被分为glass surface或者PicoTiterPlate（罗氏诊断）。固相介质扩增避免了油包水PCR，取而代之的是在固相介质上直接进行PCR（图1b,c）。该方法中，正向和反向引物结合在芯片的表面，这些引物给单链DNA（single-stranded DNA，ssDNA）提供了末端的互补序列供其结合。对模板浓度进行精确控制，可以使模板的扩增形成区域化且没有重叠的克隆簇，从而维持空间上的完整性。最近，几个NGS的平台都是用了模块化的flow cells。 By defining precisely where primers are bound to the slide, more DNA templates can be spatially resolved, enabling higher densities of reaction centre clusters and increasing sequencing throughput.

BGI使用的Complete Genomics technology测序技术是唯一一个在溶液中完成模板富集的技术。在这种情况下，DNA被多次连接，成环以及剪切，从而产生一个包含4个不同接头的环状的模板。通过旋转环状扩增（rolling circle amplification，RCA），可以最多产生超过200亿的DNA微球（图1d）。微球混合物随后被分配到芯片表面上，使得每个微球可以占据芯片的一个位点。

---

![Template amplification strategies](http://static.zybuluo.com/yixf/bupsi5yhfk7xy1xnf8qumaqx/fig1.jpg)
**Figure 1: Template amplification strategies.**
a. In emulsion PCR, fragmented DNA templates are ligated to adapter sequences and are captured in an aqueous droplet (micelle) along with a bead covered with complementary adapters, deoxynucleotides (dNTPs), primers and DNA polymerase. PCR is carried out within the micelle, covering each bead with thousands of copies of the same DNA sequence.
b. In solid-phase bridge amplification, fragmented DNA is ligated to adapter sequences and bound to a primer immobilized on a solid support, such as a patterned flow cell. The free end can interact with other nearby primers, forming a bridge structure. PCR is used to create a second strand from the immobilized primers, and unbound DNA is removed.
c. In solid-phase template walking154, fragmented DNA is ligated to adapters and bound to a complementary primer attached to a solid support. PCR is used to generate a second strand. The now double-stranded template is partially denatured, allowing the free end of the original template to drift and bind to another nearby primer sequence. Reverse primers are used to initiate strand displacement to generate additional free templates, each of which can bind to a new primer.
d. In DNA nanoball generation, DNA is fragmented and ligated to the first of four adapter sequences. The template is amplified, circularized and cleaved with a type II endonuclease. A second set of adapters is added, followed by amplification, circularization and cleavage. This process is repeated for the remaining two adapters. The final product is a circular template with four adapters, each separated by a template sequence. Library molecules undergo a rolling circle amplification step, generating a large mass of concatamers called DNA nanoballs, which are then deposited on a flow cell. 

Parts a and b are adapted from Ref. 18, Nature Publishing Group.

---

## 边连接边测序（SOLiD和Complete Genomics）
从根本上来说，SBL法包含了杂交和对标记的探针的连接。探针包含了一到两个特定碱基序列和一系列通用序列，这可以使得探针与模板之间进行互补配对。锚定的片段则包含一段已知的和接头互补的序列用于提供连接位点。连接之后，模板被系统进行测序反应。在锚和探针复合物或者荧光基团被完全移除之后，也或者连接位点重新生成之后，新的循环又重新开始了。

SOLiD平台使用的是双碱基编码的探针，每个荧光基团信号代表了一个二核糖核酸。因此，原始输出的数据并非直接和已知的核糖核酸相关联。因为16种可能的二核糖核酸组合并不能单独结合荧光基团。每四种组合使用一种荧光信号，共有四种荧光信号。所以，每种连接信号代表了几种可能的二核糖核酸组合，leading to the term colour-space (rather than base-space), which must be deconvoluted during data analysis。SOLiD测序过程由一系列的探针-锚的结合，连接，图像获取以及切割的循环组成（图2a）。Over the course of the cycles, single-nucleotide offsets are introduced to ensure every base in the template strand is sequenced.

Complete Genomics使用探针-锚的连接方式（cPAL）或者探针-锚的合成方式（cPAS）来进行测序。在cPAL中（图2b），锚的序列（与四种接头序列其中之一的互补）以及探针杂交到DNA微球的不同位置。每个循环中，杂交探针是一组特定位置已知碱基序列的探针的一员。每个探针包含一段已知序列的碱基以及对应的荧光基团。获取图像之后，全部的探针-锚复合物被移除，新的探针-锚复合物被杂交。Each subsequent cycle utilizes a probe set with the known base in the n + 1 position. Further cycles in the process also use adaptors of variable lengths and chemistries, allowing sequencing to occur upstream and downstream of the adaptor sequence.cPAS方法是cPAL的修改版，增加了read的长度；然而，目前来说，该方法的细节还相当匮乏。

---

![Sequencing by ligation methods](http://static.zybuluo.com/yixf/v5yzbi2rtgf5xe1246jssvee/fig2.jpg)
**Figure 2: Sequencing by ligation methods.**
a. SOLiD sequencing. Following cluster generation or bead deposition onto a slide, fragments are sequenced by ligation, in which a fluorophore-labelled two-base-encoded probe, which is composed of known nucleotides in the first and second positions (dark blue), followed by degenerate or universal bases (pink), is added to the DNA library. The two-base probe is ligated onto an anchor (light purple) that is complementary to an adapter (red), and the slide is imaged to identify the first two bases in each fragment. Unextended strands are capped by unlabelled probes or phosphatase to maintain cycle synchronization. Finally, the terminal degenerate bases and the fluorophore are cleaved off the probe, leaving a 5 bp extended fragment. The process is repeated ten times until two out of every five bases are identified. At this point, the entire strand is reset by removing all of the ligated probes and the process of probe binding, ligation, imaging and cleavage is repeated four times, each with an n + 1, n + 2, n + 3 or n + 4 offset anchor.
b. Complete Genomics. DNA is sequenced using the combinatorial probe–anchor ligation (cPAL) approach. After DNA nanoball deposition, an anchor complementary to one of four adapter sequences and a fluorophore-labelled probe are bound to each nanoball. The probe is degenerate at all but the first position. The anchor and probe are then ligated into position and imaged to identify the first base on either the 3′ or the 5′ side of the anchor. Next, the probe–anchor complex is removed and the process begins again with the same anchor but a different probe with the known base at the n + 1 position. This is repeated until five bases from the 3′ end of the anchor and five bases from the 5′ end of the anchor are identified. Another round of hybridization occurs, this time using anchors with a five-base offset identifying an additional five bases on either side of the anchor. Finally, this whole process is repeated for each of the remaining three adapter sequences in the nanoball, generating 100 bp paired-end reads.

---

## 边合成边测序（Sequencing-by-synthesis）
SBS的方法是指那些依赖于大量的DNA聚合酶来进行测序的方法。但是，SBS中依然包括了各种不同的测序原理。本文中，SBS方法被分为循环可逆终止（Cyclic reversible termination, CRT）以及单核糖核酸增加（single-nucleotide addition, SNA）。

### 边合成边测序：CRT（Illumina，Qiagen）
CRT方法是根据类似于Sanger测序的终止反应来界定的，其3'-OH基团被屏蔽而被阻止继续延伸。在反应开始时，DNA模板被一段和探针序列互补的接头结合，DNA聚合酶也是从这段序列开始结合。每个循环过程中，四种单独标记的复合物和3'屏蔽的脱氧核糖核酸被添加进反应中。在延伸过程中每结合一个dNTP，其他没有被结合的dNTPs被移除，并且获取图像来确定是哪个碱基在某个簇中被结合。荧光基团以及屏蔽基团随后被移除并且开始一轮新的反应。

Illumina的CRT（图3a）和其他平台相比，代表了最大的测序平台市场。Illumina短读长测序的设备可以从台式的低通量单位到大型的超高通量，如应用于全基因组测序（whole-genome sequencing，WGS）。dNTPs是通过两个或者四个激光通道来对荧光进行分析的。在绝大多数Illumina平台上，每种dNTP结合一种荧光基团，因此需要四种不同的激光通道。而NextSeq和Mini-Seq则使用的是双荧光基团系统。

2012年，Qiagen获得了Intelligent BioSystems CRT平台，并且在2015年将该平台命名为GeneReader重新推出并且使之商业化（图3b）。与其他平台不同的是，该平台打算做一站式的NGS平台，从样本制备到数据分析，全部一站式解决。为此，GeneReader系统整合了QIAcube样本制备系统和Qiagen Clinical Insight平台用于不同的数据分析。GeneReader平台的技术原理与Illumina平台基本一致。然而，该平台并非让每个DNA模板都去结合带有荧光基团的dNTPs，而是只要足够的dNTPs结合到模板上就可以完成鉴定。

---
![Sequencing by synthesis: cyclic reversible termination approaches](http://static.zybuluo.com/yixf/ff5ne1oeso620pklehl63bbo/fig3.jpg)
**Figure 3: Sequencing by synthesis: cyclic reversible termination approaches.**
a. Illumina. After solid-phase template enrichment, a mixture of primers, DNA polymerase and modified nucleotides are added to the flow cell. Each nucleotide is blocked by a 3′-O-azidomethyl group and is labelled with a base-specific, cleavable fluorophore (F). During each cycle, fragments in each cluster will incorporate just one nucleotide as the blocked 3′ group prevents additional incorporations. After base incorporation, unincorporated bases are washed away and the slide is imaged by total internal reflection fluorescence (TIRF) microscopy using either two or four laser channels; the colour (or the lack or mixing of colours in the two-channel system used by NextSeq) identifies which base was incorporated in each cluster. The dye is then cleaved and the 3′-OH is regenerated with the reducing agent tris(2-carboxyethyl)phosphine (TCEP). The cycle of nucleotide addition, elongation and cleavage can then begin again.
b. Qiagen. After bead-based template enrichment, a mixture of primers, DNA polymerase and modified nucleotides are added to the flow cell. Each nucleotide is blocked by a 3′-O-allyl group and some of the bases are labelled with a base-specific, cleavable fluorophore. After base incorporation, unincorporated bases are washed away and the slide is imaged by TIRF using four laser channels. The dye is then cleaved and the 3′-OH is regenerated with the reducing agent mixture of palladium and P(PhSO3Na)3 (TPPTS).

---

### 边合成边测序：SNA（454，Ion Torrent）
与CRT不同的是，SNA方法依赖于单信号标记dNTP来对链进行延伸。四种核糖核酸都必须反复添加到测序反应过程中。不仅如此，SNA不需要将dNTP屏蔽，因为测序反应过程中下一个碱基的缺失会阻止链的延伸。碱基的寡聚体则是一个例外，在这种情况下，信号的强度会随着dNTP数量的增加而成比例的增强。

第一个NGS仪器是454焦磷酸测序仪。这种SNA系统将结合有模板的珠子以及酶混合物分配到PicoTiterPlate中。由于一个dNTP只能结合到一条链上，酶复合物会对其产生生物荧光。一个特定的珠子中的一个或多个dNTPs可以通过电荷共轭偶联设备（charge-coupled device, CCD）检测到的荧光来确认（图4a）。

Ion Torrent是第一个没有光学感应的NGS平台。与酶化学复合物产生的信号相比，Ion Torrent平台检测的是dNTP中释放出来的H+离子。pH值的改变通过integrated complementary metal-oxide-semiconductor （CMOS）以及ion-sensitive field-effect transistor （ISFET）来检测（图4b）。传感器对pH的变化对于连续碱基的检测还不够完善，因此在测量同一碱基连续出现时的数量可能会有所误差。

---
![Sequencing by synthesis: single-nucleotide addition approaches](http://static.zybuluo.com/yixf/k8t0npxvw7in652zpr45uap7/fig4.jpg)
**Figure 4: Sequencing by synthesis: single-nucleotide addition approaches.**
a. 454 pyrosequencing. After bead-based template enrichment, the beads are arrayed onto a microtitre plate along with primers and different beads that contain an enzyme cocktail. During the first cycle, a single nucleotide species is added to the plate and each complementary base is incorporated into a newly synthesized strand by a DNA polymerase. The by-product of this reaction is a pyrophosphate molecule (PPi). The PPi molecule, along with ATP sulfurylase, transforms adenosine 5′ phosphosulfate (APS) into ATP. ATP, in turn, is a cofactor for the conversion of luciferin to oxyluciferin by luciferase, for which the by-product is light. Finally, apyrase is used to degrade any unincorporated bases and the next base is added to the wells. Each burst of light, detected by a charge-coupled device (CCD) camera, can be attributed to the incorporation of one or more bases at a particular bead. 
b. Ion Torrent. After bead-based template enrichment, beads are carefully arrayed into a microtitre plate where one bead occupies a single reaction well. Nucleotide species are added to the wells one at a time and a standard elongation reaction is performed. As each base is incorporated, a single H+ ion is generated as a by-product. The H+ release results in a 0.02 unit change in pH, detected by an integrated complementary metal-oxide semiconductor (CMOS) and an ion-sensitive field-effect transistor (ISFET) device. After the introduction of a single nucleotide species, the unincorporated bases are washed away and the next is added.
Part a is adapted from Ref. 18, Nature Publishing Group.

---

## 短读长平台的比较
每个平台在通量，成本，错误率以及read结构上都大相径庭（表一）。尽管有多家NGS技术供应商，NGS研究最常用的还是Illumina平台。尽管该平台极为稳定，数据可靠，但是基于其使用的单一测序的方法，具有系统偏好性的问题。因此，新技术的发展使得研究人员能够有完整的测序方案来获得完整的序列信息。

---

![Summary of NGS platforms](http://static.zybuluo.com/yixf/e11xevqalc2ixqv8gr0rot9i/tab1.png)

---

SOLiD与Complete Genomics系统使用的SBL技术准确率非常高（~99.99%），因为每个碱基都会被标记多次。虽然这些技术非常准确，但是在敏感性与特异性之间依然不能达到完美的平衡，当一些错误的碱基变化出现时，真实的碱基变化可能被忽略。该类技术在应用上最大的限制可能就是其过短的读长。尽管所有的平台都能产生单末端和双末端的reads，SOLiD的最大读长只能达到75bp，Complete Genomics只能达到28-100bp，使得其在基因组拼接和结构变异研究中的可操作性大大降低。不幸的是，SOLiD系统不仅受制于运行时间，还受制于其工业生产。另外，尽管cPAL计划准备在成本和通量上和Illumina竞争，却在2016年被迫下马，该技术仅在人类WGS中有所应用。cPAS的BGISEQ-500系统则受制于中国大陆政府。

Illumina由于其技术成熟，平台之间高度互补性与交叉性，使得其在短读长测序上大占优势。Illumina的产品覆盖了从低通量的Mini-Seq到超高通量的HiSeq X系列，其中HiSeq X系列最多可以在一年内产生1800多个30×覆盖度的人类基因组数据量。此外，其运行时间，read结构以及read长度（最大300bp）都在不停的改进。但是，作为一个依赖于CRT技术的Illumina平台，相对于SNA平台的优势在于其在读取核糖核酸多聚体（同一种核糖核酸多次出现）时较低的错误率。尽管SNA平台总体上的准确率可以达到99.5%，但是在读取那些AT富集或者GC富集的片段的时候错误率还不能令人满意。在2008年，据Bentley等报道，Illumina平台鉴定到的人类单核糖核酸多态性（SNPs）与基因芯片鉴定的SNPs具有惊人的一致性。但是，这种高度的敏感性也随之带来了2.5%左右的错误率。因此，其他小组计划使用Sanger测序来对鉴定到的SNPs进行重新测序以便区分测序错误导致的SNPs与真实的基因突变导致的SNPs。在对所有的可能性都进行优化之后，Illumina平台被大量的研究人员认可，在大量的领域中均有涉及：WGS的基因组测序与外显子测序；遗传学应用如染色质免疫共沉淀测序（chromatin immunoprecipitation followed by sequencing）；ATAC-Seq（transposase-accessible chromatin using sequencing）或者DNA甲基化测序（Methyl-Seq）；RNA转录组测序（transcriptomics applications through RNA sequencing, RNA-seq）等等。NextSeq与MiniDeq平台使用的双色标记系统通过降低双色通道的扫描与荧光基团的使用实现成本的降低和测序速度的提升。然而，双通道系统却会略微增加测序的错误率。HiSeq X是目前最高通量的仪器，但其由于通量过大，因此只在部分应用上得以使用，如WGS与全基因组甲基化测序。不仅如此，HiSeq X更大的局限在于其高昂的成本，以至于超过了绝大多数单位的可接受程度。

Qiagen的GeneReader是专为临床诊断设计的，其主要关注点在肿瘤基因panels上，也因此其局限性较大。根据对其运行时间与功能的分析，GeneReader与Illumina的MiSeq较为相似。尽管还没有使用数据，但是GeneReader和MiSeq平台有相同的优缺点。

454平台和Ion Torrent平台相比于其他的短读长平台而言，能够提供较长的read读长，分别大约在700bp与400bp，因此在基因组结构较为复杂的研究上应用较多。然而，由于同样都是基于SNA技术，它们都拥有相同的缺点。虽然，其在非碱基多聚体（non-homopolymer）的测序上正确率与其它NGS平台相差无几，但其插入与缺失（Insertion and deletion，indel）是最大的问题。同一碱基的多聚体是该类技术最大的问题所在。有报道，对同一碱基的多聚体的测序误差能够达到6-8个碱基之多。不幸的是，尽管Ion Torrent依然在紧跟快速进化的NGS平台的步伐，454平台却由于成本与应用范围过于狭小已经被罗氏公司停产。

Ion Torrent平台为不同的研究人员的不同需求提供了不同的芯片与设备，通量从50Mb到15Gb不等，运行时间也从2小时到7小时不等。这一点使得其几乎是所有目前的二代测序平台中最快的一个。这也使得其在基因panel与精准临床诊断上大有优势，包括转录组与可变剪切鉴定。Ion Torrent先后发布Ion Personal Genome Machine （PGM） Dx与Ion S5系列，希望在临床诊断上打开疆土。与Ion Chef文库制备试剂盒和芯片上样设备结合使用，S5系列希望能够成为最方便操作的设备，消除其它Ion Torrent设备对氩的依赖。但是，其最大的缺点在于Ion PGM Dx系统可以进行双向测序，更高通量的Ion Proton与S5系统却并不支持双向测序，也因此限制了其在大范围基因组测序与转录组结构上的应用。

# 长读长（read）的NGS测序
## 综述
基因组是一个复杂的复合物，其中包含了多种重复序列，拷贝数变化，结构变异。这些与进化，适应以及疾病密切相关。然而，许多复合物元件由于过长，导致短读长测序并不能够完美的对其进行测序。长读长测序的reads可以达到几千个碱基，这使得可以对大的结构进行功能解析。此类的长读长测序产生的单一长序列可以跨越复合物或者重复序列。长读长测序在转录组测序过程中也大有益处，因为长读长的reads可以跨越完整的mRNA的转录本而不需要拼接。这可以使得研究人员可以鉴定到更多的基因亚型等。

最近，人们开发出了两种长读长测序的实验方案，分别是：单分子实时测序（single-molecule real-time sequencing）以及依赖于已有短读长技术体外构建长读长的合成法。单分子法与短读长测序完全不同，因为单分子法不需要对模板进行扩增来产生足够测序仪读取的信号，也不需要轮番添加dNTP。而合成法并非产生原始的长读长的reads，而是通过利用barcodes来进行拼接获得长片段。

## 单分子长读长测序（PacBio和ONT）
最近这段时间，最常用的长读长测序法平台就是使用PacBio Biosciences（PacBio）的单分子实时测序法（single-molecule real-time sequencing, SMRT）（图5a）。该设备使用了一个特制的流动单元，其中包含了成千上万的单独的底部透明的皮升孔（picolitre wells）——zero-mode waveguides（ZMW）。短读长SBS技术需要使得聚合酶结合DNA，沿着DNA进行扩增，而PacBio则固定聚合酶在孔的底部，让DNA链通过ZMW。由于聚合酶有固定的位置，因此该系统可以对单分子DNA进行测序。dNTP结合在每个孔的单分子模板上，通过激光或者成像设备记录ZMW底部标记在核糖核酸上的发射波长的颜色与持续时间来进行序列的读取。聚合酶在结合dNTPs的过程中，切割dNTP结合的荧光基团，使得荧光基团在第二个标记的碱基进入ZMW前将前一个荧光基团去除。SMRT平台也使用了独特的环状模板，这种方式的模板可以使得聚合酶反复读取模板的序列。尽管这种方法不太容易对长度大于3kb的片段反复读取，但是短的模板却可以反复读取多次。由于多次读取同一序列，因此系统会产生多次测序后的保守序列（consensus sequence, CCS）。

2014年，第一个消费级别的nanopore测序仪的原型机——MinION在Oxford Nanopore Technologies（ONT）诞生。与其他平台不同的是，nanopore测序仪并不监测模板DNA结合或杂交的核糖核酸。其它平台通过监测次级信号，光，颜色或pH等来进行碱基序列的读取，而nanopore则直接对天然的ssDNA分子进行读取。为达成此，DNA需要通过一个蛋白孔（protein pore）（图5b），孔也会因为DNA分子的通过导致的电压阻塞（voltage blockade）的发生。对这些电荷瞬时的追踪称为squiggle space，特定DNA序列通过孔会产生特定的电压改变，这被称为k-mer。相比于1-4种可能的信号，nanopore拥有1000多种可能的k-mer，尤其是当天然DNA序列中存在修饰的碱基的时候。最近的MK1 MinION流动单元由特殊应用的芯片组成，包涵了512个独立的通道，每秒可以读取70bp长度，到2016年预计能够增加到500bp/秒。新推出的PromethION设备是包含了48个独立流动单元的高通量平台。该项工作最多可以在2天内输出～2-4Tb的数据量，这使可能其成为HiSeq X系列的强力竞争者。与PacBio的环状模板类似的是，ONT MinION使用一个leader-harpin library结构。这使得正向DNA链可以通过孔，接着harpin蛋白结合双链，最后是反义链。这产生了1D和2D reads，1D链可以通过比对产生一个保守的2D read。

---
![Real-time and synthetic long-read sequencing approaches](http://static.zybuluo.com/yixf/rvrjx69g0pegci9xrq83wklu/fig5.jpg)
**Figure 5: Real-time and synthetic long-read sequencing approaches.**
A. Real-time long-read sequencing platforms.
Aa. Single-molecule real-time (SMRT) sequencing from Pacific Biosciences (PacBio). Template fragments are processed and ligated to hairpin adapters at each end, resulting in a circular DNA molecule with constant single-stranded DNA (ssDNA) regions at each end with the double-stranded DNA (dsDNA) template in the middle. The resulting 'SMRTbell' template undergoes a size-selection protocol in which fragments that are too large or too small are removed to ensure efficient sequencing. Primers and an efficient φ29 DNA polymerase are attached to the ssDNA regions of the SMRTbell. The prepared library is then added to the zero-mode waveguide (ZMW) SMRT cell, where sequencing can take place. To visualize sequencing, a mixture of labelled nucleotides is added; as the polymerase-bound DNA library sits in one of the wells in the SMRT cell, the polymerase incorporates a fluorophore-labelled nucleotide into an elongating DNA strand. During incorporation, the nucleotide momentarily pauses through the activity of the polymerase at the bottom of the ZMW, which is being monitored by a camera.
Ab. Oxford Nanopore Technologies (ONT). DNA is initially fragmented to 8–10 kb. Two different adapters, a leader and a hairpin, are ligated to either end of the fragmented dsDNA. Currently, there is no method to direct the adapters to a particular end of the DNA molecule, so there are three possible library conformations: leader–leader, leader–hairpin and hairpin–hairpin. The leader adapter is a double-stranded adapter containing a sequence required to direct the DNA into the pore and a tether sequence to help direct the DNA to the membrane surface. Without this leader adapter, there is minimal interaction of the DNA with the pore, which prevents any hairpin–hairpin fragments from being sequenced. The ideal library conformation is the leader–hairpin. In this conformation the leader sequence directs the DNA fragment to the pore with current passing through. As the DNA translocates through the pore, a characteristic shift in voltage through the pore is observed. Various parameters, including the magnitude and duration of the shift, are recorded and can be interpreted as a particular k-mer sequence. As the next base passes into the pore, a new k-mer modulates the voltage and is identified. At the hairpin, the DNA continues to be translocated through the pore adapter and onto the complement strand. This allows the forward and reverse strands to be used to create a consensus sequence called a '2D' read.
B. Synthetic long-read sequencing platforms.
Ba. Illumina. Genomic DNA templates are fragmented to 8–10 kb pieces. They are then partitioned into a microtitre plate such that there are around 3,000 templates in a single well. Within the plate, each fragment is sheared to around 350 bp and barcoded with a single barcode per well. The DNA can then be pooled and sent through standard short-read pipelines.
Bb. 10X Genomics' emulsion-based sequencing. With as little as 1 ng of starting material, the GemCode can partition arbitrarily large DNA fragments, up to ~100 kb, into micelles (also called 'GEMs') along with gel beads containing adapter and barcode sequences. The GEMs typically contain ~0.3× copies of the genome and 1 unique barcode out of 750,000. Within each GEM, the gel bead dissolves and smaller fragments of DNA are amplified from the original large fragments, each with a barcode identifying the source GEM. After sequencing, the reads are aligned and linked together to form a series of anchored fragments across a span of ~50 kb. Unlike the Illumina system, this approach does not attempt to get full end-to-end coverage of a single DNA fragment. Instead, the reads from a single GEM are dispersed across the original DNA fragment and the cumulative coverage is derived from multiple GEMs with dispersed — but linked — reads.
Part Aa is adapted from Ref. 18, Nature Publishing Group. Part Ba is adapted from Ref. 62.

---

## 长reads的合成
与真正测序的平台不同的是，合成长读长技术依赖于一个barcode系统来结合不同的片段，通过已有的短读长测序仪来获得长读长reads。该方法将大的DNA分子分割成若干个小片段到微孔中或者乳液中。每个微孔或者乳液中的模板被切割并且加上了barcodes。这种方法允许在短读长测序仪上使用，测序后数据被通过barcode分开按照barcodes的序列进行拼接。

合成法有两个系统：Illumina长片段合成平台（图5c）与10X Genomics乳液系统（图5d）。Illumina系统（Moleculo）分割DNA到小板上而不需要特殊仪器。然而，10X Genomics乳液系统（GemCode与Chromium）使用乳液分隔DNA并且需要微流体平台（microfluidic instrument）来进行测序前的准备工作。在其实浓度低至1ng的情况下，10X Genomics乳液系统可以任意切割长的DNA片段（最大达到100kb）到微粒（GEM）中，这种微粒一般包含了≤0.3×的基因组以及一个独特的barcode。

## 单分子测序与合成法测序的比较
人们对长读长测序越来越感兴趣，每个系统都有其优劣（表一）。最近长读长测序最受欢迎的是PacBioRS II。该设备可以产生超过50kb长度的单个read，长链建库测序平均长度为10-15kb。这种特性使得在基因组拼接与大范围基因组结构的应用中大有好处。但是，长链的单个碱基错误率在15%左右，使得人们对该仪器的使用有所顾虑。不幸的是，这些错误随机分布在每个reads，也因此必须有足够高的覆盖度来消除单个碱基错误率的负面影响。PacBio的环状模板有时候也会出现错误。单个碱基测序次数越多，结果就越可靠，其最高准确率达到99.999%。其高准确率与Sanger测序相似，使得该方法与Sanger测序一道成为SNPs的研究方法。该设备的运行时间与通量受测序读长的影响，长的模板需要更长的时间。举例来说，1kb的库运行1小时测序每个分子可以产生7500个碱基，平均大约重复8次；而运行4小时每个分子可以产生大约30000个碱基（大约重复30次）。相反的是，10kb的库运行4小时产生30000个碱基只能重复3次左右。通量的限制以及高昂的成本（1000美元/G），加上较高的覆盖度使得PacBio RS II成为那些较小的实验室难以应用的技术。然而，考虑到这些问题，PacBio推出了Sequel系统，其通量与RS II相比高出了7倍，使得30×覆盖度的人类基因组测序成本大幅下降一半。

ONT MinION是一个小的（~3cm × 10cm）USB设备，并且可以在个人电脑上运行，使得其成为最小的测序平台。这使得MinION具有极高的便携性，并且在临床诊断中以及那些不容易到达的地方有着广泛的应用前景。尽管周边设备依然只有在实验室中才有，如文库准备的恒温器，这依然可以大幅减少设备空间。与其他平台不同，MinION在片段大小上是有限制的。理论上来讲，任意大小的DNA分子都可以在该设备上测序，但是实际情况是在对长片段进行测序过程中，是有所制约的。作为ONT技术本身的特性，ONT拥有超过1000种独立的信号，这使得ONT拥有巨大的错误率——1D read大约在30%左右（主要是indel）。有效的对核糖核酸复合物的测序也是ONT MinION面临的一大问题。当核糖核酸复合物超过k-mer长度，就很难准确鉴定前一个k-mer何时离开孔而下一个k-mer何时进入孔。因为修饰的碱基会改变原有的k-mer设定的电压变化，所以碱基的修饰对MinION而言同样也是一大挑战。幸运的是，最近的一系列的对试剂以及算法的改进使得其准确率提高不少。

The Illumina synthetic long-read approaches are a direct response to the costs, error rates and throughput of true long-read sequencers. Relying on the existing Illumina infrastructure affords researchers the ability to simply purchase a kit for long-read sequencing. Accordingly, the throughput and error profile are identical to those of current Illumina devices. However, as a consequence of how the DNA is partitioned, the system requires more coverage than is required for a typical short-read project, thus increasing the costs associated with this technology relative to other Illumina applications.

Like the Illumina synthetic long-read platform, the 10X Genomics emulsion-based platform relies on an existing short-read infrastructure to provide the sequencing. The microfluidic instrument is a one-time additional equipment cost, and the emulsion approach used allows for as little as 1 ng of starting material, which can be beneficial for situations in which the DNA is precious, such as biopsy samples. Currently, data output from the GemCode instrument is partially limited by the number of barcodes used and the somewhat inefficient DNA partitioning. Inefficient partitioning can lead to a surplus of DNA fragments within a droplet, thus complicating sequence deconvolution, which is further exacerbated by the limited number of barcodes. Both of these conditions lead to ambiguity regarding the positional relationship between reads sharing the same barcode, making analysis more difficult. To rectify this, 10X Genomics plans to release the Chromium System in mid-2016; this will be an upgrade from the GemCode device. Although the chemistry will remain fundamentally the same, the number of possible micelle partitions will increase from 100,000 to 1 million, and the number of barcodes will increase from 750,000 to ~4 million.

# 应用
WGS正在成为NGS中最广泛的应用。通过该技术并且结合生物学应用，研究人员可以获得基因组信息中最值得注意的信息。举例来说，2012年，Ellis等报道了基因与乳腺癌患者芳香酶抑制剂（aromatase inhibitor）治疗法之间的关联。他们指出突变，后果与诊断之间的关联，同样还有癌症相关基因的突变的富集。这提供了一个可能性，即：乳腺癌有不同的突变造成不同的表型，具有复杂的病理学。最近的NGS平台的改进使得研究人员发现了一些几年前难以想象的新观点与机会。在2010年，千人基因组计划（1000 genomes project）开放了其从179个个体中获得的WGS原始数据以及697个个体的测序数据。到2015年，研究人员已经构建了26个不同人群的2504个人的基因组群体。给人们从种群的角度来观察人类的变异。但这还不是该项目的终点，越来越多的人的基因组正在被得以测序。种群水平的测序已经成为人们更好的理解人类疾病的一个重要的工具，同样也得到了意想不到的结果。一个例子是，Sidore等对2120个撒丁岛人（Sardinians）的WGS研究发现了一些新的和脂肪相关的基因以及炎症的标志物，给人们对血液胆固醇的分子机制的研究提供了新思路。

全外显子组测序和靶向测序（Whole-exome and targeted sequencing）同样也广泛应用于测序的研究中。通过限制使用的基因组材料的大小，更多的个人样本可以在一个测序中实现，增加了基因组研究的宽度以及深度。使用外显子测序，Iossifov等对超过2500个单一的家庭进行测序，每个家庭都有一个小孩患有自闭症（autism spectrum disorder, ASD）。研究人员在30%的样本中发现了错义突变（missense mutations），基因干扰的突变（gene-disrupting mutations）以及拷贝数的变异。该工作与其他的工作一道鉴定到了ASD相关的基因突变。其他证据表明，高覆盖度的WGS也可以解决复杂的变异以及临床样本的分析。2015年，Griffith等认为可以使用一个完美的跨平台的方法（包含靶向测序）来鉴定肿瘤中高可信度的SNPs。该方法中，作者认为10000×的覆盖度可以鉴定到稀有突变。由于10000×的覆盖度对于WGS而言实在过高，靶向测序便在临床中得到了广泛的应用。

NGS同样在基因的调控研究中有广泛的应用。蛋白-DNA互作可以通过染色质免疫共沉淀结合NGS测序（ChIP-seq）来得以研究。利用NGS对修饰碱基的研究也是可行的。举例来说，甲基化测序包含了甲基化DNA的捕获与富集，对甲基化与非甲基化区段的选择性消化。但是，尽管利用此方法获得了很多重大的发现，修饰与捕获过程成为其最大的限制。2010年，Flusberg等发表了一个概念性的研究方法，即：使用PacBio来区分甲基化与非甲基化的碱基。由于聚合酶即便是甲基化的碱基也能够延伸，但在甲基化位点上会停留更多的时间，因此这里改变的信号可以认为含有甲基化修饰。与之相同的是，nanopore平台也能够监测修饰的碱基，因为甲基化同样会影响鉴定到的电压的变化。这使得甲基化的测序可以在不需要化学操作的条件下进行。

一个最近的NGS的范例是对长链DNA的测序。重复序列以及复合序列长久以来较难以拼接，短读长测序很难解决这个问题。最近，Chaisson等对长读长测序的使用使得其能够在人类GRCh37数据库中提交超过1Mb的新的序列，这些序列弥补甚至跨越了曾经的沟。Chaisson等还鉴定到了大于26000个超过50bp的indels，也因此，GRCh37数据库成为最有参考价值的几个基因组之一。除了简单的增加基因组数据可靠性之外，长读长还能够提供更有效的临床诊断。

在对转录水平上的研究也因为NGS受益匪浅。今天，研究人员甚至能够使用NGS的深度测序对单个转录本进行研究。2014年，Treutlein等使用了组织发育过程中不同细胞类群的单细胞RNA测序发现了用于鉴定细胞亚群的标志物。尽管长读长测序相对而言在对转录本的定量上不占优势，但是，长读长可以在研究转录组的结构上有所帮助。举例来说，最近的人类长读长转录组测序研究表明>10%的reads是新的可变剪切体。

NGS最新的设备——nanopore测序仪，依然在寻找其定位的过程中。然而，研究人员正在将其快速的文库制备，实时的数据生产以及小的体积的优势转变为资本。最近，英国Stanley Royd Hospital的研究人员使用MinION用于监测沙门氏菌（Salmonella enterica）的爆发。MinION测序仪最令人振奋的应用可能就是2014年的埃博拉病毒爆发。在位于日内瓦的欧洲移动实验室的主持下，作者对埃博拉病毒的传播以及进化历史进行了深入的研究。

# 结尾
我们正处在新的NGS技术革命的顶端。NGS现在已经不仅仅只是一个新奇的事物，而已经成为了一个在生物学研究中广泛应用的技术。最新的超高通量测序仪已经将曾经认为不可能的事情变为可能。这包含了首创的精准医疗（medicine initiatives）以及Illumina计划的对循环肿瘤DNA（circulating tumour DNA, ctDNA）进行测序。每个计划都对数万个基因组样本进行测序。所以，快速以及低成本的测序给予了内科医生强大的工具来翻译基因组信息成为有用的临床诊断结果。

这个革命也带来了新的挑战。由于NGS旨在广泛的应用于临床，时间就成为一个NGS首先需要面对的挑战。对于那些严重的神经性疾病或者极为危险的癌症患者而言，数周的WGS分析的等待时间足以使患者错过最佳的治疗时间。对于急性感染而言，这些事件已经下降到几天。尽管人们已经对时间做出了巨大的改进，但是绝大多数现有的系统都不能完全满足快速模式下的足够产出。

虽然临床诊断面临着数据量不够的问题，NGS其他方面的应用却面临着生产力过剩的境地。目前，已有超过14000个基因组序列上传到美国的National Center for Biotechnology Information（NCBI）中。2013年，Schatz与Langmead报道了全世界每年可以生产超过15PB的数据量，并且数量与通量依然在继续增加。数据量的富裕对分析以及其下游提出了严峻的挑战，这需要革命性的存储与生信解决方案。将海量的数据量翻译成有生物学与遗传学内涵的结果同样也是一个挑战。在临床诊断方面，通过NGS分析的数据产生的假阳性或者假阴性同样也是需要慎重考虑的问题。

最近，Illumina由于NGS与其周边产品获得了巨大的成功。其它生产商也在快速革新自身的产品。Illumina的市场仍然在增长，以至于优势巨大。BGISEQ-500以及Helicos technology的GenoCare在亚洲也有所斩获。ONT PromethION与Illumina HiSeq X系列则向着成本与产量的极限大步迈进。随着人们对临床诊断测序兴趣的增加，已有的NGS供应商正在提供各种快速的解决方案，如Ion Torrent S5以及Illumina的MiniSeq，还有新加入者Qiagen的GeneReader也来参与竞争。

今后的几年里，更多的玩家也会带着心得解决方案进入这个市场。GenapSys (Sigma-Aldrich)的electronic ‘lunchbox’-sized sequencer; Genia (Roche)的新的nanopore测序方案; 以及单通道CMOS技术，都号称能够在临床应用上节约足够的时间。这些已有的和新的搅局者都有着科技革命的潜质，包括直接对RNA或者蛋白进行测序等，这些最近和未来的进步使得今天成为NGS发展的黄金时期。

# Glossary
* **Read**: The sequence of bases from a single molecule of DNA.
* **Sanger sequencing**: An approach in which dye-labelled normal deoxynucleotides (dNTPs) and dideoxy-modified dNTPs are mixed. A standard PCR reaction is carried out and, as elongation occurs, some strands incorporate a dideoxy-dNTP, thus terminating elongation. The strands are then separated on a gel and the terminal base label of each strand is identified by laser excitation and spectral emission analysis.
* **Template**: A DNA fragment to be sequenced. The DNA is typically ligated to one or more adapter sequences where DNA sequencing will be initiated.
* **Fragmentation**: The process of breaking large DNA fragments into smaller fragments. This can be achieved mechanically (by passing the DNA through a narrow passage), by sonication or enzymatically.
* **Clusters**: Groups of DNA templates in close spatial proximity, generated either though bead-based amplification or by solid-phase amplification. Bead-based approaches rely on emulsions to maintain template isolation during amplification. Solid-phase approaches rely on the template-to-bound-adapter ratio to probabilistically bind template molecules at a sufficient distance from each other.
* **Flow cells**: Disposable parts of a next-generation sequencing routine. Template DNA is immobilized within the flow cell where fluid reagents can be streamed into the cell and flushed away.
* **Rolling circle amplification**: (RCA). A method of DNA amplification using a circular template. Briefly, DNA polymerase binds to a primed section of a circular DNA template. As the polymerase traverses the template, a new strand is synthesized. When the polymerase completes a full circle and encounters the double-stranded DNA (dsDNA) template, it displaces the template without degradation, thus creating a long ssDNA fragment composed of many copies of the template sequence.
* **One-base-encoded probes**: Oligonucleotides that contain a single interrogation base in a known position. The base corresponds to a fluorescent label on each probe. The remaining bases are either degenerate (any of the four bases) or universal (unnatural bases with nonspecific hybridization), allowing the probe to interact with many different possible template sequences.
* **Two-base-encoded probes**: Oligonucleotides that contain two adjacent interrogation bases in a known position. The bases correspond to a fluorescent label on each probe. The remaining bases are either degenerate (any of the four bases) or universal (unnatural bases with nonspecific hybridization) allowing the probe to interact with many different possible
template sequences.
* **Colour-space**: A system exclusively used by SOLiD. When a two-base-encoded probe is used, the bound label corresponds to two bases rather than one. Thus, the signal derived from a SOLiD run is in a series of colours that represent overlapping dinucleotides, rather than each colour being directly correlated to a single base. A reference-based alignment is the most efficient way to translate colour-space into base-space. For example, in the sequence ATGT the first probe will match AT, the second will match TG and the third GT. If the AT is known, then the subsequent colour order is uniquely solved as TG and GT, leading to a readout of ATGT. Final
sequence deconvolution of colour-space is achieved with the knowledge of the second base identity in one round and the colour of the subsequent round in which the ligation is offset by one nucleotide, allowing for the identification of the next base.
* **Base-space**: A system used by most next-generation sequencing platforms. When a one-base-encoded probe or a sequencing-by‐synthesis
approach is used, each signal is correctly correlated to a base.
* **Two-fluorophore system**: A system in which bases are discriminated by labelling Cs and Ts with a red or green fluorophore, respectively. Each A base is labelled with either a red or green fluorophore, but the two populations are mixed. During base discrimination, clusters that are either red or green are called either C or T, whereas clusters with a red and green mixed signal are called A. The G base is unlabelled, thus any cluster without a fluorophore signal is called G.
* **Homopolymer**: A sequence run of identical bases.
* **Charge-coupled device**: (CCD). A device composed of an integrated circuit that forms light-sensitive elements: pixels. When a photon interacts
with the device, the light generates a charge that can be interpreted by an
electronic device.
* **Integrated complementary metal-oxide-semiconductor**: (CMOS). An integrated circuit design that is printed on a microchip that contains different types of semiconductor transistors to create a circuit that both uses very little power and is resistant to high levels of electronic noise.
* **Ion-sensitive field-effect transistor**: (ISFET). A type of transistor
that is sensitive to changes in ion concentration.
* **Single-end and paired-end sequencing**: In single-end sequencing, a DNA template is sequenced only in one direction. In paired-end sequencing, a DNA
template is sequenced from both sides; the forward andreverse reads may or may not overlap. A deviation in the expected genome alignment between two ends of a paired-end read can indicate astructural variation.
* **Structural variant**: A variation larger than single-nucleotide polymorphisms (SNPs). This can include the insertion or deletion of blocks of DNA, inversions or translocations of DNA segments, and copy-number differences.
* **ChIP–seq**: (Chromatin immunoprecipita-tion followed by sequencing). A method used to analyse protein interactions with DNA by combining ChIP with
massively parallel DNA sequencing to identify the binding sites of DNA-associated proteins.
* **ATAC–seq**: (Assay for transposase-access­ible chromatin with high-throughput sequencing). A method that uses the activity of a hyperactive transposase to cleave exposed DNA and add sequencing adapters. Regions that cannot be sequenced are inferred to be chromatin interacting.
* **RNA sequencing**: (RNA-seq). A method of sequencing cDNA derived from
RNA. This approach can be used to sequence both coding and non-coding RNA.
* **Real-time sequencing**: A sequencing strategy used in the Pacific Biosciences (PacBio) and Oxford Nanopore Technologies (ONT) platforms. In these approaches there is no pause after the detection of a base or series of bases, thus the sequence is derived in real-time.
* **Barcodes**: A series of known bases added to a template molecule either through ligation or amplification. After sequencing, these barcodes can be used to identify which sample a particular read is derived from.
* **Zero-mode waveguides**: (ZMW). Nanostructure devices used in the Pacific Biosciences (PacBio) platform. Each ZMW well (also called a waveguide) is
several nanometres in diameter and is anchored to a glass substrate. The size of each well does not allow for light propagation, thus the fluorophores bound to bases can only be visualized through the glass substrate in the bottom-most portion of the well, a volume in the zeptolitre
range.
* **Read of insert**: The highest-quality single sequence for an insert, regardless of the number of passes.
* **Consensus sequence**: In next-generation sequencing (NGS) routines that allow multiple overlapping reads from a single molecule of DNA, all related reads are aligned to each other and the most likely base at each position is
determined. This process helps to overcome high, single-pass error rates. A high-quality consensus sequence derived from the circular template from Pacific Biosciences (PacBio) is called a circular consensus sequence (CCS).
* **Squiggle space**: A system exclusively used by Oxford Nanopore Technologies (ONT). As DNA translocates through the pore, a shift in voltage occurs that is directly correlated to a k‐mer within the pore. Thus, the signal derived from a nanopore run is a continuous series of voltage shifts (squiggles) that represent a series of overlapping k‐mers.
* **K‐mer**: A substring within a sequence of bases of some (k) length. Currently, k‐mer sizes of Oxford Nanopore Technologies (ONT) range from 3 to 6 bases.
* **1D and 2D reads**: Oxford Nanopore Technologies (ONT) sequencing allows for both the full forward and full reverse strand of a double-stranded DNA (dsDNA) molecule to be sequenced and associated. A 1D read is the sequence of DNA bases derived from either the forward or reverse DNA strand. A 2D read is a consensus sequence derived from both the forward and the reverse reads.
* **BAC‐by‐BAC sequencing**: A sequencing method where a physical map is generated from overlapping bacterial artificial chromosome (BAC) clones tiled across a chromosome. Each BAC is then fragmented and sequenced.
The sequenced fragments are aligned with the knowledge of the originating BAC.
* **Linked reads**: Reads derived from the 10X Genomics synthetic long-read
platform. These are discontinuous reads each sharing the same barcode, thus they are derived from the same original long molecule.
* **Read cloud**: The means by which the 10X Genomics platform determines
a synthetic long read. Discontinuous linked reads from the same genomic region are aligned to each other. No single linked read contains the entire long sequence; however, when they are stacked, full coverage is achieved.
* **Polymerase reads**: Contiguous sequences of nucleotides incorporated by
the DNA polymerase while reading a template. These reads include sequences from adapters and can represent sequences from multiple passes around a circular template.
* **Single-pass**: The single-molecule real-time (SMRT) sequencing approach
from Pacific Biosciences (PacBio) enables a single molecule of DNA to be
sequenced multiple times. A single pass is one single iteration through a molecule.
* **Subreads**: The sequences derived from a single pass as a polymerase
traverses a DNA molecule multiple times. A subread is trimmed to exclude any
adapter sequence.
* **Whole-exome and targeted sequencing**: Sequencing of only exons or other selected regions. A system of capture or amplification is used to isolate
or enrich for only exons or target regions. This is done by designing probes or primers for the regions of interest.
* **Genome phasing**: A method to identify which chromosome a DNA sequence
is derived from. By examining polymorphisms, the chromosome of origin can be
inferred by matching the reads that share the same variation.
* **Family studies**: A study design in which many members of a family across several generations are sequenced. These studies are used to understand how phenotypes manifest within a particular genotype
background.
* **Helicos Genetic Analysis System**: A sequencing technology based on single nucleotide addition. Each nucleotide contains a ‘virtual terminator’
that prevents the incorporation of multiple nucleotides per cycle.
* **Fluorescence resonance energy transfer**: (FRET; also known as Förster
resonance energy transfer). A system in which energy can be transferred from one light-sensitive molecule to another. When the two molecules are in close
proximity (≤30 nm), energy transferred between the two molecules modulates the intensity of a fluorescence signal.

# References
1. Watson, J. D. & Crick, F. H. The structure of DNA. Cold Spring Harb. Symp. Quant. Biol. 18, 123–131 (1953).
2. Mardis, E. R. Next-generation sequencing platforms. Annu. Rev. Anal. Chem. (Palo Alto Calif.) 6, 287–303 (2013).
**This article provides a concise description of technological advancements supporting NGS.**
3. Wetterstrand, K. A. DNA sequencing costs: data from the NHGRI Genome Sequencing Program (GSP). National Human Genome Research Institute [online], http://www.genome.gov/sequencingcosts (updated 15 Jan 2016).
4. Kircher, M. & Kelso, J. High-throughput DNA sequencing — concepts and limitations. Bioessays 32, 524–536 (2010).
5. Veritas Genetics. Veritas genetics launches \$999 whole genome and sets new standard for genetic testing — Press Release. Veritas Genetics [online], https://www.veritasgenetics.com/documents/VG-launches-999-whole-genome.pdf (updated 4 Mar 2016).
6. Veritas Genetics. Veritas genetics breaks \$1,000 whole genome barrier — Press Release. Veritas Genetics [online], https://www.veritasgenetics.com/documents/VG-PGP-Announcement-Final.pdf (29 Sep 2015).
7. Liu, L. et al. Comparison of next-generation sequencing systems. J. Biomed. Biotechnol. 2012, 251364 (2012).
8. Dressman, D., Yan, H., Traverso, G., Kinzler, K. W. & Vogelstein, B. Transforming single DNA molecules into fluorescent magnetic particles for detection and enumeration of genetic variations. Proc. Natl Acad. Sci. USA 100, 8817–8822 (2003).
9. Shendure, J. et al. Accurate multiplex polony sequencing of an evolved bacterial genome. Science 309, 1728–1732 (2005).
10. Kim, J. B. et al. Polony multiplex analysis of gene expression (PMAGE) in mouse hypertrophic cardiomyopathy. Science 316, 1481–1484 (2007).
11. Leamon, J. H. et al. A massively parallel PicoTiterPlate based platform for discrete picoliter-scale polymerase chain reactions. Electrophoresis 24, 3769–3777 (2003).
12. Fedurco, M., Romieu, A., Williams, S., Lawrence, I. & Turcatti, G. BTA, a novel reagent for DNA attachment on glass and efficient generation of solid-phase amplified DNA colonies. Nucleic Acids Res. 34, e22 (2006).
13. Harris, T. D. et al. Single-molecule DNA sequencing of a viral genome. Science 320, 106–109 (2008).
14. Drmanac, R. et al. Human genome sequencing using unchained base reads on self-assembling DNA nanoarrays. Science 327, 78–81 (2010).
**This paper describes the use of DNA nanoballs to achieve clonal amplification and the use of cPAL to achieve human genome sequencing as implemented by Complete Genomics (BGI).**
15. Tomkinson, A. E., Vijayakumar, S., Pascal, J. M. & Ellenberger, T. DNA ligases: structure, reaction mechanism, and function. Chem. Rev. 106, 687–699 (2006).
16. Landegren, U., Kaiser, R., Sanders, J. & Hood, L. A ligase-mediated gene detection technique. Science 241, 1077–1080 (1988).
17. Valouev, A. et al. A high-resolution, nucleosome position map of C. elegans reveals a lack of universal sequence-dictated positioning. Genome Res. 18, 1051–1063 (2008).
**This paper describes the use of cleavable two-base-encoded probes to achieve genome-wide nucleosome mapping in Caenorhabditis elegans. This technology is implemented by Applied Biosystems (Thermo Fisher) for the SOLiD platform.**
18. Metzker, M. L. Sequencing technologies — the next generation. Nat. Rev. Genet. 11, 31–46 (2010).
19. Ju, J. et al. Four-color DNA sequencing by synthesis using cleavable fluorescent nucleotide reversible terminators. Proc. Natl Acad. Sci. USA 103, 19635–19640 (2006).
20. Guo, J. et al. Four-color DNA sequencing with 3′-O-modified nucleotide reversible terminators and chemically cleavable fluorescent dideoxynucleotides. Proc. Natl Acad. Sci. USA 105, 9145–9150 (2008).
21. Timmerman, L. DNA sequencing market will exceed $20 billion, says Illumina CEO Jay Flatley. Forbes [online], http://www.forbes.com/sites/luketimmerman/2015/04/29/qa-with-jay-flatley-ceo-of-illumina-the-genomics-company-pursuing-a-20b-market/#4dbd19943bf5 (29 Apr 2015).
22. Karow, J. Qiagen launches GeneReader NGS System at AMP; presents performance evaluation by broad. GenomeWeb [online], https://www.genomeweb.com/molecular-diagnostics/qiagen-launches-genereader-ngs-system-amp-presents-performance-evaluation (4 Nov 2015).
23. Smith, D. R. & McKernan, K. Methods of producing and sequencing modified polynucleotides. US Patent 8058030 (2011).
24. Margulies, M. et al. Genome sequencing in microfabricated high-density picolitre reactors. Nature 437, 376–380 (2005).
**This paper describes the development of the first NGS technology through the use of pyrosequencing. The authors demonstrate this method through sequencing of the Mycoplasma genitalium genome.**
25. Rothberg, J. M. et al. An integrated semiconductor device enabling non-optical genome sequencing. Nature 475, 348–352 (2011).
**This paper describes the first non-optical sequencing technology using a massively parallel semi-conductor device to monitor H+ release during DNA synthesis, as implemented by the Ion Torrent platform (Thermo Fisher). The authors demonstrate this technology by sequencing both bacterial and human DNA.**
26. Rieber, N. et al. Coverage bias and sensitivity of variant calling for four whole-genome sequencing technologies. PLoS ONE 8, e66621 (2013).
27. Zook, J. M. et al. Integrating human sequence data sets provides a resource of benchmark SNP and indel genotype calls. Nat. Biotechnol. 32, 246–251 (2014).
28. Nothnagel, M. et al. Technology-specific error signatures in the 1000 Genomes Project data. Hum. Genet. 130, 505–516 (2011).
29. Shen, Y. Sarin, S., Liu, Y., Hobert, O. & Pe'er, I. Comparing platforms for C. elegans mutant identification using high-throughput whole-genome sequencing. PLoS ONE 3, e4012 (2008).
30. Chan, M. et al. Development of a next-generation sequencing method for BRCA mutation screening: a comparison between a high-throughput and a benchtop platform. J. Mol. Diagnost. 14, 602–612 (2012).
31. Wall, J. D. et al. Estimating genotype error rates from high-coverage next-generation sequence data. Genome Res. 24, 1734–1739 (2014).
32. Harismendy, O. et al. Evaluation of next generation sequencing platforms for population targeted sequencing studies. Genome Biol. 10, R32 (2009).
33. BGI. Revolocity Whole Genome Sequencing Service — Press Release. BGI [online], http://u70g92ptbyk941g21dd41fc4.wpengine.netdna-cdn.com/wp-content/uploads/2015/10/Global-WGSRevolocity-ENG-10-15.pdf (2015).
34. Karow, J. BGI halts revolocity launch, cuts complete genomics staff as part of strategic shift. GenomeWeb [online], https://www.genomeweb.com/sequencing-technology/bgi-halts-revolocity-launch-cuts-complete-genomics-staff-part-strategic-shift (23 Nov 2015).
35. Bentley, D. R. et al. Accurate whole human genome sequencing using reversible terminator chemistry. Nature 456, 53–59 (2008).
**This paper demonstrates the use of reversible dye-terminator chemistry for human genome sequencing. This platform is used by the Illumina suite of platforms.**
36. Dohm, J. C., Lottaz, C., Borodina, T. & Himmelbauer, H. Substantial biases in ultra-short read data sets from high-throughput DNA sequencing. Nucleic Acids Res. 36, e105 (2008).
37. Nakamura, K. et al. Sequence-specific error profile of Illumina sequencers. Nucleic Acids Res. 39, e90 (2011).
38. Minoche, A. E., Dohm, J. C. & Himmelbauer, H. Evaluation of genomic high-throughput sequencing data generated on Illumina HiSeq and genome analyzer systems. Genome Biol. 12, R112 (2011).
39. Ley, T. J. et al. DNA sequencing of a cytogenetically normal acute myeloid leukaemia genome. Nature 456, 66–72 (2008).
40. Sarin, S., Prabhu, S., O'Meara, M. M., Pe'er, I. & Hobert, O. Caenorhabditis elegans mutant allele identification by whole-genome sequencing. Nat. Methods 5, 865–867 (2008).
41. Park, P. J. ChIP–seq: advantages and challenges of a maturing technology. Nat. Rev. Genet. 10, 669–680 (2009).
**This review provides an overview of ChIP–seq methods for detecting chromatin–DNA interactions and their importance to epigenetics research.**
42. Buenrostro, J. D., Giresi, P. G., Zaba, L. C., Chang, H. Y. & Greenleaf, W. J. Transposition of native chromatin for fast and sensitive epigenomic profiling of open chromatin, DNA-binding proteins and nucleosome position. Nat. Methods 10, 1213–1218 (2013).
43. Brunner, A. L. et al. Distinct DNA methylation patterns characterize differentiated human embryonic stem cells and developing human fetal liver. Genome Res. 19, 1044–1056 (2009).
44. Wang, Z., Gerstein, M. & Snyder, M. RNA-Seq: a revolutionary tool for transcriptomics. Nat. Rev. Genet. 10, 57–63 (2009).
**This review provides an overview of advances and challenges in techniques that are used in transcriptomic research with a specific focus in methods that use NGS technologies.**
45. Wang, X. et al. A trimming-and-retrieving alignment scheme for reduced representation bisulfite sequencing. Bioinformatics 31, 2040–2042 (2015).
46. Qiagen. Oncology insights enabled by knowledge base-guided panel design and the seamless workflow of the GeneReader NGS system — Press Release. Qiagen [online], http://www.genereaderngs.com/PROM-9192-001_1100403_WP_GeneReader_NGS_0116_NA.pdf (2016).
47. Forgetta, V. et al. Sequencing of the Dutch elm disease fungus genome using the Roche/454 GS-FLX Titanium System in a comparison of multiple genomics core facilities. J. Biomol. Tech. 24, 39–49 (2013).
48. Loman, N. J. et al. Performance comparison of benchtop high-throughput sequencing platforms. Nat. Biotechnol. 30, 434–439 (2012).
49. GenomeWeb. Roche shutting down 454 sequencing business. GenomeWeb [online], https://www.genomeweb.com/sequencing/roche-shutting-down-454-sequencing-business (15 Oct 2015).
50. Malapelle, U. et al. Ion Torrent next-generation sequencing for routine identification of clinically relevant mutations in colorectal cancer patients. J. Clin. Pathol. 68, 64–68 (2015).
51. Li, S. et al. Multi-platform assessment of transcriptome profiling using RNA-seq in the ABRF next-generation sequencing study. Nat. Biotechnol. 32, 915–925 (2014).
52. Life Technologies. Ion semiconductor sequencing uniquely enables both accurate long reads and paired-end sequencing. Life Technologies [online], https://www3.appliedbiosystems.com/cms/groups/applied_markets_marketing/documents/generaldocuments/cms_098680.pdf (2011)
53. Campbell, P. J. et al. Identification of somatically acquired rearrangements in cancer using genome-wide massively parallel paired-end sequencing. Nat. Genet. 40, 722–729 (2008).
54. McCarroll, S. A. & Altshuler, D. M. Copy-number variation and association studies of human disease. Nat. Genet. 39, S37–S42 (2007).
55. Mirkin, S. M. Expandable DNA repeats and human disease. Nature 447, 932–940 (2007).
56. Stankiewicz, P. & Lupski, J. R. Structural variation in the human genome and its role in disease. Annu. Rev. Med. 61, 437–455 (2010).
57. Eid, J. et al. Real-time DNA sequencing from single polymerase molecules. Science 323, 133–138 (2009).
**The authors describe the development of a real-time sequencing method using their zero-mode waveguide sensors as implemented by the Pacific Biosciences platform. The authors demonstrate the technique by sequencing synthetic DNA templates.**
58. Levene, M. J. et al. Zero-mode waveguides for single-molecule analysis at high concentrations. Science 299, 682–686 (2003).
59. Loomis, E. W. et al. Sequencing the unsequenceable: expanded CGG-repeat alleles of the fragile X gene. Genome Res. 23, 121–128 (2013).
60. Clarke, J. et al. Continuous base identification for single-molecule nanopore DNA sequencing. Nat. Nanotechnol. 4, 265–270 (2009).
**The authors demonstrate the use of a mutant alpha-hemolysin for ordered, continuous detection of free nucleotides in solution. This work provides the basis for the approach used by ONT.**
61. Voskoboynik, A. et al. The genome sequence of the colonial chordate, Botryllus schlosseri. eLife 2, e00569 (2013).
62. McCoy, R. C. et al. Illumina TruSeq synthetic long-reads empower de novo assembly and resolve complex, highly-repetitive transposable elements. PLoS ONE 9, e106689 (2014).
63. Schatz, M. C., Delcher, A. L. & Salzberg, S. L. Assembly of large genomes using second-generation sequencing. Genome Res. 20, 1165–1173 (2010).
64. English, A. C. et al. Assessing structural variation in a personal genome-towards a human reference diploid genome. BMC Genomics 16, 286 (2015).
65. Carneiro, M. O. et al. Pacific Biosciences sequencing technology for genotyping and variation discovery in human data. BMC Genomics 13, 375 (2012).
66. Quail, M. A. et al. A tale of three next generation sequencing platforms: comparison of Ion Torrent, Pacific Biosciences and Illumina MiSeq sequencers. BMC Genomics 13, 341 (2012).
67. Koren, S. et al. Hybrid error correction and de novo assembly of single-molecule sequencing reads. Nat. Biotechnol. 30, 693–700 (2012).
68. Larsen, P. A., Heilman, A. M. & Yoder, A. D. The utility of PacBio circular consensus sequencing for characterizing complex gene families in non-model organisms. BMC Genomics 15, 720 (2014).
69. Heger, M. PacBio launches higher-throughput, lower-cost single-molecule sequencing system. GenomeWeb [online], https://www.genomeweb.com/business-news/pacbio-launches-higher-throughput-lower-cost-single-molecule-sequencing-system (01 Oct 2015).
70. Goodwin, S. et al. Oxford Nanopore sequencing, hybrid error correction, and de novo assembly of a eukaryotic genome. Genome Res. 25, 1750–1756 (2015).
71. Jain, M. et al. Improved data analysis for the MinION nanopore sequencer. Nat. Methods 12, 351–356 (2015).
72. Heger, M. 10X Genomics, Pacific Biosciences provide business updates at JP Morgan Healthcare Conference. GenomeWeb [online], https://www.genomeweb.com/sequencing-technology/10x-genomics-pacific-biosciences-provide-business-updates-jp-morgan-healthcare (13 Jan 2016).
73. Cirulli, E. T. & Goldstein, D. B. Uncovering the roles of rare variants in common disease through whole-genome sequencing. Nat. Rev. Genet. 11, 415–425 (2010).
**This review provides a comprehensive overview of advances in, and challenges of using, WGS for variant discovery in human disease.**
74. Ellis, M. J. et al. Whole-genome analysis informs breast cancer response to aromatase inhibition. Nature 486, 353–360 (2012).
75. Prat, A. & Perou, C. M. Mammary development meets cancer genomics. Nat. Med. 15, 842–844 (2009).
76. 1000 Genomes Project Consortium. A map of human genome variation from population-scale sequencing. Nature 467, 1061–1073 (2010).
77. 1000 Genomes Project Consortium. A global reference for human genetic variation. Nature 526, 68–74 (2015).
78. Sudmant, P. H. et al. An integrated map of structural variation in 2,504 human genomes. Nature 526, 75–81 (2015).
79. UK10K Consortium. The UK10K project identifies rare variants in health and disease. Nature 526, 82–90 (2015).
80. Gudbjartsson, D. F. et al. Large-scale whole-genome sequencing of the Icelandic population. Nat. Genet. 47, 435–444 (2015).
81. Regalado, A. U.S. to develop DNA study of one million people. MIT Technology Review [online], http://www.technologyreview.com/news/534591/us-to-develop-dna-study-of-one-million-people (30 Jan 2015).
82. Sidore, C. et al. Genome sequencing elucidates Sardinian genetic architecture and augments association analyses for lipid and blood inflammatory markers. Nat. Genet. 47, 1272–1281 (2015).
83. Hodges, E. et al. Genome-wide in situ exon capture for selective resequencing. Nat. Genet. 39, 1522–1527 (2015).
**This paper describes the in situ capture and selective enrichment of human exons for downstream NGS. This manuscript provides the methodological basis for whole-exome and targeted sequencing.**
84. Iossifov, I. et al. The contribution of de novo coding mutations to autism spectrum disorder. Nature 515, 216–221 (2014).
85. O'Roak, B. J. et al. Sporadic autism exomes reveal a highly interconnected protein network of de novo mutations. Nature 485, 246–250 (2012).
86. Sanders, S. J. et al. De novo mutations revealed by whole-exome sequencing are strongly associated with autism. Nature 485, 237–241 (2012).
87. Griffith, M. et al. Optimizing cancer genome sequencing and analysis. Cell Syst. 1, 210–223 (2015).
88. Rauch, C. et al. Towards an understanding of DNA recognition by the methyl-CpG binding domain 1. J. Biomol. Struct. Dyn. 22, 695–706 (2005).
89. Oda, M. et al. High-resolution genome-wide cytosine methylation profiling with simultaneous copy number analysis and optimization for limited cell numbers. Nucleic Acids Res. 37, 3829–3839 (2009).
90. Irizarry, R. A. et al. Comprehensive high-throughput arrays for relative methylation (CHARM). Genome Res. 18, 780–790 (2008).
91. Meissner, A. et al. Reduced representation bisulfite sequencing for comparative high-resolution DNA methylation analysis. Nucleic Acids Res. 33, 5868–5877 (2005).
92. Flusberg, B. A. et al. Direct detection of DNA methylation during single-molecule, real-time sequencing. Nat. Methods 7, 461–465 (2010).
93. Wescoe, Z. L., Schreiber, J. & Akeson, M. Nanopores discriminate among five C5-cytosine variants in DNA. J. Am. Chem. Soc. 136, 16582–16587 (2014).
94. Lam, E. T. et al. Genome mapping on nanochannel arrays for structural variation analysis and sequence assembly. Nat. Biotechnol. 30, 771–776 (2012).
95. Eichler, E. E., Clark, R. A. & She, X. An assessment of the sequence gaps: unfinished business in a finished human genome. Nat. Rev. Genet. 5, 345–354 (2004).
96. Chaisson, M. J., Wilson, R. K. & Eichler, E. E. Genetic variation and the de novo assembly of human genomes. Nat. Rev. Genet. 16, 627–640 (2015).
97. Chaisson, M. J. et al. Resolving the complexity of the human genome using single-molecule sequencing. Nature 517, 608–611 (2015).
**This article provides strong support for the utility of long-read sequencing for generating high-quality reference genomes. The authors demonstrate this by closing and/or extending gaps and resolving structural variants in the GRCh37 human reference genome.**
98. Ritz, A. et al. Characterization of structural variants with single molecule and hybrid sequencing approaches. Bioinformatics 30, 3458–3466 (2014).
99. Snyder, M. W., Adey, A., Kitzman, J. O. & Shendure, J. Haplotype-resolved genome sequencing: experimental methods and applications. Nat. Rev. Genet. 16, 344–358 (2015).
100. Kuleshov, V. et al. Whole-genome haplotyping using long reads and statistical methods. Nat. Biotechnol. 32, 261–266 (2014).
101. Treutlein, B. et al. Reconstructing lineage hierarchies of the distal lung epithelium using single-cell RNA-seq. Nature 509, 371–375 (2014).
102. Sharon, D., Tilgner, H., Grubert, F. & Snyder, M. A single-molecule long-read survey of the human transcriptome. Nat. Biotechnol. 31, 1009–1014 (2013).
103. Quick, J. et al. Rapid draft sequencing and real-time nanopore sequencing in a hospital outbreak of Salmonella. Genome Biol. 16, 114 (2015).
104. Quick, J. et al. Real-time, portable genome sequencing for Ebola surveillance. Nature 530, 228–232 (2016).
105. GenomeWeb. White House announces efforts to accelerate precision medicine initiative. GenomeWeb [online], https://www.genomeweb.com/molecular-diagnostics/white-house-announces-efforts-accelerate-precision-medicine-initiative (25 Feb 2016).
106. Illumina. Illumina forms new company to enable early cancer detection via blood-based screening — Press Release. Illumina [online], http://www.illumina.com/company/news-center/press-releases/press-release-details.html?newsid=2127903 (10 Jan 2016).
107. Schatz, M. C. & Langmead, B. The DNA data deluge: fast, efficient genome sequencing machines are spewing out more data than geneticists can analyze. IEEE Spectr. 50, 26–33 (2013).
108. Pop, M. & Salzberg, S. L. Bioinformatics challenges of new sequencing technology. Trends Genet. 24, 142–149 (2008).
109. Sunyaev, S. R. Inferring causality and functional significance of human coding DNA variants. Hum. Mol. Genet. 21, R10–R17 (2012).
110. Gargis, A. S. et al. Assuring the quality of next-generation sequencing in clinical laboratory practice. Nat. Biotechnol. 30, 1033–1036 (2012).
111. Chrystoja, C. C. & Diamandis, E. P. Whole genome sequencing as a diagnostic test: challenges and opportunities. Clin. Chem. 60, 724–733 (2014).
112. McGuire, A. L. et al. Point-counterpoint. Ethics and genomic incidental findings. Science 340, 1047–1048 (2013).
113. Bowers, J. et al. Virtual terminator nucleotides for next-generation DNA sequencing. Nat. Methods 6, 593–595 (2009).
114. Heger, M. China's Direct Genomics unveils new targeted NGS system based on Helicos Tech for clinical use. GenomeWeb [online], https://www.genomeweb.com/business-news/chinas-direct-genomics-unveils-new-targeted-ngs-system-based-helicos-tech-clinical-use (27 Oct 2015).
115. Karow, J. Oxford Nanopore presents details on new high-throughput sequencer, improvements to MinIon. GenomeWeb [online], https://www.genomeweb.com/sequencing/oxford-nanopore-presents-details-new-high-throughput-sequencer-improvements-mini (16 Sep 2014).
116. Karow, J. Sigma-Aldrich enters co-marketing agreement with GenapSys for Genius sequencer. GenomeWeb [online], https://www.genomeweb.com/sequencing-technology/sigma-aldrich-enters-co-marketing-agreement-genapsys-genius-sequencer (1 Jul 2015).
117. Roche. Roche acquires Genia Technologies to strengthen next generation sequencing pipeline — Press Release. Roche [online], http://www.roche.com/media/store/releases/med-cor-2014-06-02.htm (2 Jun 2014).
118. Heger, M. Illumina unveils mini targeted sequencer, semiconductor sequencing project at JP Morgan Conference. GenomeWeb [online], https://www.genomeweb.com/sequencing-technology/illumina-unveils-mini-targeted-sequencer-semiconductor-sequencing-project-jp (1 Jan 2016).
119. NanoString. NanoString Technologies presents proof-of-concept data for novel massively parallel single molecule sequencing chemistry at AGBT meeting — Press Release. NanoString [online], http://investors.nanostring.com/releasedetail.cfm?ReleaseID=954517 (11 Feb 2016).
120. Raz, T. & Pascaline, M. Nucleic acid target detection using a detector, a probe and an inhibitor. US Patent 20130344485 (2013).
121. Mankos, M. et al. A novel low energy electron microscope for DNA sequencing and surface analysis. Ultramicroscopy 145, 36–49 (2014).
122. Augenlicht, L. H. & Kobrin, D. Cloning and screening of sequences expressed in a mouse colon tumor. Cancer Res. 42, 1088–1093 (1982).
123. Dandy, D. S., Wu, P. & Grainger, D. W. Array feature size influences nucleic acid surface capture in DNA microarrays. Proc. Natl Acad. Sci. USA 104, 8223–8228 (2007).
124. Keating, B. J. et al. Concept, design and implementation of a cardiovascular gene-centric 50 k SNP array for large-scale genomic association studies. PLoS ONE 3, e3583 (2008).
125. DeRisi, J. et al. Use of a cDNA microarray to analyse gene expression patterns in human cancer. Nat. Genet. 14, 457–460 (1996).
126. Alizadeh, A. A. & Staudt, L. M. Genomic-scale gene expression profiling of normal and malignant immune cells. Curr. Opin. Immunol. 12, 219–225 (2000).
127. Rhodes, D. R. et al. Large-scale meta-analysis of cancer microarray data identifies common transcriptional profiles of neoplastic transformation and progression. Proc. Natl Acad. Sci. USA 101, 9309–9314 (2004).
128. Vora, G. J., Meador, C. E., Stenger, D. A. & Andreadis, J. D. Nucleic acid amplification strategies for DNA microarray-based pathogen detection. Appl. Environ. Microbiol. 70, 3047–3054 (2004).
129. Wilson, W. J. et al. Sequence-specific identification of 18 pathogenic microorganisms using microarray technology. Mol. Cell Probes 16, 119–127 (2002).
130. Imai, K., Kricka, L. J. & Fortina, P. Concordance study of 3 direct-to-consumer genetic-testing services. Clin. Chem. 57, 518–521 (2011).
131. Dolgin, E. Personalized investigation. Nat. Med. 16, 953–955 (2010).
132. Jia, P., Wang, L., Meltzer, H. Y. & Zhao, Z. Common variants conferring risk of schizophrenia: a pathway analysis of GWAS data. Schizophr. Res. 122, 38–42 (2010).
133. Welter, D. et al. The NHGRI GWAS Catalog, a curated resource of SNP-trait associations. Nucleic Acids Res. 42, D1001–D1006 (2014).
134. Carter, N. P. Methods and strategies for analyzing copy number variation using DNA microarrays. Nat. Genet. 39, S16–S21 (2007).
135. Vrijenhoek, T. et al. Recurrent CNVs disrupt three candidate genes in schizophrenia patients. Am. J. Hum. Genet. 83, 504–510 (2008).
136. Marshall, C. R. et al. Structural variation of chromosomes in autism spectrum disorder. Am. J. Hum. Genet. 82, 477–488 (2008).
137. Buck, M. J. & Lieb, J. D. ChIP-chip: considerations for the design, analysis, and application of genome-wide chromatin immunoprecipitation experiments. Genomics 83, 349–360 (2004).
138. Liang, L. et al. A cross-platform analysis of 14,177 expression quantitative trait loci derived from lymphoblastoid cell lines. Genome Res. 23, 716–726 (2013).
139. Zhao, S., Fung-Leung, W. P., Bittner, A., Ngo, K. & Liu, X. Comparison of RNA-Seq and microarray in transcriptome profiling of activated T cells. PLoS ONE 9, e78644 (2014).
140. Holland, P. M., Abramson, R. D., Watson, R. & Gelfand, D. H. Detection of specific polymerase chain reaction product by utilizing the 5′right arrow3′ exonuclease activity of Thermus aquaticus DNA polymerase. Proc. Natl Acad. Sci. USA 88, 7276–7280 (1991).
141. Morin, P. A. & McCarthy, M. Highly accurate SNP genotyping from historical and low-quality samples. Mol. Ecol. Notes 7, 937–946 (2007).
142. VanGuilder, H. D., Vrana, K. E. & Freeman, W. M. Twenty-five years of quantitative PCR for gene expression analysis. Biotechniques 44, 619–626 (2008).
143. Weaver, S. et al. Taking qPCR to a higher level: Analysis of CNV reveals the power of high throughput qPCR to enhance quantitative resolution. Methods 50, 271–276 (2010).
144. Sedlak, R. H., Cook, L., Cheng, A., Magaret, A. & Jerome, K. R. Clinical utility of droplet digital PCR for human cytomegalovirus. J. Clin. Microbiol. 52, 2844–2848 (2014).
145. Kulkarni, M. M. in Current Protocols in Molecular Biology Ch. 25 (eds Ausubel, F. M. et al.) (Wiley, 2011).
146. Nielsen, T. et al. Analytical validation of the PAM50-based Prosigna Breast Cancer Prognostic Gene Signature Assay and nCounter Analysis System using formalin-fixed paraffin-embedded breast tumor specimens. BMC Cancer 14, 177 (2014).
147. Ku, B. M. et al. High-throughput profiling identifies clinically actionable mutations in salivary duct carcinoma. J. Transl. Med. 12, 299 (2014).
148. Sailani, M. R. et al. The complex SNP and CNV genetic architecture of the increased risk of congenital heart defects in Down syndrome. Genome Res. 23, 1410–1421 (2013).
149. Lira, M. E. et al. Multiplexed gene expression and fusion transcript analysis to detect ALK fusions in lung cancer. J. Mol. Diagn. 15, 51–61 (2013).
150. Schwartz, D. C. et al. Ordered restriction maps of Saccharomyces cerevisiae chromosomes constructed by optical mapping. Science 262, 110–114 (1993).
151. Hastie, A. R. et al. Rapid genome mapping in nanochannel arrays for highly complete and accurate de novo sequence assembly of the complex Aegilops tauschii genome. PLoS ONE 8, e55864 (2013).
152. Cao, H. et al. Rapid detection of structural variation in a human genome using nanochannel-based genome mapping technology. Gigascience 3, 34 (2014).
153. Pendleton, M. et al. Assembly and diploid architecture of an individual human genome via single-molecule technologies. Nat. Methods 12, 780–786 (2015).
154. Life Technologies. 5500 W series genetic analyzers. Life Technologies [online], https://tools.thermofisher.com/content/sfs/brochures/5500-w-series-spec-sheet.pdf (2012).
155. Yuzuki, D. BGISEQ-500 debuts at the International Congress of Genomics 10. Next Generation Technologist [online], http://www.yuzuki.org/bgiseq-500-debut-at-the-international-congress-of-genomics-10 (24 Oct 2015).
156. Winnick, E. Illumina launches four new systems; provides financial, Dx update at JP Morgan. GenomeWeb [online], https://www.genomeweb.com/business-news/illumina-launches-four-new-systems-provides-financial-dx-update-jp-morgan (12 Jan 2015).
157. [No authors listed.] Illumina HiSeq 3000 Service Fees. Oregon State University [online], http://cgrb.oregonstate.edu/core/illumina-hiseq-3000/illumina-hiseq-3000-service-fees (updated 1 Jan 2016)
158. Heger, M. Thermo Fisher launches new systems to focus on plug and play targeted sequencing. GenomeWeb [online], https://www.genomeweb.com/sequencing-technology/thermo-fisher-launches-new-systems-focus-plug-and-play-targeted-sequencing (1 Sep 2015).
159. Ip, C. L. et al. MinION analysis and reference consortium: Phase 1 data release and analysis. F1000Research 4, 1075 (2015).
160. Glenn, T. C. Field guide to next-generation DNA sequencers. Mol. Ecol. Resour. 11, 759–769 (2011).
161. Karow, J. At AGBT, 10X Genomics launches GemCode platform; shipments slated for Q2 as firm battles IP lawsuits. GenomeWeb [online], https://www.genomeweb.com/sample-prep/agbt-10x-genomics-launches-gemcode-platform-shipments-slated-q2-firm-battles-ip-lawsuits (2 Mar 2015).

# FURTHER INFORMATION
- [10X Genomics](http://www.10xgenomics.com/)
- [454 Sequencing](http://www.454.com/)
- [Advances in Genome Biology and Technology (AGBT)](http://www.agbt.org/)
- [BGISEQ-500](http://seq500.com/en/portal/Sequencer.shtml)
- [Illumina](http://www.illumina.com/)
- [Ion Torrent](https://www.thermofisher.com/us/en/home/brands/ion-torrent.html)
- [Oxford Nanopore Technologies](https://www.nanoporetech.com/)
- [Pacific Biosciences](http://www.pacb.com/)
- [Personal Genome Project](http://www.personalgenomes.org/)
- [SOLiD Next-Generation Sequencing](http://www.thermofisher.com/us/en/home/life-science/sequencing/next-generation-sequencing/solid-next-generation-sequencing.html)
- [The 1000 Genomes Project](http://www.1000genomes.org/)

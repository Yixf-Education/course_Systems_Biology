* [BPSM Assignment 1](http://129.215.170.35/BPSM_2018_Assignment1.html)
BPSM Assignment 1
Due 14:00 Fri 12 October 2018
Background to the technology
Next Generation Sequencing (NGS) is the broad term used to describe the process whereby millions of sequence reads (or read-pairs) are generated from samples at a comparatively low cost. If you'd like to find out more about the technology and its uses, https://www.illumina.com/ is a good place to start!
RNA-Seq (RNA sequencing), as a generic technique, enables us to assess the levels of gene transcripts (usually mRNA molecules) in a group of samples, perhaps to see how gene expression levels change over time, or, perhaps to answer a question like: "what happens when drug X is administered to cultured mouse heart cells: how do the cells respond at the gene level, and what role do those genes play?".
As you can probably guess, there are actually many different applications for the technology, some of which are described here:
https://en.wikipedia.org/wiki/RNA-Seq.

Background to the biology
Trypanosoma brucei spp (comprising Trypanosoma brucei brucei and the human infective forms T. b. rhodesiense and T. b. gambiense) are eukaryotic protozoan parasites responsible for African sleeping sickness in 36 countries of sub-Saharan Africa, which are the poorest developing countries worldwide.
Sleeping sickness has a devastating impact on human health and prosperity: >0.5 million cases and 70,000 deaths per year are a result of the parasite and the disease can be fatal unless treated. The parasite also infects cattle and game animals (where it causes the disease ‘nagana’).
The trypanosome is transmitted between mammalian hosts by the tsetse fly, Glossina spp, in which it initially establishes in the midgut after a bloodmeal but then migrates to the salivary glands in preparation for transmission to a new mammalian host (see image below). In mammals, the parasite survives free in the bloodstream, being able to evade antibody responses through antigenic variation.
Trypanosomes proliferate in the mammalian bloodstream as morphologically "slender" forms, these being replaced by non-proliferative "stumpy" forms as parasite numbers increase. The accumulation of division-arrested forms limits the increase in parasite numbers and thereby prolongs host survival (and hence the probability of disease transmission back into the insect host for the cycle to continue).


https://www.researchgate.net/publication/8077434_The_developmental_cell_biology_of_Trypanosoma_brucei

Your task
You have been asked to have a look at some RNA-Seq data that have been generated from Trypanosoma brucei brucei. The research lab is particularly interested in whether there are any differences in gene expression levels in two different life cycle stages: "slender" and "stumpy". There are three biological replicates for each of the two conditions, and the technology used was paired-end sequencing.

There are online tools that could be used (at least in part) to process and analyse this kind of data (e.g. https://usegalaxy.org/), but in this instance, we are going to do all the processing from scratch using the command-line interface (i.e. in a terminal) on our MSc course server.

The goal for this assignment is to write a pipeline programme that, when executed in a Unix terminal on our MSc server, will process the data provided in the directory /localdisk/data/BPSM/Assignment1/fastq. The sample details are also in this directory, in a file called fqfiles. The slender samples are the first three, the stumpy ones the last three.

The pipeline should have the following minimum overall design:
perform a quality check on the paired-end raw sequence data (which are in gzip compressed fastq format; https://support.illumina.com/bulletins/2016/04/fastq-files-explained.html) using the installed programme fastqc
assess the numbers and quality of the raw sequence data based on the output of fastqc
align the read pairs to the Trypanosoma brucei brucei genome using installed programme bowtie2, converting the output to indexed "bam" format with samtools; the Trypanosoma brucei brucei genome sequence is provided in the directory /localdisk/data/BPSM/Assignment1/Tbb_genome/
generate counts coverage data: the number of reads that align to the regions of the genome that code for genes; this is to be done using the installed programme bedtools and the Tbbgenes.bed "bedfile" that contains the information about the gene locations in the genome; the bedfile is provided in the directory /localdisk/data/BPSM/Assignment1/
generate a plain text tab-delimited output that gives the statistical mean (average) of the counts per gene for each group, e.g. gene name, mean for slender samples, mean for stumpy samples.

Considerations
don't panic: it isn't as bad as it first looks!
don't immediately try to start coding! This is a pipeline made up of various component "bits": try drawing it out first on a piece of paper, so that you can clearly understand what the inputs and outputs are for each "bit": this is time very well spent...
most programmes have many parameters/flags that can be set by the user: the defaults are not always the best, so chose wisely
most programmes have a "-h" for help
try to make it so the user doesnt actually have to do much other than execute the programme
the "genome sequence" actually comprises many sequences, and will need to be made into a "bowtie2" database before it can be used
normally, when you get raw sequence data, you'd get lots more that this, and each sample wouldnt have the same number of read-pairs...
Google is your friend
I like to think I am your friend too, but I really can't tell you the answers, no matter how politely you ask, sorry...

What should be submitted for this assignment
a plain text file that is your pipeline/programme code that I can run directly on our server. It should contain "comments" (i.e. lines with a # at start of the line) so than anyone looking at the code knows what each bit is doing
a PDF file that:
has an overview that describes how the pipeline processes the data
indicates any things the user does have to do to make things work
indicates why you have chosen the parameters/flags that you have for each step
highlights any difficulties, if any, that you have come across
indicates any additional/alternative features that you think might be beneficial to include

What I'll be looking for
the programme that you have written: it must be your work (but by all means discuss things with your colleagues)
comments in the code so that I can see what it does
a programme that works and produces the requested output in the correct format
any additional "flexibility" or features that have been added/suggested that indicate to me that you understand what is being done/not done AND why your pipeline helps biology (this is BIOinformatics after all!)

What I would rather not see...
I have nearly 50 assignments to mark, so....
(please) keep the PDF content "focussed"! It is quality, not quantity, that is more important ...
the pipeline can actually be written using quite a small number of (carefully constructed) commands, so if your programme is hundreds of lines, you are probably not doing the "right" thing!


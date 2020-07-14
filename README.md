# Bioinformatics

A suite of modules, pipelines, and tutorials for common DNA and RNA sequence analysis for use on the University of Sydney's [High Performance Computing service](https://informatics.sydney.edu.au/services/artemis/).


Acknowledgements (and co-authorship, where appropriate) are an important way for us to demonstrate the value we bring to your research. Your research outcomes are vital for ongoing funding of the Sydney Informatics Hub. If you use any SIH material towards a publication, please acknowledge the Sydney Informatics Hub.

Suggested acknowledgement:
This research was supported by the Sydney Informatics Hub and the University of Sydney’s high performance computing service, Artemis, funded by the University of Sydney.

## NCI Gadi optimised pipelines

The Sydney Informatics Hub has worked alongside with the National Compute Infrastructure (NCI) team to establish fast, efficient and scalable bioinformatics workflows on NCI’s HPC, Gadi. The workflows implement best practice workflows and reputable software and are specifically designed to utilise NCI Gadi’s infrastructure optimally. The table below contains a list and descriptions of bioinformatics workflows optimised for NCI Gadi that are available on our GitHub page. 


| Github Repo| Description     |	Software	|
|-----------|-----------------|-----------------|
|[QC-tools]|Obtain fastQC reports, perform trimming, convert quality score encodings for fastq files|fastQC, multiQC, BBTools|
|[FASTQ-BAM]|Whole genome sequence alignment to a reference genome following pre-processing recommendations by the BROAD Institute|bwa-kit, fastp, BWA-MEM, SAMbamba, SAMblaster, SAMtools, GATK 4|
|[Germline-ShortV]|Germline short variant calling (joint calling) following the Germline short variant discovery (SNPs + Indels) Best Practices Workflow by the BROAD Institute|GATK4|
|[Somatic-ShortV]|Somatic short variant calling (joint calling) following the Somatic short variant discovery (SNPs + Indels) Best Practices Workflow by the BROAD Institute for tumour-normal pairs|GATK 4|
|[StructuralV]|TBA: Structural variant calling using MANTA, GRIDSS2 and CNVkit|Manta, GRIDSS2, CNVkit|
|[RNASeq-DE]|Process RNA sequencing data for differential expression, including fastQC, trimming, mapping with STAR and obtaining a raw count matrix|fastQC, multiQC, bbduk, STAR, RSeQC, HTSeq|

## NCI Raijin optimised pipelnes

| Github Repo| Description     |	Software	|
|-----------|-----------------|-----------------|
|[SIH-Raijin-Trinity](https://github.com/Sydney-Informatics-Hub/SIH-Raijin-Trinity)| Trinity assembles Illumina RNA-Seq data into transcript sequences. Trinity was developed at the Broad Institute and the Hebrew University of Jerusalem. SIH-Raijin-Trinity allows Trinity to be scalable by enabling use of multiple nodes on NCI Raijin. The entire workflow can complete ~4X faster using 10 broadwell nodes!| samtools/1.9, java/jdk1.8.0_60, bowtie2/2.3.3.1, jellyfish/2.2.6, salmon/0.11.0, perl/5.22.1, trinity/2.8.4, python3/3.6.7|


## Suggested workflows

### Whole genome sequencing

__Human__


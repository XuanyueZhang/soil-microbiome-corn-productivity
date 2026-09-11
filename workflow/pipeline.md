# Bioinformatics Pipeline

## 1. Sample Collection
Composite soil samples are collected from organic and conventional corn fields at two time points:
- Pre-planting
- Mid-to-late growth

## 2. DNA and RNA Extraction
- DNA: DNeasy PowerSoil Pro Kit
- RNA: RNeasy PowerSoil Total RNA Kit

## 3. Sequencing
- Illumina paired-end sequencing
- Metagenomic sequencing for microbial community composition
- Metatranscriptomic sequencing for gene-expression activity

## 4. Read Quality Control
Raw sequencing reads are processed using:
- fastp
- Trimmomatic

These steps remove adapters, low-quality reads, and sequencing artifacts.

## 5. Metagenomic Analysis
- metaSPAdes: assemble reads into contigs
- MetaBAT2: bin contigs into metagenome-assembled genomes
- CheckM: evaluate genome completeness and contamination

## 6. Metatranscriptomic Analysis
- rnaSPAdes: transcript assembly
- Salmon: transcript quantification
- DESeq2: differential expression analysis

## 7. Functional and Taxonomic Annotation
Candidate taxa and genes are characterized using databases such as:
- KEGG
- eggNOG
- NCBI RefSeq

## 8. Statistical Analysis
Planned analyses include:
- Microbial diversity analysis
- Differential expression
- Microbiome-wide association analysis
- ANCOVA
- Multi-omics integration using vegan and mixOmics

## 9. Predictive Modeling
Random Forest models are proposed to integrate:
- Microbial taxa
- Functional genes
- Soil chemistry
- Environmental metadata
- Agricultural management variables

The final objective is to identify predictors of corn yield and soil health.

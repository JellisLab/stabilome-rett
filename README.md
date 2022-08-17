### Introduction
Code and data to measure the contribution of RNA stability to the misregulation of genes in Rett iPSC-derived neurons. Look up [preprint paper](https://www.biorxiv.org/content/10.1101/2021.12.11.472181v1) for details.

### Data
The *data* folder contains auxiliary sequence data, quantified genes based on pA sites from the polyA_DB 3 database [PMID: 29069441](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5753232/) and quantified microRNAs. 

### R notebooks
1. **process_counts_data.Rmd**

   Estimate fold-changes in transcription rate, steady state abundance and mRNA half-lifes from drosophila normalized gene level counts data. Gene counts were obtained from as a sum of counts from all pA sites of a gene.
2. **measure_global_HL.Rmd**

   Average mRNA half-life between cell types based on saturation curve method.
3. **buffering_of_TR.Rmd**

   Buffering of transcription rate changes with mRNA half-life
4. **train_random_forest_on_TR.Rmd**

   Train the random forest classifier for transcription rate changes based on k-mer content of coding and gene body sequence.
5. **microRNA_analysis.Rmd**

   Normalize endogenous microRNA abundances with spike-in RNA.
6. **construct_primir_annotation.Rmd**

   Prepare pA sites annotations of primary microRNAs based on transcripts annotation from [PMID: 26290535] (https://genome.cshlp.org/content/25/9/1401)
7. **transite_analysis.Rmd**

   Identify sequence features of buffered mRNAs relative to mRNAs with a same direction of transcription rate shift.

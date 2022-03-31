# SCTLD-metagenomes
Workflow of metagenomics on coral samples to learn more about SCTLD. The workflow is divided in several steps down below. 


# Quality control
For correct re-assembly of samples, quality control is required. Sequence trimming is performed with Trimgalore, which uses the Cutadapt software to remove adapter sequences. Subsequent quality control is done with FastQC. Optionally, host (and maybe later symbiont) sequences can be removed from the files using Bowtie2 and Samtools. 


# Assembly

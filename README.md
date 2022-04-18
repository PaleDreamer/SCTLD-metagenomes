# SCTLD-metagenomes
Workflow of metagenomics on coral samples to learn more about SCTLD. The workflow is divided in several steps down below. If working with these files, do note the following: 
* **Installation**: This is not included in these files. Most if not all of these softwares use conda anyways, so that should work just fine. If working on Hydra, please make sure that your files are compatible with the job files for Hydra. Also make sure to activate your environments.
* **Code**: Code with comments and commentary can be found in the Jupyter notebooks in this GitHub repository. This provides you with a baseline of commands that you can use. Make sure to look at the data organization I use before starting this, because it heavily influences the way I write my code.
* **Job files**: If you are working on Hydra, I have pooled all my finalized job files in the "Job files" directory. They are ready to submit, excepting any changes to Hydra architecture. Simply copy these files to your local computer/Hydra and qsub will do the rest. 

# Data Organization
All directories have the same basic layout. This is to make sure writing scripts is easy and there is no need for going back and forth between the different directories. I start with a main directory that tells me what dataset I am working on. I then add directories for all the main steps in the process, denoted by double-digit numbers (00_raw, 01_quality, 02_assembly, etc.). Within one of those directories are 3 main directories: data, jobs, and logs. Data then contains 2 more: working and results. Together, this is an easily replicated structure that allows straightforward file organization. **NOTE**: I add databases, where necessary, in a directory in the very first directory. This way, all steps have a central database to use. 

# Quality control
For correct re-assembly of samples, quality control is required. Sequence trimming is performed with Trimgalore, which uses the Cutadapt software to remove adapter sequences. Subsequent quality control is done with FastQC. Optionally, host (and maybe later symbiont) sequences can be removed from the files using Bowtie2 and Samtools. 


# Assembly
Assembly is performed using MegaHIT, due to its memory efficiency. MegaHIT uses k-mer dependent assembly and has several subsettings. I have chosen the optimal settings for MegaHIT, but feel free to experiment and maybe find some other things as well. Contig quality is assessed by QUAST, which can give you basic stats without a reference assembly. *Need to find how to make one for more detailed information*

# Mapping
Re-aligning the raw reads (or the filtered reads) back to the contigs is an essential step to create depth-of-sequencing indexes for your binning step. This step is performed using Bowtie2 and samtools. *Script currently large and error-prone. Seeing if fixable*

# Binning

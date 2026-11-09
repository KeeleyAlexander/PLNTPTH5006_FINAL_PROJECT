# Final Project Proposal 
## Overview 
This project will establish a workflow for processing raw reads. The samples are in fastqc.gz format and come from 6 cats at several time points. There are 102 files (R1 and R2) and 51 total samples. This data comes from Dr. Jenessa Winston and another course had already processed the data so my group coud do downstream analysis. I would like to learn how to do the processing work myself so I can better understand the data and workflow. This data is available on another project folder I am apart of in OSC. I'm currently working on getting permissions to copy the data to this project. 
## Outline and Technical Aspects 
I'm currently deciding whether I want to use nf-core pipeline. If I don't use it, I feel I would be more confident in script writing and using programs. If i do use it, I could include some downstream analyses in R/quartero since I have not done any of the computational work on this data in my group project. My current idea is to not use the pipeline and if I have time perform more downstream analyses. I'd love input in this area. 

**If I dont use nf-core pipeline steps:**

*Taxonomic Profiling*
- read qc (FastQC)
- adapter and quality trimming (TrimGalore)
- removal of contaminents (BBSplit)
- Alignement to reference genome (Kraken2 or MetaPhlAn)

*Assembly*
- De Novo Assembly (MEGAHIT)
- Map reads to contigs (Bowtie2 and Samtools)
- Binning (MetaBAT2)
- Quality of MAGs (CheckM)

```
Note: Although I have slowly learned what all of these steps mean verbally in my other class, I have no experience with the computational side
```
## Limitations and Uncertainties
I am still a little confused on the difference between refernece based analysis and de novo and when to combine the two processes and why this data should be processed de novo (since that is what they did for us in my other course). I'm also a little hesitant about the downstream analyses because I have been continually lost on that aspect in my other course and we haven't gone too far into the R portion of this course, though I'm sure that will help. 

## Project Choice
I chose this project because I am actively working with the data and I thought it would help me understand it better if I got hands on experience from start to finish. Curretly in my team for this project I am the interpreter and translating the findings to physiological relevance, but I find interpreting the data that I have not generated to be challanging. 




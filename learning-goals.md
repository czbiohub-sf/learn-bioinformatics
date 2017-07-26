# Learning goals

The purpose of this document is to hold the learning goals for teaching
bioinformatics to beginners

For lesson plans, check :

- Software Carpentry's lessons
- Rosalind problems for biology-specific programming problems to practice with Python
- Python for Biologists
- Python Data Science Handbook


[TOC]: # "Table of contents"



## Getting set up

Installing ...

- Anaconda Python
- Atom text editor
- git
- Starting up a Jupyter notebook
- Changing the default font (because with Courier you can't tell the difference
  between 1 "one" and l "ell" )
- 

## Potential project-driven tasks


### Given a list of genes, get their enriched promoter motifs

Could maybe use RBPs instead of TFs since I know them better

- `grep` a gtf file for the gene names and only get "gene" lines
- use `bedtools flank` to get upstream 1000bp
- Unsupervised problem:
  - Use HOMER or other motif enricher and use all genes' upstream sequences as background
    - Get to talk about background which is important
    - HOMER motifs are very satifying
  - Count enriched kmers (using Python??)
    - Do a multiple sequence alignment
- Supervised problem:
    - Use UCSC genome browser to download transcription
  factor binding sites
    - Use `bedtools intersect` to overlap with other bed file


How can students have ownership?

- Get genes from a paper they picked
- Use a TF they're interested in

### Amy - Assembling contigs

- Get sanger sequencing reads
- Assemble subsets into contigs using `velvet`
- Align contigs to known sequence using `bwa`
- Find mismatches/SNPs using `???` vcftools?

How can students have ownership?

- Use contigs from something they created
- 


### Collaboration (git)

Teach them a bunch of different things and separate the problem into three
steps, where steps 1 and 2 are independent and feed into 3.

## Command line tools


### Unix basics
Modify Software Carpentry lessons

- Ls
    - Anatomy of a command
    - Ls -l
    - Ls -lh
- Chmod
    - Octal codes
    - Chmod 775
    - Chmod ug+r
    - Chmod og-w
- Cd
- pwd
- Mkdir
    - Mkdir folder/subfolder
- Head
    - Head -n 17
- Less
    - Less -S
- Tail
    - Tail -n 2
- Echo
- Touch
- Cat
- Wc
    - Wc -l
- Cp
- Mv
- Rm

### Makefiles


### Grep
- Search for specific term
- Search for lines that don’t match
- Add lines after
    - E.g. fastq

### Awk
- Select columns
- Get number of fields

### Git

- Cheatsheets repo

### bedtools

- intersect
- flank


# terminal-tutorial
Introduction to navigating a computer's system files, presented to the Moczek Lab at Indiana University. This tutorial will have two parts: 

1) <b>Phil on screen</b>: Review of common terminal commands, referencing this nice guide: https://gist.github.com/bradtraversy/cc180de0edee05075a6139e42d5f28ce#file-terminal-commands-md

2) <b>Together</b>: Working through a practice set of exercises, using a test set of genomic data from the Onthophagus sagittarius genome project (below).

## Exploring the <i>O. sagittarius</i> data

Before we begin, please make sure you have saved the folder conatining Osag data (from OneDrive) to your "Desktop" and rename the folder "osag1". 

Now, lets navigate to this folder via the terminal, using the "call directory" command:

```bash
cd ~/Desktop/osag1
```

And now let's check out what files are inside: 

```bash
ls -lh 
```
We can see that our "osag1" directory has 2 files (the genome sequence, and a masked version of the genome sequence) and three directories containing information about how the genome was annotated (genes, repeats, and annotations). 

We can also print what is inside other directories, without having to go into the directory first:

```bash
ls -lh ./genes
```

This directory contains three files.
1) A `gtf` file that describes the genomic locations of different gene features
2) A `fasta` file describing the nueclotide form of Osag genes
3) A `fasta` file describing the protein form of Osag genes


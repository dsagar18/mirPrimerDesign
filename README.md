*A primer designing tool for miRNA*
# miRNA-Primer-Designing-Tool
Designs forward, reverse and RT primers for miRNA

********************mirPrimerDesign*********************
Contains:
1) The python code: mirPrimerDesign.py
2) The list of short NEB adaptors: short_indexed_adaptors.txt
3) A folder called "example" where you can run the code with a sample fasta file and check the output

What does it do?

Designs forward, reverse and RT primers for a set of miRNA. Works for any miRNA from any organism.

Requirements
Python version 2.x/3.x 

Instructions:
1) Make sure that your input file is in the typical fasta format e.g.:
>hsa-miR-3124-5p_MIMAT0014986_Homo_sapiens_miR-3124-5p
UUCGCGGGCGAAGGCAAAGUC
Note: the name in the header line could be anything you want

2) The Next line, i.e. the nucleotide fasta sequence contains ONLY the mature sequence of the desired miRNA e.g.:
>hsa-miR-3124-5p_MIMAT0014986_Homo_sapiens_miR-3124-5p
UUCGCGGGCGAAGGCAAAGUC

3) Try to make sure that the input fasta file name has its words separated by "_" and not spaces. e.g.:
mirna fasta file.fasta = Less preferable
mirna_fasta_file.fasta = More preferable

4) The fasta file to be given as the input should be in the same folder/directory as that of the python code mirPrimerDesign.py

Usage:
"python mirPrimerDesign.py"
#on entering the above given command, the tool will ask for the name of the fasta file
containing the mature fasta sequences of all your desired miRNA

Ouput:
A file named "miRNA_primers.txt" containing the name of the miRNA, its mature sequence and the forward, reverse and RT primers along with the melting temperatures of the forward and reverse primers.

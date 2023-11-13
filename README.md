# Type1_Protospacers
Script for the identification of type I(-C) protospacer sequences and evaluation of off-target sites.

To run this notebook, pandas (https://pandas.pydata.org/) and BioPython (https://biopython.org/) are required. To search for protospacers, simply provide the file path to an input genome in FASTA format, adjust the target region of interest, and define an output directory. Parameters such as PAM, spacer length, and seed length can be adjusted to provide compatibility with other type I CRISPR systems. The default parameters are for the type I-C CRISPR system from Pseudomonas aeruginosa (https://doi.org/10.1038/s41592-020-00980-w).

For the evaluation of off-target sites, only the seed sequence is used. Off-targets are only counted if a PAM site is present. Therefore, in the final dataframe, a match count of 1 indicates that no off-target sites were found. 


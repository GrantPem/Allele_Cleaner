# Allele_Cleaner
  
- Uses biopython version 1.81
- This Python script is designed to remove redundant amino acid sequences that appear after translating a nucleotide with synonymous snips from a FASTA file. The FASTA file can contain both DNA and amino acid sequences.

- The python scripts view identical sequences as sequences that share the same sample name and have the exact same DNA sequence. The script will remove the sample with the lower read count while retaining the highest-scoring unique sequences.  

    
- The fasta should be formatted as so:  
sample_gene_exon_readcount  
The script assumes the fields, all separated by "_".  
The first three fields can be in any order, read count must be the fourth field after the 3rd underscore.

- Test files are included with the repository. This is how you run the script:  
python Allele_Cleaner.py -f TEST.fas  
The pre-cleaned test file should contain 164 sequences, once cleaned it should have 82 sequences.


- Help command python Allele_Cleaner.py -h

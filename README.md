# Allele_Cleaner
  
- Uses biopython version 1.81
- This script takes a fasta file, and removes redundant sequences.  
- This script was designed for the purpose of removing redundant amino acids sequences that appeared after translating synonymous snips in nucleotide sequences.
- The script will still work regardless if the fasta contains nucleotides, or amino acids.

- The script will sequences with matching names and compare there sequences, if the sequences are a perfect match then the sequence with the lower read count is removed.  
- If the sequences don't match both sequences will be kept.

- This script assumes the fields, all separated by "_," with the fourth field being the read count.
- The expected naming scheme convention is this:
ARA08_MP4_Exon1_992_A1
992 is the read count
  

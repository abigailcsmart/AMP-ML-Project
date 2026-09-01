# Deep Learning University Project
*Multi-Kernel 1D CNN model*

Antimicrobial peptides (AMPs) are short chains of amino acids, typically around 5
to 50 residues long, that can inhibit or kill microorganisms such as bacteria, fungi,
viruses, and parasites. Many AMPs are part of the innate immune system in
animals, plants, and microorganisms. They often act by disrupting microbial cell
membranes, interfering with intracellular targets, or modulating immune
responses. Because of their broad antimicrobial activity and their potential to
reduce the risk of conventional antibiotic resistance, AMPs are considered
promising candidates for developing new anti-infective therapies.

In computational biology, peptide sequences are commonly represented using
standard single-letter amino acid codes, often in FASTA format. Since there are 20
standard amino acids, the number of possible peptide sequences increases
exponentially with sequence length. This makes experimental screening of all
possible AMPs impractical. Machine learning and deep learning models can help
by learning sequence patterns associated with antimicrobial activity and
predicting whether a new peptide is likely to be antimicrobial.

In this project, I was required to develop a machine learning or deep learning
model that predicts whether a peptide has antimicrobial activity based on its
amino acid sequence in the FASTA column. A CSV file, peptides.csv, is provided for
both model development and evaluation. The file contains two columns: FASTA,
which contains the peptide amino acid sequences using standard single-letter
amino acid codes, and Label, where 1 indicates an antimicrobial peptide (AMP)
and 0 indicates a non-AMP

After further review, I came to see that I mistakenly used the test set for tuning purposes, when I should have compared my different models on the validation set only. After selecting my final model based on the stopping criterion, I should have retrained it on the train and valid dataset then evaluated it on the test set.

# Needleman-Wunsch Algorithm Implementation in Perl

This Perl script implements the Needleman-Wunsch algorithm for global sequence alignment without gaps. The algorithm is a foundational method in bioinformatics for aligning protein or nucleotide sequences.

https://en.wikipedia.org/wiki/Needleman%E2%80%93Wunsch_algorithm

## Features

- Global alignment of two input sequences.
- Customizable scoring with match, mismatch, and indel values.
- Outputs the alignment score and the similarity matrix to a file.

## Prerequisites

Ensure you have Perl installed on your system. This script was written and tested with Perl 5, but should be compatible with most recent versions of Perl.

## Usage

To run the script, make it executable or invoke it through the Perl interpreter:

```bash
chmod +x needleman_wunsch.pl
./needleman_wunsch.pl
# or
perl needleman_wunsch.pl
```
## Input Format

The program expects numeric input for match value, mismatch cost, and indel cost. Sequences should be provided as strings of characters without spaces or special characters (except for sequence-related characters like A, T, C, G for DNA, or amino acid single-letter codes for proteins).

```bash
Input match value:
1
Input mismatch cost:
1
Input indel cost:
1
Input string 1:
ACTG
Input string 2:
ACGT
```

## Ouput 

The output is directed to a file named outer. It contains:

- The individual characters of the input strings.
- The value matrix 'V' with calculated scores.
- The final similarity value of the two strings.
- The maximum value observed during the alignment process.

## Author 
- Harrison Heath 


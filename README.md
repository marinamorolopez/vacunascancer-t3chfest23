# Cancer vaccine design with Python
Python tool developed for the T3chFest 2023 talk "Designing cancer vaccines with Python".
This project demonstrates how Python can be used to automate simple molecular biology workflows by generating CRISPR editing templates from DNA sequences.

## Features
- Load DNA sequences from FASTA files
- Simulate knock-in and knock-out mutations
- Generate guide RNA sequences
- Generate donor DNA templates
- Export mutated DNA sequences automatically

## Installation
You simply have to download the .py and fasta files (or get your own fasta files from a database as [NCBI](https://www.ncbi.nlm.nih.gov/)).

## Usage
Run the script and select:
1. The DNA sequence of the gene of interest.
2. The type of mutation (knock-out or knock-in)

For a knock-in, choose between:
- Single-base substitution
  - Enter the mutation position
  - Specify the new nucleotide (A, T, C or G)
- Whole-gene insertion
  - Select the FASTA file containing the DNA sequence to be inserted

Once the analysis is complete, the program generates three output files:
- guideRNA.txt
- donorDNA.txt
- mutated_sequence.txt

## Example
Input
```
Gene: TP53
Mutation: Knock-in
Position: 125
Base: A
```
Output
```
guideRNA.txt
donorDNA.txt
mutated_sequence.txt
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)

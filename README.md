## How to use the snp_fasta.py
This script adds entries to an existing fasta. All missense SNPs from the mutations.csv file are searched and a number of AA before and after the SNP are added.

1. Get the mutations file

Look for your cell line of interest on [DepMap](https://depmap.org/portal/) and download the mutations.csv file.

2. Install needed packages:
```bash
pip install SeqIO
```
3. Run the python script:

For example, run the code with the following arguments:
- fasta file: test.fasta
- mutations file: mutations.csv
- number of AAs before and after the mutation: 15
- output fasta: MUT_test.fasta

```bash
python --fasta_file test.fasta --snp_file mutations.csv --num_aa 15 --output_file MUT_test.fasta
```

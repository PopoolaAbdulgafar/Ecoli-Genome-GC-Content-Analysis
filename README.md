 Genome-Wide GC Content Analysis of Escherichia coli

Overview

This project analyzes the nucleotide composition and genome-wide GC content of the Escherichia coli genome using Python and Biopython.

The analysis combines whole-genome nucleotide composition with a sliding-window approach to examine how GC content varies across different regions of the genome.

Objectives

- Calculate the genome length and nucleotide composition.
- Determine the overall AT and GC content.
- Analyze GC content using a sliding-window approach.
- Examine local variation in GC content across the genome.
- Calculate the AT/GC ratio across genomic regions.
- Visualize the distribution and genomic pattern of GC content.
- Save the analysis results as CSV files and publication-quality PNG figures.

Dataset

Organism: Escherichia coli
Input file: "Sequence.fasta"
Genome length: 4,641,652 bp
Window size: 1,000 bp
Step size: 100 bp

Methodology

The genome sequence was loaded from the FASTA file using Biopython's "SeqIO" module.

The nucleotide composition was calculated by determining the number and percentage of adenine (A), thymine (T), guanine (G), and cytosine (C) bases.

A sliding-window analysis was then performed using a 1,000 bp window with a 100 bp step size. For each window, GC content, AT content, and the AT/GC ratio were calculated.

A total of 46,407 genomic windows were analyzed.

Key Results

The E. coli genome had an overall GC content of approximately 50.79% and an AT content of 49.21%.

The sliding-window analysis showed that GC content varied from 27.40% to 69.90%, with a mean of 50.79% and a standard deviation of 4.78%.

The mean AT/GC ratio was 0.989, indicating an overall near-balanced AT and GC composition.

Results

The analysis generates the following files:

- "gc_sliding_window_analysis.csv" — GC content, AT content, and AT/GC ratio for each genomic window.
- "gc_statistical_summary.csv" — Statistical summary of the GC analysis.
- "nucleotide_composition.csv" — Nucleotide counts and percentages.
- "genome_wide_gc_content.png" — Genome-wide GC content plot.
- "at_gc_ratio.png" — Genome-wide AT/GC ratio plot.
- "gc_content_histogram.png" — Distribution of GC content across genomic windows.

Project Structure

ecoli-genome-gc-content-analysis/
├── README.md
├── gc_ecoli_content.ipynb
├── Sequence.fasta
└── results/
    ├── gc_sliding_window_analysis.csv
    ├── gc_statistical_summary.csv
    ├── nucleotide_composition.csv
    ├── genome_wide_gc_content.png
    ├── at_gc_ratio.png
    └── gc_content_histogram.png

Tools Used

- Python
- Biopython
- NumPy
- Pandas
- Matplotlib
- JupyterLab

Biological Interpretation

The genome has an overall GC content of approximately 50.79%, indicating a relatively balanced AT/GC composition.

However, the sliding-window analysis revealed substantial local variation in GC content across the genome, with some regions having considerably lower or higher GC content than the genome-wide average.

This demonstrates that examining local GC composition can provide more information about genome organization than relying only on the overall GC percentage.

Reproducibility

The analysis can be reproduced by installing the required Python packages:

pip install biopython numpy pandas matplotlib

The notebook "gc_ecoli_content.ipynb" contains the complete analysis workflow and can be executed from beginning to end in JupyterLab.

Author

Popoola Abdulgafar

Bioinformatics | Genomics | Python | NGS Analysis

License

This project is intended for educational and portfolio purposes.

#This project demonstrates practical application of computational techniques in genomics and highlights the importance of GC content analysis in understanding bacterial genome structure.




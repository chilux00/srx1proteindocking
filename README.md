# SRX1 Protein Docking to TSA1/2 Paralogs
Protein docking simulation of SRX1 to TSA1/2 paralogs in S. cerevisiae using Colab Alphafold and RoseTTAFold deep learning. 


## 🧬 RoseTTAFold Local Prediction Workflow

```mermaid
flowchart TD
    A[Input FASTA sequence] --> B[Generate MSA using ColabFold or AlphaFold]
    B --> C[Download A3M alignment file]
    C --> D[Run RoseTTAFold locally with predict_complex script]
    D --> E[Output predicted structure PDB and confidence NPZ]
```

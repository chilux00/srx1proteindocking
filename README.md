# SRX1 Protein Docking to TSA1/2 Paralogs
Protein docking simulation of SRX1 to TSA1/2 paralogs in S. cerevisiae using Colab Alphafold and RoseTTAFold deep learning. 


## 🧬 RoseTTAFold Local Prediction Workflow

```mermaid
flowchart LR
    A[FASTA sequence] --> B[Generate MSA (.a3m) via ColabFold / AlphaFold]
    B --> C[Download .a3m alignment]
    C --> D[Run RoseTTAFold locally with predict_complex.py]
    D --> E[Output: Predicted structure (.pdb) + confidence (.npz)]

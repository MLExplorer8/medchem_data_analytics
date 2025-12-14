Visual Medicinal Chemistry Analysis from SMILES

This repository implements a structure-centric medicinal chemistry workflow starting from SMILES-based chemical data and experimental affinity values.
The goal is to extract interpretable SAR insights before applying machine-learning models.

The dataset contains compound identifiers, SMILES strings, and affinity values (nM), where lower affinity indicates higher potency.
Invalid SMILES and non-physical values are removed during preprocessing.

Several calculated molecular columns are derived, including pAffinity, LogP, and MMFF force-field energy, providing chemically intuitive descriptors.
Morgan fingerprints (ECFP4) are generated to encode molecular structure.

Fingerprint similarity (Tanimoto) is used to explore chemical space and identify closely related compounds.
This enables similarity heatmaps and nearest-neighbor analysis.

Visual SAR analysis includes activity histograms, LogP vs pAffinity, energy vs potency, and affinity vs lipophilicity plots.
These visualizations help distinguish lipophilicity-driven potency from genuine binding effects.

Bemis–Murcko scaffolds are extracted to identify common cores and compare potency across chemotypes.
Scaffold-level analysis highlights privileged structures within the dataset.

Activity cliffs are detected as highly similar molecule pairs showing large potency differences.
These cliffs reveal minor structural changes responsible for significant activity loss or gain.

Overall, this workflow combines SMILES-based descriptors, fingerprints, and visualization to support rational medicinal chemistry decisions.

The dataset was obtained from **(https://drugdesigndata.org/about/datasets/2028)**   
Please refer to the original source for data licensing and usage terms.

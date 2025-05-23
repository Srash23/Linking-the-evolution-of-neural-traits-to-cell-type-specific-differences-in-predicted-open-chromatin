# Circadian Behavior in Mammals

## Introduction

Circadian rhythms are intrinsic time-keeping mechanisms in organisms, regulating physiological functions such as sleep-wake cycles, metabolism, and hormonal secretion. These rhythms are governed by the suprachiasmatic nucleus (SCN) in the hypothalamus, which modulates gene expression through feedback loops of core clock genes including CLOCK, BMAL1, PER, and CRY.

This project investigates the evolutionary divergence and convergent evolution of circadian regulation in mammals by analyzing open chromatin regions in astrocytes and microglia, key glial cell types involved in circadian functions.

## Key Objectives

1. Identify evolutionary conserved and divergent chromatin accessibility regions regulating circadian genes.

2. Analyze the role of astrocytes and microglia in circadian regulation.

3. Establish correlations between chromatin accessibility and mammalian circadian behavior.

## Data & Methods

1. Phylogenetic Regression Analysis

To assess chromatin accessibility and circadian regulation across species, we applied Phylogenetic Generalized Least Squares (PGLS) models using the phylolm package.

2. Identification of Significant Peaks

We applied the Benjamini-Hochberg correction to adjust for multiple hypothesis testing. The adjusted p-values determined the significance of chromatin peaks associated with circadian traits.

3. Gene Ontology Analysis

We used GREAT (Genomic Regions Enrichment of Annotations Tool) to determine whether significantly associated chromatin regions were enriched in known biological pathways.

4. Open Chromatin Accessibility Analysis

We visualized chromatin accessibility across mammalian species using Integrated Genomic Viewer (IGV) and CATlas UMAP plots.


## Key Findings

### Astrocytes

1. More significantly associated open chromatin peaks were found in astrocytes compared to microglia.

2. Two positively associated and three negatively associated peaks were identified.

**Notable peaks:**

i. hg38.chr4.148981308-148981809 (positively associated) → correlated with increased chromatin accessibility in diurnal species.

ii. hg38.chr1.15928890-15929391 (negatively associated) → decreased accessibility in nocturnal species.

**Nearest genes:**

i. EDNRA – Endothelin receptor involved in vascular function.

ii. NR3C2 – Mineralocorticoid receptor linked to stress response.


### Microglia

1. Fewer significant chromatin regions were associated with circadian traits.

2. One positively associated peak identified: hg38.chr12.56152313-56152814.

**Nearest genes:**

i. MYL6B – Myosin light chain involved in structural integrity.

ii. ESYT1 – Membrane tethering protein with potential circadian regulation.

## Comparison Between Astrocytes and Microglia

1. Astrocytes exhibit a greater role in circadian regulation compared to microglia.

2. Chromatin accessibility differences suggest astrocytes may be more central in regulating circadian cycles.

3. Microglia show potential secondary roles, possibly in neuroinflammatory responses affecting circadian mechanisms.

## Conclusion

1. Astrocytes play a significant role in circadian regulation, with conserved open chromatin regions across species.

2. Microglia exhibit limited but potentially significant interactions with circadian regulation, mainly through neuroinflammatory mechanisms.

3. Chromatin accessibility data provides insight into how circadian behaviors evolved in mammals, reinforcing the importance of astrocytic regulation in maintaining circadian cycles.

## Future Directions

1. Further investigation into functional validation of identified regulatory elements.

2. Expansion of datasets to include more species for deeper evolutionary insights.

3. Experimental confirmation of regulatory interactions using ATAC-seq or ChIP-seq.

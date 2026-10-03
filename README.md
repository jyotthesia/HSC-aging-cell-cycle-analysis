# Age-Associated Cell-Cycle Changes in Hematopoietic Stem Cells

## Overview

Re-analysis of single-cell RNA-seq data from GSE59114 to investigate age-associated changes in cell-cycle states of hematopoietic stem and progenitor cells.

## Biological Question

Does aging alter the distribution of cells across G0, G1/S, and G2/M phases in LT-HSCs, ST-HSCs, and MPPs?

## Dataset

Kowalczyk et al. (2015)
GEO: GSE59114
Species: Mus musculus
Data type: single-cell RNA-seq

## Analysis

1. Data preprocessing
2. Cell metadata extraction
3. G1/S and G2/M signature scoring
4. k-means cell-cycle classification
5. Young vs. old comparison
6. Cell-cycle regulator analysis in G0 LT-HSCs
7. Statistical testing and visualization

## Key Findings

- LT-HSCs show the clearest age-associated change in cell-cycle composition. The proportion of cells classified as G1/S decreased from approximately 21% in young LT-HSCs to 7% in old LT-HSCs, with a corresponding increase in the G0/non-cycling fraction.
- The same direction of change was observed in ST-HSCs, but the effect was weaker. G1/S cells decreased from approximately 14% to 10%, without a statistically significant difference in this analysis.
- MPP cell-cycle composition showed no clear age-associated difference. MPPs remained more proliferative than LT-/ST-HSCs, with approximately 36% vs. 41% of cells classified as G1/S in young and old groups, respectively.
- G0-defined LT-HSCs showed age-associated differences in several cell-cycle regulators. Nominal differences included lower Ccnd2 and Cdk5rap1, and higher Cdkn1a and Cdkn2c expression in old cells.
- The analysis supports an age-associated alteration in LT-HSC cell-cycle regulation, but does not establish a causal mechanism or directly measure cell-cycle transit time.

## Limitations

- Cell-level statistical tests do not provide formal mouse-level inference.
- The cell-cycle signatures are based on published gene sets rather than being learned specifically from this dataset.
- k-means classification forces cells into three discrete states and does not fully represent the continuous nature of cell-cycle progression.
- Cell-cycle phase proportions do not directly measure cell-cycle transit times.
- The G0 cyclin/CDK analysis is exploratory and does not establish mechanistic causality.

## Tools

- R
- ggplot2
- openxlsx
- knitr
- R Markdown

## References

Kowalczyk MS, Tirosh I, Heckl D, et al.
Single-cell RNA-seq reveals changes in cell cycle and differentiation
state during aging of hematopoietic stem cells.
Cell Stem Cell. 2015.

GEO accession: GSE59114.

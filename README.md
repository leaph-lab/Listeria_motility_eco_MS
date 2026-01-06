# Listeria_motility_eco_MS
Code used to replicate data analyses in the manuscruipt 'Motile and non-motile _Listeria_ species adopt distinct genomic and ecological strategies to achieve broad geographic range in soil.'

## Required Python packages
- numpy
- pandas
- mpl_toolkits.basemap
- matplotlib
- numpy
- csv
- shapefile
- os
- collections
- seaborn
- statannotations
- collections
- scipy
- statsmodels
- scikit-learn
- rpy2

## Required R packages
- vegan

> [!NOTE]
> For running the R code in the Jupyter notebook install ```rpy2``` package using ```pip install rpy2```
> - Use the command ```%load_ext rpy2.ipython``` for using this library before executing the R code in the python notebook
> - Ensure your R and Python environments are correctly configured and that ```rpy2``` can access R.
> - For any R code execution directly in the notebook, make sure to include the appropriate ```%R``` or ```%%R``` syntax when working with the ```rpy2``` extension.

## Structure
```Listeria_motility_eco_MS.ipynb```: The code used for analysis and to generate the plots in Figs. 1a-b, 1e-g, 2a–g, 3a-f, 4a, 4c-d, and Supplementary Figs. 1-8.

The code included analysis for:\
```Fig. 1a```: Geographic distribution of _L. welshimeri_ isolates.\
```Fig. 1b```: Geographic distribution of _L. booriae_ isolates.\
```Supplementary Fig. 1a-b```: Pairwise geographic distances between isolates within major phylogroups.\
```Fig. 1e```: Pangenome sizes of _L. welshimeri_ and _L. booriae_, divided into core and accessory genomes, with predicted pangenome sizes estimated from 100 genomes per species.\
```Supplementary Fig. 2a```: Accumulation curves of the core genome and pangenome of _L. welshimeri_ and _L. booriae_.\
```Fig. 1f```: Comparison of gene richness between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 2b```: Comparison of genome size between _L. welshimeri_ and _L. booriae_.\
```Fig. 1g```: Comparison of nucleotide diversity (π) between _L. welshimeri_ and _L. booriae_.\

```Fig. 2a```: Volcano plot of COG abundance differences between species.\
```Supplementary Fig. 3```: Comparison of relative abundance of putatively functional motility genes between _L. welshimeri_ and _L. booriae_.\
```Fig. 2b```: Comparison of relative abundance of putatively functional chemotaxis genes between _L. welshimeri_ and _L. booriae_.\
```Fig. 2c```: Enrichment of COGs among core genes with evidence of PS and no homologous recombination.\
```Fig. 2d```: Enrichment of COGs among accessory genes with evidence of PS and no homologous recombination.\
```Fig. 2e```: Comparison of Shannon-Wiener diversity of KEGG pathways related to cellular processes and environmental information processing between _L. welshimeri_ and _L. booriae_.\
```Fig. 2f```: Comparison of Shannon–Wiener diversity of KEGG pathways related to genetic information processing between _L. welshimeri_ and _L. booriae_.\
```Fig. 2g```: Comparison of Shannon–Wiener diversity of KEGG pathways related to metabolism between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 4```: Comparison of Shannon–Wiener diversity of overall KEGG biological pathways between _L. welshimeri_ and _L. booriae_.\

```Supplementary Fig. 5a```: Volcano plot of abiotic factors showing fold change versus statistical significance.\
```Supplementary Fig. 5b```: Volcano plot of relative abundance of bacterial phyla showing fold change versus statistical significance.

```Supplementary Fig. 6a```: Multidimensional scaling (MDS) analysis of genomes based on abiotic conditions.\
```Supplementary Fig. 6b```: MDS analysis of genomes based on bacterial community composition using weighted UniFrac distances derived from OTUs.

```Fig. 3a```: Venn diagrams from variation partitioning analysis (VPA) showing the proportion of overall gene richness variation explained by soil properties, climate, and surrounding land use for _L. welshimeri_ and _L. booriae_.\
```Fig. 3b```: Variation in gene richness of COG categories explained by abiotic factors in _L. welshimeri_ and _L. booriae_.\
```Fig. 3c```: Spearman’s correlations between abiotic factors and gene richness, both overall and for COGs, for _L. booriae_ only.\
```Supplementary Fig. 7a```: Spearman’s correlations between abiotic factors and gene richness, both overall and for COGs, for _L. welshimeri_ only.\
```Fig. 3d```: Venn diagrams from VPA showing the proportion of gene richness variation explained by abiotic and biotic factors for _L. welshimeri_ and _L. booriae_.\
```Fig. 3e```: Variation in gene richness of COG categories explained by both abiotic and biotic factors in _L. welshimeri_ and _L. booriae_.\
```Fig. 3f```: Spearman’s correlations between the relative abundance of bacterial phyla and gene richness, both overall and for COGs, for _L. booriae_ only.\
```Supplementary Fig. 7b```: Spearman’s correlation between relative abundance of bacterial phyla and gene richness, both overall and for COGs, for _L. welshimeri_ only.

```Fig. 4a```: Relationship between average nucleotide identity (ANI) and geographic distances in _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 8```: Relationship between gene presence/absence–based Jaccard similarity and geographic distance in _L. welshimeri_ and _L. booriae_.\
```Fig. 4c```: Pairwise ANI comparisons between soil and wildlife isolates of _L. welshimeri_.\
```Fig. 4d```: Comparison of genome size, gene richness, and GC content between monophyletic soil and wildlife _L. welshimeri_ isolates.\

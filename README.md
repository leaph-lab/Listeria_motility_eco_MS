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
```Supplementary Fig. 1a```: Pairwise geographic distances between isolates within major clade of each species.\
```Supplementary Fig. 1b```: Mean pairwise geographic distances between isolates across major clades compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 1e```: Pangenome sizes of _L. welshimeri_ and _L. booriae_, divided into core and accessory genomes, with predicted pangenome sizes estimated from 100 genomes per species.\
```Supplementary Fig. 2a```: Accumulation curves of the core genome and pangenome of _L. welshimeri_ and _L. booriae_.\
```Fig. 1f```: Gene richness compared between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 2b```: Genome sizes of isolates compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 1g```: Nucleotide diversity (π) compared between between _L. welshimeri_ and _L. booriae_.

```Fig. 2a```: Volcano plot of COG abundance differences between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 3```: Relative abundance of putatively functional motility genes compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 2b```: Relative abundance of putatively functional chemotaxis genes compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 2c```: Enrichment of COGs among core genes with evidence of positive selection.\
```Fig. 2d```: Enrichment of COGs among accessory genes with evidence of positive selection.\
```Fig. 2e```: Shannon-Wiener diversity of KEGG pathways compared between _L. welshimeri_ and _L. booriae_ for cellular processes.\
```Fig. 2f```: Shannon-Wiener diversity of KEGG pathways compared between _L. welshimeri_ and _L. booriae_ for environmental information processing.\
```Fig. 2g```: Shannon-Wiener diversity of KEGG pathways compared between _L. welshimeri_ and _L. booriae_ for genetic information processing.\
```Fig. 2h```: Shannon-Wiener diversity of KEGG pathways compared between _L. welshimeri_ and _L. booriae_ for metabolism.\
```Supplementary Fig. 4```: Shannon-Wiener diversity of overall biological pathways compared between _L. welshimeri_ and _L. booriae_.

```Supplementary Fig. 5a```: Volcano plot showing fold change (x-axis) versus statistical significance (y-axis, adjusted two-sided MW _U_ test) for abiotic factors.\
```Supplementary Fig. 5b```: Volcano plot showing fold change (x-axis) versus statistical significance (y-axis, adjusted two-sided MW _U_ test) for relative abundance of bacterial phyla.

```Supplementary Fig. 6a```: Multidimensional scaling (MDS) analysis of genomes based on Euclidean distances of abiotic factors.\
```Supplementary Fig. 6b```: MDS analysis of genomes based on weighted UniFrac distances of bacterial community composition derived from OTUs.

```Fig. 3a```: Venn diagrams from variation partitioning analysis (VPA) showing the proportion of overall gene richness variation explained by soil properties, climate, and surrounding land use for _L. welshimeri_ and _L. booriae_.\
```Fig. 3b```: Variation in gene richness of COG categories explained by abiotic factors based on VPA.\
```Fig. 3c```: Spearman’s correlations between abiotic factors and gene richness, both overall and for COGs, in _L. booriae_.\
```Supplementary Fig. 7a```: Spearman’s correlations between abiotic factors and gene richness, both overall and for COGs, in _L. welshimeri_.\
```Fig. 3d```: Venn diagrams from VPA showing the proportion of gene richness variation explained by abiotic and biotic factors for _L. welshimeri_ and _L. booriae_.\
```Fig. 3e```: Variation in gene richness of COG categories individually explained by biotic factors based on VPA.\
```Fig. 3f```: Spearman’s correlations between the relative abundance of bacterial phyla and gene richness, both overall and for COGs, in _L. booriae_.\
```Supplementary Fig. 7b```: Spearman’s correlation between relative abundance of bacterial phyla and gene richness, both overall and for COGs, in _L. welshimeri_.

```Fig. 4a```: Distance-decay relationship in _L. welshimeri_ and _L. booriae_ inferred by the linear regression for genetic similarities measured by average nucleotide identity (ANI) and geographic distances.\
```Supplementary Fig. 8```: Distance-decay relationship in _L. welshimeri_ and _L. booriae_ inferred by the linear regression for genetic similarities measured by Jaccard similarity of gene absence/presence and geographic distances.\
```Fig. 4c```: Pairwise ANI comparisons between soil and wild bird isolates of _L. welshimeri_.\
```Fig. 4d```: Genome size, gene richness, and GC content compared between monophyletic soil and wild bird _L. welshimeri_ isolates.

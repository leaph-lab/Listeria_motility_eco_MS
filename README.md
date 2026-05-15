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
```Listeria_motility_eco_MS.ipynb```: The code used for analysis and to generate the plots in Figs. 1A-B, 1E-G, 2A–H, 2J-K, 3A-F, 4A-G, and Supplementary Figs. 1-15.

The code included analysis for:\
```Fig. 1A```: Geographic distribution of _L. welshimeri_ isolates.\
```Fig. 1B```: Geographic distribution of _L. booriae_ isolates.\
```Supplementary Fig. 1A```: Pairwise geographic distances between isolates within major clade of each species.\
```Supplementary Fig. 1B```: Mean pairwise geographic distances between isolates across major clades compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 1E```: Pangenome sizes of _L. welshimeri_ and _L. booriae_, divided into core and accessory genomes, with predicted pangenome sizes estimated from 100 genomes per species.\
```Supplementary Fig. 2A```: Accumulation curves of the core genome and pangenome of _L. welshimeri_ and _L. booriae_.\
```Fig. 1F```: Gene richness compared between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 2B```: Genome sizes of isolates compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 1G```: Nucleotide diversity (π) compared between between _L. welshimeri_ and _L. booriae_.

```Fig. 2A```: Volcano plot of COG abundance differences between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 3```: Relative abundance of putatively functional motility genes compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 2B```: Relative abundance of putatively functional chemotaxis genes compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 2C```: Enrichment of COGs among core genes with evidence of positive selection.\
```Fig. 2D```: Enrichment of COGs among accessory genes with evidence of positive selection.\
```Fig. 2E```: Shannon-Wiener diversity of KEGG pathways compared between _L. welshimeri_ and _L. booriae_ for cellular processes.\
```Fig. 2F```: Shannon-Wiener diversity of KEGG pathways compared between _L. welshimeri_ and _L. booriae_ for environmental information processing.\
```Fig. 2G```: Shannon-Wiener diversity of KEGG pathways compared between _L. welshimeri_ and _L. booriae_ for genetic information processing.\
```Fig. 2H```: Shannon-Wiener diversity of KEGG pathways compared between _L. welshimeri_ and _L. booriae_ for metabolism.\
```Supplementary Fig. 4A```: KEGG pathway subgroup abundance compared between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 4B```: KEGG pathway subgroup diversity compared between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 5```: Shannon-Wiener diversity of overall biological pathways compared between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 6A```: KEGG ortholog (KO) annotations shared between _L. welshimeri_ and _L. booriae_ for core genome.\
```Supplementary Fig. 6B```: KO annotations shared between _L. welshimeri_ and _L. booriae_ for accessory genome.\
```Supplementary Fig. 7```: Distribution of essential nutrient requirements predicted in _L. welshimeri_ and _L. booriae_.\
```Fig. 2J```: Total number of utilizable substrates compared between _L. welshimeri_ and _L. booriae_.\
```Fig. 2K```: Proportional differences in utilizable substrates between _L. welshimeri_ and _L. booriae_.\

```Supplementary Fig. 8A```: Abiotic environmental factors compared between _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 8B```: Relative abundance of bacterial phyla compared between _L. welshimeri_ and _L. booriae_.

```Supplementary Fig. 9A```: Multidimensional scaling (MDS) analysis of genomes based on Euclidean distances of abiotic factors.\
```Supplementary Fig. 9B```: MDS analysis of genomes based on weighted UniFrac distances of bacterial community composition derived from OTUs.

```Fig. 3A```: Venn diagrams from variation partitioning analysis (VPA) showing the proportion of overall gene richness variation explained by soil properties, climate, and surrounding land use for _L. welshimeri_ and _L. booriae_.\
```Fig. 3B```: Variation in gene richness of COG categories explained by abiotic factors based on VPA.\
```Fig. 3C```: Spearman’s correlations between abiotic factors and gene richness, both overall and for COGs, in _L. booriae_.\
```Supplementary Fig. 10```: Spearman’s correlations between abiotic factors and gene richness, both overall and for COGs, in _L. welshimeri_.\
```Fig. 3D```: Venn diagrams from VPA showing the proportion of gene richness variation explained by abiotic and biotic factors for _L. welshimeri_ and _L. booriae_.\
```Supplementary Fig. 11A```: Shannon-Wiener diversity compared between sites where _L. welshimeri_ and _L. booriae_ were isolated.\
```Supplementary Fig. 11B```: Pielou’s evenness compared between sites where _L. welshimeri_ and _L. booriae_ were isolated.\
```Fig. 3E```: Variation in gene richness of COG categories individually explained by biotic factors based on VPA.\
```Fig. 3F```: Spearman’s correlations between the relative abundance of bacterial phyla and gene richness, both overall and for COGs, in _L. booriae_.\
```Supplementary Fig. 12```: Spearman’s correlation between relative abundance of bacterial phyla and gene richness, both overall and for COGs, in _L. welshimeri_.

```Fig. 4A```: Distance-decay relationship in _L. welshimeri_ inferred by the linear regression for genetic similarities measured by average nucleotide identity (ANI) and geographic distances.\
```Fig. 4B```: Distance-decay relationship in _L. booriae_ for genetic similarities and geographic distances.\
```Supplementary Fig. 13```: Distance-decay relationship in _L. welshimeri_ and _L. booriae_ inferred by the linear regression for genetic similarities measured by Jaccard similarity of gene absence/presence and geographic distances.\
```Fig. 4C```: Landscape resistance surfaces representing wildlife connectivity for large mammals.\
```Fig. 4D```: Landscape resistance surfaces representing wildlife connectivity for small mammals.\
```Fig. 4E```: Landscape resistance surfaces representing wildlife connectivity for regional-terrestrial birds.\
```Fig. 4F```: Landscape resistance surfaces representing wildlife connectivity for continental-aquatic birds.\
```Fig. 4G```: _R_<sup>2</sup> from linear regressions between genomic difference (1 - ANI) and resistance distance for each wildlife connectivity models.\
```Supplementary Fig. 14```: Comparison between soil and wild bird _L. welshimeri_ isolates.

```Supplementary Fig. 15```: Comparison of abiotic environmental factors between sites positive and negative for _L. welshimeri_ and _L. booriae_.

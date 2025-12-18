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
```Listeria_motility_eco_MS.ipynb```: The code used for analysis and to generate the plots in Figs. 1a-b, 1e-f, 2a–f, 3a-f, 4a, 4c-d, and Supplementary Figs. 1-6.

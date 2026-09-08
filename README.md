# AMR-prediction-and-finding-resistance-genes
1.Collection of MIC data from BV BRC of Klebsiella pneumoniae for 3 drugs - Ciprofloacin, Meropenem, Colistin.
2.Counting 11-mers of the genomes of different strains of Klebsiella pneumoniae to make a sparse matrix.
3.Feature engineering like making lineage maps and epistasis matrix to take make sure there is no data leakage between the cross validation stages and taking into account the multiple gene interaction that cause resistance.
4.Applying different ML algorithms and balanced weights due to the skewed nature of the dataset, with susceptile samples as majority, to see which gives the best PR-AUC.
5.Analysing the shortcomings of the models to find which genes it failed to predict correctly i.e. finding out the very major errors (resistance predicted as susceptible), to find potential novel targets.

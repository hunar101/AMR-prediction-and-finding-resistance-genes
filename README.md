# AMR-prediction-and-finding-resistance-genes
1.Collection of MIC data from BV BRC of Klebsiella pneumoniae for 3 drugs - Ciprofloacin, Meropenem, Colistin.

2.Counting 11-mers of the genomes of different strains of Klebsiella pneumoniae to make a sparse matrix.

3.Feature engineering like making lineage maps and epistasis matrix to take make sure there is no data leakage between the cross validation stages and taking into account the multiple gene interaction that cause resistance.

4.Applying different ML algorithms and balanced weights due to the skewed nature of the dataset, with susceptile samples as majority, to see which gives the best PR-AUC.

5.Analysing the shortcomings of the models to find which genes it failed to predict correctly i.e. finding out the very major errors (resistance predicted as susceptible), to find potential novel targets.

6.Because of hash collisions there was more than one candidate sequence for each hash, and these were aligned with the K. pneumoniae strain HS11286 reference genome in order to determine the dominant coding-region k-mer. 

7.Coordinates from GFF files were utilized to obtain the whole coding sequence that corresponds to the particular locus.
This gave thousands of sequences containing potential resistant factors for each drug.

8.The candidate genes were cross-matched with the CARD database to separate out the AMR-related genes from the hypothetical/putative genes along with this non – coding hit were also dropped. This reduced thousands of matches to potential coding sequences.

9.Sequences were selected and their protein sequence were subjected to BLASTp analysis  and verification. 


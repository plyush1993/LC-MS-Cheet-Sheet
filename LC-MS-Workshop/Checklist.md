# LC-MS-Workshop Checklist

### Converting Data
- MS-Covert (used parameters)

### Raw Data
- El-Maven for target compound EIC among samples
     - target list
- Library Search EIC & Integration
- Observe MS1/MS2/rt
- Query for spectra search / *in-silico* prediction in qry4ms

### Identification
- Spectral Similarity Search (GNPS, MEtaboAnalyst, etc)
- *In-silico* prediction (SIRIUS, MS-Finder, etc)

### Downstream Analysis
- Target Analysis
     - El-Maven
          - target list
     - MzMine
          - target list
- Untargeted Analysis (several samples/replicates + blanks)
     - mzMine *(Peak Table & mgf Generating)*
     - MetaboCensoR *(Filtering Redundant Features in Peak Table & mgf)*
     - SIRIUS *(In-silico Identification, Fragment Annotation)*
     - GNPS *(Molecular Networking, Spectral Similarity Search)*
          - metadata
     - Cytoscape *(Customize Networking, combine with SIRIUS)*
- Untargeted Analysis (one sample only)
     - SIRIUS *(In-silico Identification, Fragment Annotation)*
     - GNPS *(Molecular Networking, Spectral Similarity Search)*
          - metadata if with blank 
- Statistical Analysis
     - Prepare table for MetaboAnalyst
     - Univariate (MetaboAnalyst, Metabocano)
          - Volcano Plot
          - Statistical Tests for Comparing Means
          - Fold Change Analysis
          - Correlation Heatmaps
          - ANOVA (for multiple groups)
     - Multivariate (MetaboAnalyst)
          - Classification Models (RF, SVM)
          - Chemometrics (PCA, PLS)
          - Cluster Analysis (Dendrogram, Heatmaps, *k*-means, SOM)

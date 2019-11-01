# Practical: Biological databases, data repositories and basics of data processing

In this practical you will learn how to use repositories of public omics data and how to process and interpret such data and its quality. 
You will compute a list of differentially expressed genes for a transcriptomics experiment related to thyroid hyperplasia and cancer. 
Also, you will consult databases with biological knowledge to find out about the properties and functions of genes and metabolites. 
Next week, in practical 4, you will apply pathway and network analysis to further biologically interpret the outcome of the experiment.

## Part I: Consulting omics repositories: ArrayExpress

One of the databases that contains data generated from experiments is [ArrayExpress](https://www.ebi.ac.uk/arrayexpress/). Besides the data itself, 
this database contains information on the setup of the experiment itself and on the different samples that were generated (called 
metadata). This additional information is required to understand and interpret the generated data as well as to be able to reuse it.

Open ArrayExpress and find the experiment with identifier E-GEOD-54958 using the search box.
Now consult the information on this experiment and answer the following question:

1)	What is the title of the experiment?

2)	In which year was this data set released?

3)	Which platform was used to generate this data (microarray, sequencing) and which brand and type?

4)	Which experimental groups were compared in the experiment?

5)	Open the detailed information at ‘Protocols’. Which amount of RNA (in μg) was used for each sample?

6)	Open the detailed information at ‘Samples’. How many samples were in each of the experimental groups?

7)	For each sample ‘raw’ and ‘processed’ data are available. What is the difference (without opening them, you cannot open the raw data)?

8)	Open the normalised data for one sample. What information is in the two columns it contains?

## Part II: Processing publicly available data: quality control using ArrayAnalysis.org
 
1)	Open the boxplot of raw signal intensities per sample (‘RawDataBoxplot.png’). What does this tell you about the data quality?

2)	Open the boxplot of normalised signal intensities. What does this tell you about the data quality?

3)	Open the density plot of normalised signal intensities. Explain what this tells you.

4)	Open the cluster plot. What does this show about the samples?
 
5)	Open the array-array correlation plot. What does this indicate?

6)	Open the principal component analysis (PCA) plot. What does this show about the samples?

## Part III: Processing publicly available data: statistics using ArrayAnalysis.org
We have also applied the ArrayAnalysis.org workflow to generate statistical results based on the data from this experiment. In order to 
do so, one has to first determine which groups one wants to compare.

If we name (as on the QC plots):
•	PTC_mut = PTC with BRAF mutation
•	PTC_wt = PTC without BRAF mutation
•	FVPTC = follicular variant of PTC
•	FA = follicular adenoma
•	TN = normal thyroid tissue

Then we  compared each group to each other group: PTC_mut versus PTC_WT; PTC_mut versus FVPTC ; PTC_mut versus FA, PTC_mut versus TN; 
PTC_wt versus FVPTC; PTC_wt versus FA; PTC_wt versus TN; FVPTC versus FA; FVPTC versus TN; FA versus TN. So ten comparisons in total. 
(I WILL PICK SOME)

HERE THE QUESTIONS: something on P value histograms, FC histograms, expected number of significant genes, and some on the table of 
statistics (most significant genes, most changed, …) 

Now we will look up some more information about the most clearly changed genes. Of course, this does not take into account the totality 
of changes observed in the data set. Next time, in practical 4, you will apply pathway and network analysis methods that allow you to 
take all results into consideration and interpret them as a whole.

## Part IV: Evaluating findings by consulting genomics databases: Ensembl

For one or two genes find something about what they do and some functional annotation

## Part V: Metabolomics

Look very briefly into (another) metabolomics data set: only open results tables from the paper and confirm how limited the number of 
identified metabolites are.

## Part VI: Finding more information about metabolites: HMDB
Look up some information about T3/T4 in HMDB

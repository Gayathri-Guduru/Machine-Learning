# Machine-Learning project on Autism Spectrum Disorder Screening

The goal of the Autism Screening and Assessment Clinic is to provide identification of Autism Spectrum Disorder (ASD) to inform intensive behavioral treatment, while addressing specific skill deficits and enhancing community inclusion.

Objective is to predict the likelihood of a person having autism using survey and demographic variables. The target variable is Class_ASD. It is a classification problem. Number of Instances (records in the data set): 704 (rows) Number of Attributes (fields within each record): 21 (columns)

I divided the provided data into scaled and unscaled categories for this dataset using PCA, a feature engineering technique, and I tested each category’s performance. Prior to performing PCA, I first removed the target column. Once the PCA was scaled, two graphs were drawn, with the first principle component explaining 4.9% of the variance and the second principle component explaining 2.6%. First principle component accounts for 89.6% of the variance in the unscaled PCA plot, while second principle component accounts for 6.5% of the variance. The overall variance was 96.1%. We can conclude that unscaled PCA perform better than scaled PCA at reducing the dimensions of the data.

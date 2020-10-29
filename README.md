# Project outlines
## Title
### Building a classification model of NGS RNA-seq data with MLseq.      
## Author
### Bo Cheng
## Overview 
### 1. In this project, I will try to use a machine learning package from Bioconductor to build a model which can predict breast cancer subtype. 
### 2. I will try to optimize model parameters and find a good classifier in MLSeq. I will also use 9 data sets from TCGA to train and test this model. six as training data, and three as testing data.
### 3. The main goal of this project is to have a taste of machine learning in R. So I may do many copy and paste, but I will give my understanding and opinions in the R notebook.
### 4. The original package line: https://www.bioconductor.org/packages/devel/bioc/vignettes/MLSeq/inst/doc/MLSeq.pdf
### 5. The original Vignettes/sample link: https://www.bioconductor.org/packages/devel/bioc/vignettes/MLInterfaces/inst/doc/MLprac2_2.pdf
## Data availability
### All data are available from [TCGA](https://portal.gdc.cancer.gov/exploration?filters=%7B%22op%22%3A%22and%22%2C%22content%22%3A%5B%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.disease_type%22%2C%22value%22%3A%5B%22ductal%20and%20lobular%20neoplasms%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.primary_site%22%2C%22value%22%3A%5B%22breast%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.program.name%22%2C%22value%22%3A%5B%22TCGA%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.project_id%22%2C%22value%22%3A%5B%22TCGA-BRCA%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.samples.sample_type%22%2C%22value%22%3A%5B%22primary%20tumor%22%5D%7D%7D%5D%7D)
### The dataset list(Case ID)
#### The Training data
* TCGA-BRCA / TCGA-AN-A046
* TCGA-BRCA / TCGA-5L-AAT1
* TCGA-BRCA / TCGA-AN-A0AK
* TCGA-BRCA / TCGA-BH-A18G
* TCGA-BRCA / TCGA-A8-A09Z
* TCGA-BRCA / TCGA-BH-A0HF

#### The testing data
* TCGA-BRCA / TCGA-AO-A128
* TCGA-BRCA / TCGA-D8-A1XK
* TCGA-BRCA / TCGA-BH-A0B6

## Milestone1
### 1.Complating "the Emulation Path" coding part;
* Complating the coding part.
* complating the construction of the clasifaction of breast cancer.

### 2.Testing the coding part;
## Milestone2
### 1.Complating "the Machine Learning Path" coding part;
### 2.Testing the coding part with the GSE96058 data set(training set).
## Before handing in
### Using the model to do the evaluation. 
## Deliverable
### I will use R MarkDown/Notebook/Jupyter to display a understandable codes.
# DVA: predicting the functional impact of single nucleotide missense variants

This repository contains codes to train DVA model and predict the functional impact of single nucleotide missense variants.

#### **Requirements:**

1) The R packages including "raster", "randomForest", "filling", "stringr".
2) The ANNOVAR datasets ([ANNOVAR Documentation (openbioinformatics.org)](https://annovar.openbioinformatics.org/en/latest/)) 
3) Linux Operating System

#### **Tutorials:**

Data: This folder will be used to store some necessary raw data and intermediate process data of DVA.

Data/ANNOVAR/annovar: This folder contains all materials and codes of ANNOVAR tool.

dvatest.txt: The Demo input dataset. If you want to predict the functional impact of other variants using DVA, the format of your input data shuold be same with "dvatest.txt"(five columns including chromosome/start site/end site/ref base/alt base). 

DVA.R: Generate DVA raw scores for input variants.

#### **Demo:**

Using the following command to download the demo:

`git lfs clone https://github.com/csdwang/DVAscore.git`

Using the following command to run the demo:

`Rscript DVA.R dvatest.txt`

Result_dvatest.txt is the output file, which includes two columns: variant(chromosome/site/ref/alt) and DVA scores.

(*)before you perform this demo, you need to download LJB(dbNSFP30a) dataset, gnomAD211 dataset, TFBS dataset, phastConsElements46way dataset, and phastConsElements100way dataset from ANNOVAR and all these data should be stored into Data/ANNOVAR/annovar/humandb/.

#### **Citation:**

DVA: predicting the functional impact of single nucleotide missense variants


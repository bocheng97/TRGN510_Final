# Milestone2
## What I've done
### 1.I use 28 datasets to training all the model offered by MLSeq, and use 12 dataset to test the model.
### 2.I find out the best model I have now is "voomNSC", which has about 75% accuracy.
### 3.The possible biomarkers I found is  [1] "ENSG00000108821.12" "ENSG00000210082.2"  "ENSG00000164692.16" "ENSG00000198804.2"  "ENSG00000115414.17" "ENSG00000168542.11" "ENSG00000115461.4"  "ENSG00000198727.2" [9] "ENSG00000111341.8"  "ENSG00000234745.8"  "ENSG00000075624.12" "ENSG00000198712.1"  "ENSG00000012223.11" "ENSG00000113140.9"  "ENSG00000198938.2"  "ENSG00000166710.16"[17] "ENSG00000204525.13" "ENSG00000198888.2"  "ENSG00000159763.3"  "ENSG00000172551.9"  "ENSG00000198899.2"  "ENSG00000160862.11" "ENSG00000189058.7"  "ENSG00000087086.12"[25] "ENSG00000206503.10" "ENSG00000133110.13" "ENSG00000133112.15" "ENSG00000100316.14" "ENSG00000111640.13" "ENSG00000175899.13" "ENSG00000070756.12" "ENSG00000197746.12"[33] "ENSG00000163359.14" "ENSG00000080824.17" "ENSG00000171345.12" "ENSG00000161016.14" "ENSG00000141424.11" "ENSG00000204287.12" "ENSG00000124942.12" "ENSG00000096384.18"[41] "ENSG00000137558.6"  "ENSG00000142192.19" "ENSG00000100345.19" "ENSG00000231500.5"  "ENSG00000179218.12" "ENSG00000149925.15" "ENSG00000074800.12" "ENSG00000164733.19"[49] "ENSG00000169710.6"  "ENSG00000135821.15" "ENSG00000196924.13" "ENSG00000149273.13" "ENSG00000142541.15" "ENSG00000137154.11" "ENSG00000163220.10" "ENSG00000096696.12"[57] "ENSG00000164919.9"  "ENSG00000115457.8"  "ENSG00000185624.13" "ENSG00000124107.5"  "ENSG00000126709.13" "ENSG00000125730.15" "ENSG00000139329.4"  "ENSG00000087460.22"[65] "ENSG00000141367.10" "ENSG00000026025.12" "ENSG00000011465.15" "ENSG00000196230.11" "ENSG00000170421.10" "ENSG00000142156.13" "ENSG00000044574.7" 
## What issues I found
### 1.I found in the vignette is the "voomDLDA" method, which has errors for now I can't solve, so I just skip this method.
### 2.Another thing is the model accuracy is low, maybe I need more dataset.
### 3.I need to convert the ensembl_ID into gene_name 
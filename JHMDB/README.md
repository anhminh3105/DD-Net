# DD-Net on JHMDB dataset

## CHANGES FROM THE ORIGINAL REPO
* Prepocess and export a subset of JHMDB dataset in terms of selected action classes
* Added weighted class for training to alleviate some skewed effects
* norm_scale() by mean and variance
* A modification of DD-Net replacing all Dropouts -> BatchNorms
* Training DD-Net on the combined 3 splits of the preprocessed dataset subset
* Ckpt saving every time the model gains val_acc

## 1. Download JHMDB dataset from 
```
http://jhmdb.is.tue.mpg.de/challenge/JHMDB/datasets  
```
(or you can directly use our preprocessed features in /data)

## 2. Using jhmdb_data_preprocessing.ipynb to preprocess JHMDB raw data.

## 3. Run jhmdb_1D.ipynb or jhmdb_1D_lite.ipynb

# Lpn-paper

## Scripts

### upsample the training data
```sh upsample.sh```  

### make the config file
```sh config-file-maker.sh```  

### run the CV-loop
```sh runner.sh```  

### compile the CV report
```sh report-maker.sh```  

### determin the best models

#### MELB-2018
```tail -n +2 report.csv | grep "MELB-2018" | sort -t ',' -k 8 -nr | head -1 | cut -f 1 -d ','```  
```grep "MELB-2018_535_SKA_align_m-0.1_k-15_p-0.1.CLIPPED.OHE_US-100_VAL-0.8_k-500_model-RFC_class_1_weight-2"$ config.csv > MELB-2018_config.csv```

#### MELB-A
```tail -n +2 report.csv | grep "MELB-A" | sort -t ',' -k 8 -nr | head -1 | cut -f 1 -d ','```  

#### MELB-G
```tail -n +2 report.csv | grep "MELB-G" | sort -t ',' -k 8 -nr | head -1 | cut -f 1 -d ','```  

#### MELB-M
```tail -n +2 report.csv | grep "MELB-M" | sort -t ',' -k 8 -nr | head -1 | cut -f 1 -d ','```  

### run model on the clinical test dataset


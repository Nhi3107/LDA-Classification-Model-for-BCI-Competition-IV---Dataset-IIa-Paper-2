## LDA Classification Model for BCI Competition IV - Dataset IIa.
### mainanalysis_dataset1.m
- BCI Competition IV—Dataset IIa was put into Matlab and proceeded to be input to the model.
- Performed preprocessing steps by filtering out high-frequency, low-frequency noise and powerline interference.
- The feature used in the model is filter banks, add more temporal information or features to a single trial.
- To run the model, we used 10-fold cross validation with one-vs-all methods. Two steps (feature selection and classification) were combined in the classification functions.

Note: 
  
  Dataset IIa: https://bnci-horizon-2020.eu/database/data-sets

This code is only part of the paper: "Optimize temporal configuration for motor imagery-based multiclass performance and its relationship with subject-specific frequency" (doi.org/10.1016/j.imu.2022.101141)

### eeg_filter.m
- Is the function used to filter noise in the preprocessing step in the script 'mainanalysis_dataset1.m'.

### Result folder
- Là kết quả mẫu khi chạy scipt 'mainanalysis_dataset1.m'.

## LDA Classification Model for BCI Competition IV - Dataset IIa.
### mainanalysis_dataset1.m
- BCI Competition IV—Dataset IIa was put into Matlab and proceeded to be input to the model.
- Performed preprocessing steps by filtering out high-frequency, low-frequency noise and powerline interference.
- The feature used in the model is filter banks, add more temporal information or features to a single trial.
- To run the model, we used 10-fold cross validation with one-vs-all methods. Two steps (feature selection and classification) were combined in the classification functions.

 #### How to run
4.	Toggling/Untoggling in Pre-processing: Let’s jump to %%PREPROCESSING, which has 4 subsections (%%1-s segment, %%1-second overlapping 0.5-second, %%2-second overlapping 1-second, %%Whole segment). Each of these subsections corresponds to each time segment type mentioned in the study. There are 2 steps to toggle/untoggle (comment/uncomment) the case:
a.	First toggling: comment/uncomment (CTRL + R or CTRL + T) all lines in a specific subsection to select/unselect the case.
b.	Second toggling: If the feature extraction method used is CSP, comment the Case 01 and uncomment Case 02, and vice versa.

5.	Toggling/Untoggling in Feature Extracting: Let’s jump to %%FEATURE EXTRACTION, which has 5 subsections (%%CSP, %%FBCSP, %%DFBCSP Fisher, %%DFBCSP mRmR, %%DFBCSP FmRmR). Each of these subsections corresponds to each feature extraction method mentioned in the study. Likewise, uncomment the intended subsection and comment other subsections. Please note: If the feature extraction method used is CSP, comment the Case 01 and uncomment Case 02 (in %%PREPROCESSING), and vice versa.


Note: 
  
  Dataset IIa: https://bnci-horizon-2020.eu/database/data-sets

This code is only part of the paper: "Optimize temporal configuration for motor imagery-based multiclass performance and its relationship with subject-specific frequency" (doi.org/10.1016/j.imu.2022.101141)

### eeg_filter.m
- Is the function used to filter noise in the preprocessing step in the script 'mainanalysis_dataset1.m'.

### Result folder
- Is a sample result when running scipt 'mainanalysis_dataset1.m'.

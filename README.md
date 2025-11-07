# ImagingNeuroscience_ReadingWhiteGrayMatterfMRI
Analysis code analyzing white- and gray-matter fMRI connectivity in relation to reading

# Inputs:
1. Behavioral dataset
2. White matter labels -- from Eve atlas
3. Gray matter labels -- from Brodman Area atlas
4. Participant white matter-gray matter functional connectivity matrices
5. Example region of interest (ROI)-based connectivity matrix and coordinates

# Analysis Steps:
1. Load behavioral dataset [Input: a]
2. Calculate descriptive statistics of behavioral variables [Table 1]
3. Load atlas labels [Inputs: b & c]
4. Load participant white matter-gray matter functional connectivity matrices [Input: d]
5. Visualize group-averaged white matter-white matter functional connectivity [Supplemental Figure 1]
6. Filter connectivity values by white matter tracts, including left uncinate fasciculus and control tracts (right uncinate fasciculus, left saggital stratum, and left cingulum)
7. Transform & collapse data across individual matrices
8. Load data for analysis, merging behavioral and functional connectivity datasets
9. Visualize distributions of reading scores and their correlation [Figure 2a + 2b]
10. Residualize white matter-gray matter functional connectivity values by covariates, includign framewise displacemenet (FD) values and demographics (handedness, age, & sex)
11. Filter Brodman Area gray matter regions of interest (ROIs) based on structural circuitry
12. Run regression, where word recognition (WJ Basic Reading) and functional connectivity interact and predict reading comprehesnion (WJ Passage Comprehension) [Table 2]
13. Visualize ROI-based connectivity matrix [Input: e] [Figure 3a]
14. Visualize interaction plots [Figure 3b]

# Outputs:
Table 1. Descriptive statistics for the sample [Step 2]
Supplementsal Figure 1. Group-averaged white matter-white matter functional connectivity matrix [Step 5]
Figure 2a. Distrbutions of reading scores [Step 8]
Figure 2b. Correlation between reading scores [Step 8]
Table 2. Findings for left uncinate fasciculus and gray matter functional connectivity interactions with reading scores [Step 12]
Figure 3a. Visualization of left uncinate fasciculus functional connectivity with gray matter structures that showed significant interactions with reading scores [Step 13]
Figure 3b. Plots of interaction effects [Step 14]

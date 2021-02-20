# FAO_Detrend


This repository contains the codes and reports used to download and temporally de-trend FAO national wheat yield time series for the USA, Germany and Morocco.

* The Analysis.Rmd file generates a report with all the code and graphs relevant to the analysis. 
The code contained in this file downloads the yield data from FAO and savesit into the Data/ folder. 
Then it uses this data to produce 3 different trend models: simple linear regression, second order polynomial regression and locally weighed regression model.
The root mean square error (RMSE) for each model and region is calculated, and the model with the lowest RMSE is chosen for the detrending analysis.
Furthermore, the detrending is done through both an additive and multiplicative decomposition approaches.

* The Report_FAO-Detrending.Rmd file generates a report summarizing the results from the Analysis.Rmd file.

* The Data/ folder contains the data downloaded from the FAO database.

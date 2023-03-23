# SWV_Nature_Geoscience

Uses Anaconda 3 and Python 3.8.8 throughout.

Jupyter-notebooks to run through key steps of the paper

Nowack et al. Response of stratospheric water vapour to global warming constrained by satellite observations. under review in Nature Geoscience (2023).

These notebooks are:

1) create_SWOOSH_time_series.ipynb

In this notebook, the SWOOSH data is pre-processed according to the description in the Methods section of the paper. For example, this concerns masking periods of missing or unreliable data, and estimating uncertainties introduced by sampling irregularities.

2) CMIP_models_ridge_training_T60NS_5plevs.ipynb

In this notebook, we run through the ridge regression analysis for all CMIP5/6 models, as described under Methods and as used for the main part of the paper (temperature predictors within 60N to 60S, five pressure levels). Parameters can easily be changed to run other calculations and tests presented in the Extended Data section and in the Supplementary Material.

3) ridge_train_on_obs_predict_cmip4xco2.ipynb

In this notebook, we first train ridge regressions on 150 pairs of reanalysis/SWOOSH data (3 reanalyses x 50 SWOOSH realisations). Afterwards, we calculate stratospheric water vapour (SWV) changes per degree global warming for 

(a) abrupt-4xCO2 for each CMIP model
(b) the CMIP-model consistent predictions using functions trained on each model's historical period data (validation of predictive skill under 4xCO2 forcing)
(c) combining the 150 observational functions with the CMIP model temperature responses.

(c) are observationally constrained 4xCO2 projections, which form a part of the overall observational constraint.

4) constraint_calculations_from_ridge_60NS.ipynb

Notebook to calculate the observational constraint on the SWV responses, in support of Figure 2 in the paper.

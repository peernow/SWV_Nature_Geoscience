# SWV_Nature_Geoscience

Uses Anaconda 3 and Python 3.8.8 throughout.

Jupyter-notebooks to run through key steps of the paper

Nowack et al. Response of stratospheric water vapour to global warming constrained by satellite observations. under review in Nature Geoscience (2023)

These notebooks are:

1) create_SWOOSH_time_series.ipynb
In this notebook, the SWOOSH data is pre-processed according to the description in the Methods section of the paper. For example, this concerns masking periods of missing or unreliable data, and estimating uncertainties introduced by sampling irregularities.

2) CMIP_models_ridge_training_T60NS_5plevs.ipynb
In this notebook, we run through the ridge regression analysis for all CMIP5/6 models, as described under Methods and as used for the main part of the paper (temperature predictors within 60N to 60S, five pressure levels). Parameters can easily be changed to run other calculations and tests presented in the Extended Data section and in the Supplementary Material.

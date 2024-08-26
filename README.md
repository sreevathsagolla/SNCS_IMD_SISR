## SNCS_IMD_SISR
### Comparative Assessment of Image Super-Resolution Techniques for Spatial Downscaling of Gridded Rainfall Data
-----

This is code for the research article that we published on [SN Computer Science](https://link.springer.com/journal/42979):
>Golla, S., Murukesh, M. & Kumar, P. Comparative Assessment of Image Super-Resolution Techniques for Spatial Downscaling of Gridded Rainfall Data. SN COMPUT. SCI. 5, 312 (2024). https://doi.org/10.1007/s42979-024-02653-3
<br>
## Repository File Structure
- **environment.txt** : Python environment file within which the code scripts were run.
- **sisr.py** : Python script with a class containing all the model-building and training functions.
- **run_x.py** : These files import the sisr.py model, and hyperparameters required for training a model 'x' are defined here.
- **MODEL_RUNS** : Folder containing model files (.h5) and training log (.csv) for each model run.
- **DATA** : Contains the testing and training data, shapefile of India and other variables (longitude, latitude, dates saved as separate variables) for plotting purposes, the bicubic interpolation output that was achieved by using CDO (RF_INTERPBIC_025_2016_2021.nc) and the mask variables (at high and low-resolutions) again for plotting purposes.
- **ANALYSIS**: This folder contains the Analysis_and_Plotting.ipynb Python file, a comma-separated sheet of error metrics, all the model outputs along with ground-truth saved as a netCDF file (SISR_Outputs.nc), Pearson correlations of each model output with ground-truth (pearsonr_all_models.npz), a field-mean of outputs and ground truth over the domain saved as a netCDF, and all the figures made from the Analysis_and_Plotting.ipynb code.

<br>

Feel free to contact me (via sreevathsa18@iiserb.ac.in [or] sreevathsa.golla@soton.ac.uk) or any of the authors if you have any questions.

**NOTE:**
Here are the files/folders that were 'gitignore'd due to space constraints:
- /MODEL_RUNS/EXP001_AUTOENC/*
- /DATA/*
- /ANALYSIS/SISR_Outputs.nc

You can download this exact repository along with the above (ignored) files from:
> Golla, Sreevathsa; Murukesh, Midhun; Kumar, Pankaj (2023). SNCS_IMD_SISR. figshare. Software. https://doi.org/10.6084/m9.figshare.22262248.v2

## To-do:

- Improve README file
- Add code usability directions
- Host 'gitignored' files 
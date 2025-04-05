# Case Study: Weather Regimes Preprocessing Sensitivity

***Repository Authors: Jhayron S. Perez-Carrasquilla and Maria J. Molina (University of Maryland, College Park)***

## How to compute weather regimes?

Weather regimes are large-scale, persistent, and recurrent atmospheric patterns useful for prediction at subseasonal timescales due to their impact on surface weather anomalies (e.g., [Molina et al., 2023](https://journals.ametsoc.org/view/journals/aies/2/2/AIES-D-22-0051.1.xml); [Perez-Carrasquilla and Molina, 2025](https://arxiv.org/abs/2409.08174)). 

These weather regimes are often defined using 500-hPa geopotential height anomalies over a specified domain (e.g., North America) and k-means clustering. 

Here, we demonstrate how seemingly minor differences in preprocessing choices can lead to a different number of preferred subseasonal weather regimes over North America with different spatial characteristics. 

Weather regimes are computed using ERA5 data that is regridded/resampled following ```0_ResampleRegridERA5.py```.

To highlight preprocessing sensitivity, we will calculate the North American weather regimes in three different ways contained in the following Jupyter Notebooks:

- ```ExpC_WRCompClean.ipynb```
- ```Exp1_StdDevOfEachPixel.ipynb```
- ```Exp2_19792023.ipynb```

## Software and Acknowledgement

The Python environment used to run associated software is contained in ```wrpreprocessing_env.yml```. 

We would like to acknowledge high-performance computing support from the Derecho system (doi:10.5065/qx9a-pg09) provided by the NSF National Center for Atmospheric Research (NCAR), sponsored by the National Science Foundation.

- Computational and Information Systems Laboratory. 2023. Derecho: HPE Cray EX System (University Community Computing). Boulder, CO: NSF National Center for Atmospheric Research. doi:10.5065/qx9a-pg09.
- Paper/preprint citation forthcoming.

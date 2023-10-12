## hot-july
Global daily 2m temperature projections

A Toy model for reference

Make sure to download and overwrite the local data from: https://climatereanalyzer.org/clim/t2_daily/json/cfsr_world_t2_day.json

Update the day numbers for a specific run (day numbers are 1-indexed: January 1 is day 1)

Note: Specific runs may take a few minutes.

## /gefs
# gefs_global_2m_temp_mean_bias_corrected-Oct.ipynb
Only use the Oct notebook (as it is the only one that calculates average temps using weighted-area).

Calculates 2m average world temps from GEFS bc (weighted area using pyproj ellipsoid projection, WGS84) and adjusts the temps to fit CFSR for the same forecast period.
Extends this adjusted GEFS forecast with prophet and more manual adjustments for rest of year.
Outputs a CFSR with forecasted temps for rest of year (for a different project: monthly-mean-land-ocean-temp)

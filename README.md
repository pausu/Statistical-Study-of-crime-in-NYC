# Statistical-Study-of-crime-in-NYC
Analysis of incident event data collected by the New York Police Department over a timespan of 18 years.  
- Arrests. NYPD arrests data (historic). https://catalog.data.gov/dataset/nypd-arrests-data-historic,   
- Shooting. NYPD shooting incident data (historic). https://catalog.data.gov/dataset/nypd-shooting-incident-data-historic  

We present an investigation on temporal and spatial patterns of census and incident public data
retrieved from the NYC Open data portal. We observe that the relative frequency of
crime events has been quite stable over the years for all neighborhoods we considered, 
and that it is possible to cluster blocks over homogeneous regions to identify the city areas which should
be considered more dangerous. The analysis is carried out using fused lasso methods, both for one- and two-dimensional data.

The results are presented in the [report](./Crime_NYC.pdf). Two appendices contain parts of the code: [App1: 1d_fusedLasso](./app1_crime_timeN.Rmd) (written in R) and in [App2: 2d_fusedLasso](./app2_crime2d.ipynb) (written in Python).

## Methodology

- analysis of temporal patterns in data using 1d fused Lasso methods with the help of R package genlasso, equiped with cross-validation function calculating the optimal regularization parameter
- analysis of spatial patterns on city maps using 2d fused Lasso methods and optimalisation techniques based on Alternating Direction Method of Multipliers
  
## Skills employed
- R: EDA, genlasso
- Python: Pandas, Geopandas, Matplotlib, Numpy, Sklearn, CVXPY

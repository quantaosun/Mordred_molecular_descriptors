# descriptor

The original paper is on https://jcheminf.biomedcentral.com/articles/10.1186/s13321-018-0258-y 

The following Binder link provides a readily installed Mordred and other tools to generate and process the calculated molecular descriptors, which can  be used in downstream machine learning model building.

## Launch Mordred from here

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/quantaosun%2Fdescriptor/HEAD?labpath=mordred.ipynb)

you could use a similar filtering code to filter those columns with values that is not a number

```
# Identify and drop columns with non-numeric values
non_numeric_columns = df.apply(pd.to_numeric, errors='coerce').isna().any()
df = df.loc[:, ~non_numeric_columns]
```



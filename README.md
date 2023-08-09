# oceanbench-data-registry
Data registry for the ocean bench project


## Conda installation:

```
conda create -n data-registry
conda activate data-registry
conda install -c conda-forge funcy=1.18 fsspec=2022.11.0 dvc-s3=2.21.0
```

## Usage
The data is stored using dvc (check documentation for more info):

To download a file:
```
dvc get https://github.com/quentinf00/oceanbench-data-registry.git osse_natl60/grid/gf_obs_nadir.nc
```

Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
Or download the data registry (very light) and pull the necessary files:
```
git clone https://github.com/quentinf00/oceanbench-data-registry.git
cd oceanbench-data-registry
dvc pull osse_natl60/grid/gf_obs_nadir.nc
```

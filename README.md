# cb-emulators
Production of figures for Carbon Brief guest post [The role 'emulator' models play in climate change projections](https://www.carbonbrief.org/guest-post-the-role-emulator-models-play-in-climate-change-projections).

## install and reproduce
You know the drill by now: `conda` is used for everything. This was tested on MacOS using Python 3.8.

```
git clone https://github.com/chrisroadmap/cb-emulators
cd cb-emulators
conda env create -f environment.yml
conda activate cb-emulators
jupyter notebook
```

then the notebooks (in `notebooks` directory) numbered 1-4 do the work. Note that notebook 2 will take time to reproduce as it generates a 100,000 member ensemble of projections from [FaIR](https://github.com/OMS-NetZero/FAIR).

## credit
Notebooks 1 and 3 made use of [`netcdf-scm`](https://gitlab.com/netcdf-scm/netcdf-scm) v2.1.1 (Nicholls et al., 2021)

Nicholls, Z, Lewis, J, Makin, M, et al. Regionally aggregated, stitched and de-drifted CMIP-climate data, processed with netCDF-SCM v2.0.0. Geosci Data J. 2021; 00: 1– 45. https://doi.org/10.1002/gdj3.113

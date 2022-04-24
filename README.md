# Southern Africa - Topography and bathymetry

A 1 arc-minute  resolution grid of topography over Southern Africa referenced to
mean sea-level.

![Southern Africa topography](preview.jpg)

| | Summary |
|--:|:--|
| File | `southern-africa-topography.nc` |
| Size | 1.70 Mb |
| Version | [v1](https://github.com/fatiando-data/southern-africa-topography/releases/latest) |
| DOI | https://doi.org/10.5281/zenodo.6481379 |
| License | [CC-BY](https://creativecommons.org/licenses/by/4.0/) |
| MD5 | `md5:609d14fe4e551c5dcf320cdceedd30e8` |
| SHA256 | `sha256:3e3878a4bdf5e2e71cb85bab9d97e4e9733caf7ab5f74c0d799154fad1b41bef` |
| Source | [ETOPO1](https://doi.org/10.7289/V5C8276M) |
| Original license | [public domain](https://ngdc.noaa.gov/mgg/global/dem_faq.html#sec-2.4) |
| Processing code | [`prepare.ipynb`](https://nbviewer.org/github/fatiando-data/southern-africa-topography/blob/main/prepare.ipynb) |

## Changes made

> These are the changes made to the original dataset.

* Crop it to a region that covers only the Southern Africa.
* Rename the coordinates to `longitude` and `latitude`.
* Rename the `xarray.DataArray` to `topography`.
* Improved metadata of the dataset following CF-conventions.

## About this repository

This is a place to format and prepare the original dataset for use in our
tutorials and documentation.

We include the source code that prepares the datasets for redistribution by
filtering, standardizing, converting coordinates, compressing, etc.
The goal is to make loading the data as easy as possible (e.g., a single call
to `pandas.read_csv` or `xarray.load_dataset`).
Whenever possible, the code also downloads the original data (otherwise the
original data are included in this repository).

> 💡 **Tip:** The easiest way to download this dataset is using
> [Pooch](https://www.fatiando.org/pooch), particularly to download straight
> from the DOI of a release.

## Contributing

See our [Contributing Guidelines][contrib] for information on proposing new
datasets and making changes to this repository.

## License

All Python source code is made available under the BSD 3-clause license. You
can freely use and modify the code, without warranty, so long as you provide
attribution to the authors.

Unless otherwise specified, all data files and figures created by the code are
available under the Creative Commons Attribution 4.0 License (CC-BY).

See [`LICENSE.txt`](LICENSE.txt) for the full text of each license.

The license for the original data is specified in this `README.md` file.


[contrib]: https://github.com/fatiando-data/.github/blob/main/CONTRIBUTING.md

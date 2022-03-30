About images-into-array
=======================

Home: https://github.com/sujitmandal/images-into-array

Package license: MIT

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/images-into-array-feedstock/blob/main/LICENSE.txt)

Summary: Convert Multiple Images into a Array and Different Color Spaces into a Array

Development: https://github.com/sujitmandal/images-into-array

Documentation: https://sujitmandal.github.io/images-into-array/

Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=15799&branchName=main">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/images-into-array-feedstock?branchName=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-images--into--array-green.svg)](https://anaconda.org/conda-forge/images-into-array) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/images-into-array.svg)](https://anaconda.org/conda-forge/images-into-array) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/images-into-array.svg)](https://anaconda.org/conda-forge/images-into-array) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/images-into-array.svg)](https://anaconda.org/conda-forge/images-into-array) |


[![Build Status](https://travis-ci.org/sujitmandal/images-into-array.svg?branch=master)](https://travis-ci.org/sujitmandal/images-into-array) [![GitHub license](https://img.shields.io/github/license/sujitmandal/images-into-array)](https://github.com/sujitmandal/images-into-array/blob/master/LICENSE) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/images-into-array) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/images-into-array) ![PyPI](https://img.shields.io/pypi/v/images-into-array) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/images-into-array.svg)](https://anaconda.org/conda-forge/images-into-array) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/images-into-array/badges/version.svg)](https://anaconda.org/conda-forge/images-into-array) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/images-into-array/badges/installer/conda.svg)](https://conda.anaconda.org/conda-forge) [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/images-into-array.svg)](https://anaconda.org/conda-forge/images-into-array) [![Conda Recipe](https://img.shields.io/badge/recipe-images--into--array-green.svg)](https://anaconda.org/conda-forge/images-into-array) ![](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/images-into-array-feedstock?branchName=main)

[![Downloads](https://pepy.tech/badge/images-into-array)](https://pepy.tech/project/images-into-array) 

Installing images-into-array
============================

Installing `images-into-array` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `images-into-array` can be installed with `conda`:

```
conda install images-into-array
```

or with `mamba`:

```
mamba install images-into-array
```

It is possible to list all of the versions of `images-into-array` available on your platform with `conda`:

```
conda search images-into-array --channel conda-forge
```

or with `mamba`:

```
mamba search images-into-array --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search images-into-array --channel conda-forge

# List packages depending on `images-into-array`:
mamba repoquery whoneeds images-into-array --channel conda-forge

# List dependencies of `images-into-array`:
mamba repoquery depends images-into-array --channel conda-forge
```

## Package Installation  : 
```
pip install images-into-array
```
[Package Link](https://pypi.org/project/images-into-array/)

```
conda install -c conda-forge images-into-array
```
[Conda Package Link](https://anaconda.org/conda-forge/images-into-array)

[images-into-array-feedstock](https://github.com/conda-forge/images-into-array-feedstock)


## Convert-Images-Into-Array:
Convert Multiple Images into a Array and Different Color Spaces into a Array.This package fuction requres three argument one is path of the images folder and other is image_height and image_width.

OpenCV Document :
-----------------
[OpenCV Document](https://docs.opencv.org/3.4/de/d25/imgproc_color_conversions.html)

## How to import the module:
```python
images_path = ('')

image_height = 'Enter The Image Size [32, 64, 128]'

image_width = 'Enter The Image Size [32, 64, 128]'
```
## NORMAL :
```python
from images_into_array.images_into_array import images

array = images(images_path, image_height, image_width)

print(array.shape)
```
## RGB ↔ GRAY :
```python
from images_into_array.images_into_array import rgb_gray

gray = rgb_gray(images_path, image_height, image_width)

print(gray.shape)
```
## RGB ↔ CIE L*a*b* :
```python
from images_into_array.images_into_array import rgb_lab

lav = rgb_lab(images_path, image_height, image_width)

print(lav.shape)
```
## RGB ↔ HLS :
```python
from images_into_array.images_into_array import rgb_hls

hls = rgb_hls(images_path, image_height, image_width)

print(hls.shape)
```
## RGB ↔ CIE L*u*v* :
```python
from images_into_array.images_into_array import rgb_luv

luv = rgb_luv(images_path, image_height, image_width)

print(luv.shape)
```
## RGB ↔ HSV :
```python
from images_into_array.images_into_array import rgb_hsv

hsv = rgb_hsv(images_path, image_height, image_width)

print(hsv.shape)
```
## RGB ↔ YCrCb JPEG (or YCC) :
```python
from images_into_array.images_into_array import rgb_ycrcb

ycrcb = rgb_ycrcb(images_path, image_height, image_width)

print(ycrcb.shape)
```

## Required package’s:
```
• conda install -c conda-forge opencv=4.2.0

• pip install shuffle

• pip install numpy

• pip install tqdm
```

About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [Anaconda-Cloud](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating images-into-array-feedstock
====================================

If you would like to improve the images-into-array recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/images-into-array-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@sujitmandal](https://github.com/sujitmandal/)


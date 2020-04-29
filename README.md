Python for Geosciences
======================

Video of the course available here https://www.youtube.com/watch?v=5nunA-pSS2g

You can run this notebooks interactevely on [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/koldunovn/python_for_geosciences/master)
 
This is a short overview of how Python is used in science and particularly in geosciences. 
The idea is to show how to setup Python for purposes of scientific computation and visualization, cover some basic features of the language and show some of the real world applications such as:

* Array manipulations.
* I/O (binary, txt, netCDF, mat).
* Creation of maps and graphics.
* Time series analysis.

This overview is aimed at the scientists who are interested in Python but don't know how to start using it (this might be really confusing for a newcomer), or would like to learn more about possible Python applications. For those of you who already use Python there will be nothing really new.

This notes will be helpful only if you know some programming language already (preferably Matlab). Notes are also avalible as webpages at [earthpy.org](http://earthpy.org/category/introduction-to-python.html).

PRs with corrections are very welcomed.

## Getting started for Linux/Mac

The fastest way is to install [Miniconda](http://conda.pydata.org/miniconda.html), that contains [`conda`](http://conda.pydata.org/docs/intro.html) package manager and `Python`. On the [Miniconda](http://conda.pydata.org/miniconda.html) page select **Python 3** installer script for your system and download it, for example:

```
wget https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
```

Change mode of the downloaded scrip to executable, e.g.:

```
chmod +x Miniconda3-latest-MacOSX-x86_64.sh
```

Run installation process:
```
./Miniconda3-latest-MacOSX-x86_64.sh
```
At the end the script will offer you to add Miniconda3 install location to the PATH in your `.bashrc/.bash_profile`. You should say 'yes'. Please double check that you have something like this in your `.bashrc/.bash_profile`:

```
# added by Miniconda3 4.3.21 installer
export PATH="/Users/koldunovn/miniconda3/bin:$PATH"
```
If you for whatever strange reason use csh/tcsh, then add to your `.cshrc`:

```
setenv PATH /Users/koldunovn/miniconda3/bin:$PATH
```
Now you can open a new terminal window (sourcing not always works) and try to type:

```
conda
```
if as a result you see conda help, then everything is set up properly. The last thing before installing packages is to add `conda-forge` channel:
```
conda config --add channels conda-forge 
```
Now you can install nessesary packages:
```
conda install ipython jupyter matplotlib scipy pandas basemap netcdf4 requests xarray cartopy
```
To begin working with notebooks execute:
```
jupyter notebook
```
the browser should pop up with jupyter main page. You can navigate to the folder with notebooks from there and open them.

## Getting started for Windows

- First you have to download and install Anaconda python distribution for your system from [here](https://www.anaconda.com/products/individual#windows) (scroll down to "Anaconda installers"). [There is a nice video tutorial](https://medium.com/@GalarnykMichael/install-python-anaconda-on-windows-2020-f8e188f9a63d). If installation is sucessful, you will be able to work with notebooks from 02 to 07. In order to work with `netCDF` files `Basemap`, `cartopy`, `xarray` some additional steps are required.

- Go to start menu and launch `Anaconda prompt` programm.
- Execute follwing commands:
```
conda config --add channels conda-forge 
```
and then
```
conda install basemap netcdf4 requests xarray cartopy
```
- Agree with installation of additional packages by entering `Y`

Now you should be good to go. You can launch Jupyter notebook from visual Anaconda interface, or by opening `Anaconda prompt` and typing:
```
jupyter notebook
```


Links to nbviewer versions
======================

[00 Why python?](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/00%2520-%2520Why%2520Python.ipynb)

[01 Scientific modules and IPython](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/01%2520-%2520Scientific%2520modules%2520and%2520IPython.ipynb)

[02 Python basics](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/02%2520-%2520Python%2520basics.ipynb)

[03 NumPy arrays](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/03%2520-%2520NumPy%2520arrays.ipynb)

[04 Work with different data formats](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/04%2520-%2520Work%2520with%2520different%2520data%2520formats.ipynb)

[05 Graphs and maps (Matplotlib and Basemap)](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/05%2520-%2520Graphs%2520and%2520maps%2520%2528Matplotlib%2520and%2520Basemap%2529.ipynb)

[06 Time series analysis (Pandas)](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/06%2520-%2520Time%2520series%2520analysis%2520%2528Pandas%2529.ipynb)

[07 Other modules for geoscientists and collection of links](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/07%2520-%2520Other%2520modules%2520for%2520geoscientists.ipynb)

[Links](http://nbviewer.ipython.org/urls/raw.github.com/koldunovn/python_for_geosciences/master/Links.ipynb)

Author
========
Nikolay Koldunov

koldunovn@gmail.com

![Platform](https://anaconda.org/conda-forge/vitables/badges/platforms.svg) ![License](https://anaconda.org/conda-forge/vitables/badges/license.svg)

![Conda](https://anaconda.org/conda-forge/vitables/badges/version.svg) ![Conda_downloads](https://anaconda.org/conda-forge/vitables/badges/downloads.svg) ![PyPI](https://img.shields.io/pypi/v/vitables) ![PyPI_Downloads](https://static.pepy.tech/badge/vitables/month)

# ViTables

ViTables is a graphical tool for browsing and editing files in both PyTables
and HDF5 format. With ViTables you can easily navigate through the data
hierarchy, view and modify metadata, view actual data and more.

ViTables has been developed using Python and PyQt, a binding to Qt
libraries, so it should run on any platform that support these components
(this includes Windows, Mac OS X, Linux and many other Unices). The interface
and features are the same in all platforms. At the moment, ViTables has been
heavily tested on Linux and Windows platforms.

## Installation

### System requirements

ViTables 3.0.2 has been tested against the latest versions of Python 3,
PyTables and PyQt. You can try other versions at your own risk :).

### Installation on a conda environment

Using conda you should be able to run vitables on any system, let it
be linux, mac or windows. The following are instructions for linux-like
systems.

Simply run::

  $ conda install -c conda-forge vitables

### Installation on Windows and Mac OS X platforms

Currently there are no graphical installers available for these platforms. You
have to install ViTables from the command line, using one of the methods
described in the Linux section.

### Installation on Linux platforms

The Python setuptools are used to build and install ViTables.

The easiest way to install it is to download it from PyPi::

  $ pip install ViTables

Alternatively, you can download the binary package from the download area
(see vitables.org/Downloads for details), go to the directory where you have
downloaded the file and issue the command::

  $ pip install ViTables-3.0.2-py3-none-any.whl

This should install the ViTables wheel. If you experience problems installing
the binary package then you can install from sources (provided your system fulfills
the requirements listed in the above section). Just download the tarball from
the download area, uncompress it, change to the distribution directory and execute

 $ python setup.py install

If you are doing this on a MacOS X platform, please make sure that the
DYLD_LIBRARY_PATH environment variable has been setup properly.

If you are installing with a system Python then you will need superuser privileges
because ViTables will be installed in the system-protected area where
your system installs third party Python packages. If you prefer to install the package
in a different location (for instance, your home directory) so that the installation can be done by
non privileged users, you can do it using the --prefix (or --home) tag

 $ python setup.py install --prefix=/home/myuser/mystuff

Please, remember that installing Python modules in non-standard locations
makes it necessary to setup properly the PYTHONPATH environment variable so
that the Python interpreter can find the new modules.

If you need further customizations, please have a look to the output of the
command

 $python setup.py install --help

to see all the available options.

Feel free to subscribe to the [ViTables users group](https://groups.google.com/forum/#!forum/vitables-users) and to report bugs and
send suggestions or features requests.

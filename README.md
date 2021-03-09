# Moberg Analytics HDF5 Functions

This package provides user-friendly functions for reading HDF5 file content into Python. 

## Installation

You can install the Moberg Analytics HDF5 package from [PyPI](insert_link_to_pypi):

    pip install moberg_analytics_hdf5
    
This package was created using Python version 3.9.0.

## How to use

1 - Import the package into Python:
	
	from moberg_analytics_hdf5 import hdf5_tools
	
2 - Choose your HDF5 file:

	hdf5_filepath = r"path to the hdf5 file"
	
3 - Instantiate the HDF5Content class:
The HDF5Content class contains methods that organize the content of the HDF5 file into lists and dictionaries.

	cont_obj = hdf5_tools.HDF5Content(hdf5_filepath=hdf5_filepath)

4 - Instantiate the HDF5Components class:
The HDF5Components class contains methods that return various components of the HDF5 file such as
groups, datasets, dataset values, NumPy/Pandas matrices of dataset values, metadata, and structured dictionaries.

	comp_obj = hdf5_tools.HDF5Components(hdf5_filepath=hdf5_filepath)

# cell-image

Tools for segmenting and tracking cells and analyzing them.

Initialized from root-image project.

## Setup instructions:

### Windows:
   1. Download and install Anaconda (download link: http://repo.continuum.io/archive/Anaconda2-2.5.0-Windows-x86_64.exe)
   2. Enable conda-forge and install tifffile. See instructions at https://github.com/conda-forge/tifffile-feedstock
   3. (This can also be done in a virtualenv)

### Linux:
   1. Make a virtualenv in an env/ subdir of the main directory and activate it
   2. Install packages: pip install -r requirements.txt (this file was generated from pip freeze > requirements.txt)
       The exact package versions probably aren't necessary - it works with a bunch - but you may need a new-ish version to support all the TIFF features.

## Notes:
   - Received images for cell tracking have been slightly postprocessed after segmentation and have some artifacts (are those from jpg?). Make sure the whole integrated workflow doesn't do this.
   - Load tiffs source: https://stackoverflow.com/questions/7569553/working-with-tiffs-import-export-in-python-using-numpy
   - Warning: intermediate files are very big uncompressed TIFFs
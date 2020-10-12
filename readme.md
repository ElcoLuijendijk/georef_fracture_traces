# Jupyter notebooks to georeference a line shapefile

## Description
You can use this notebook to georeference a line shapefile using a set of control points. The shapefile is defined by the variable ``shpfile`` and the control point file by the variable ``control_pt_file`` that can be found in the parameters box in the notebook. The transformation can be performed using a first or second order polynomial. The resulting file is a 3D shapefile and is saved with the same filename as the input file, but with ``_georef.shp`` apppended to the filename. Note I am still working on finding a convenient output format for this, given that most GIS software only reads 2D shapefiles. The georeferenced control points and the georeferencing error is saved as a csv file named [georeferencing_results_control_pts.csv](georeferencing_results_control_pts.csv). In addition, the georeferenced control pts are saved as a 3D figure named [fig/transform_error.pdf](fig/transform_error.pdf)

In addition the resulting 3D line file can be converted back to a 2D file by projecting the lines onto a plane. The plane is defined by three points that are read from a shapefile that is defined by the variable ``plane_pt_file``. The resulting 2D shapefile is saved using the same name as the input file but with ``_projected_to_plane`` appended to the filename.


## Dependencies

The notebooks requires a number of python packages: numpy, matplotlib, pandas, geopandas, scipy, shapely, sympy
The easiest way to install these it to use Anaconda Python: https://www.anaconda.com/products/individual



## Authors
* **Elco Luijendijk**, <elco.luijendijk-at-posteo.de>


## Reference


## License
This project is licensed under the GNU lesser general public license (LGPL v3). See the [LICENSE.txt](LICENSE.txt) file for details.


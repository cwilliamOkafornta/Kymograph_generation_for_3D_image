# **<h1 align='center'>Kymograph_generation_for_3D_image</h1>**
This is a repo that demonstrates the generation of 2D kymograph from a 3D image (x, y and time). 

The embedded notebook is used to compute for the generation of a kymograph from a three-dimensional image (i.e.: x, y and time). The line profile intensity of each image frame is read out using the x- and y -y-coordinate positions of the two ends of the line. The readout intensities over the profile line are stacked along the y-axis to display a 2D kymograph as a simplified representation of the dynamics process from the input 3D image dataset.

Also, it is possible to extend the profile line beyond the initial two ends of the original x- and y-coordinates input for each frame. The profile line extension is set at 0 (i.e., there is no extension of the profile line beyond its original input.)

## `Input files`:

Two input files are required to run this notebook.
* 1.) 3D image (x, y and time)
* 2.) a CSV file containing 4 columns with the x- and y-coordinates values of the two ends. The columns should have the following headers:
 | X1 | Y1 | X2 | Y2 |
| :-----: | :-----: | :-----: | :-----: |
| `number` | `number` | `number` | `number` |
| `...` | `...` | `...` | `...` |


## `Output files`:

Three files are saved in the output folder after running this notebook.
* 1.) Kymograph image in .tif format.
* 2.) Heatmap of the kymograph in .png format.
* 3.) CSV file containing the intensity values of the kymograph. In principle, the kymograph can be reconstructed from this CSV file.


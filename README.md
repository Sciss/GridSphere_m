# Readme

This is a GNU Octave library by Kurt von Laven, published under a BSD style license. The original location are https://www.mathworks.com/matlabcentral/fileexchange/28842-grid-sphere and https://www.mathworks.com/matlabcentral/fileexchange/28844-find-nearest-neighbors-on-sphere - I forked this to GitHub to not having to deal with this idiotic MathWorks account crap to perform this simplest actions on their website.

Below is the original info:

## GridSphere

The grid may have a total of exactly 12, 42, 162, 642, ... points. Mathematically speaking, the grid may have either 12 or 2 + ( 10 * (4 ^ k) ) points, where k is a positive integer. The user may request any number of points, and the closest attainable value will be produced. All code is compatible with GNU Octave. The algorithm was developed by Nick A. Teanby of Oxford University. Refer to his website for the publication describing the approach and more elaborate geodesic grid software written in IDL: http://www.atm.ox.ac.uk/user/teanby/software.html#icos. Use the FindNearestNeighbors function, available on the MATLAB file exchange at http://www.mathworks.com/matlabcentral/fileexchange/28844-find-nearest-neighbors-on-sphere, to find the grid points closest to arbitrary query points.
GridSphere and FindNearestNeighbors share some functions in common. Each package contains a copy of these functions so that both can stand alone. To eliminate duplicates, simply move all the files into a single folder and replace the shared files when prompted.
Sample usage:

```
[latGridInDegrees, longGridInDegrees] = GridSphere(12)
latGridInDegrees =
-58.28253
-58.28253
-31.71747
-31.71747
0.00000
0.00000
0.00000
0.00000
31.71747
31.71747
58.28253
58.28253
longGridInDegrees =

0.00000
180.00000
-90.00000
90.00000
-148.28253
-31.71747
31.71747
148.28253
-90.00000
90.00000
0.00000
180.00000
```

## Nearest Neighbours

A geodesic grid is an even grid over the surface of a sphere. The algorithm is optimized for a grid generated by GridSphere and won't work on an arbitrary geodesic grid. All code is compatible with GNU Octave. The GridSphere function is available on the MATLAB file exchange at http://www.mathworks.com/matlabcentral/fileexchange/28842-gridsphere.
FindNearestNeighbors and GridSphere share some functions in common. Each package contains a copy of these functions so that both can stand alone. To eliminate duplicates, simply move all the files into a single folder and replace the shared files when prompted.


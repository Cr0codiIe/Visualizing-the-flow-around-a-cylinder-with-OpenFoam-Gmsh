# Visualizing-the-flow-around-a-cylinder-with-OpenFoam-Gmsh
Simulation and visualization of fluid flow around a circular cylinder using OpenFOAM ,specifically with icoFoam Solver. The Mesh was generated with Gmsh and results visualized in ParaView.

Steps taken: 
    1-Creating the geometry of the Mesh in Gmsh:
        4 Points with lines in between to create a rectangle
        5 points in the form of a circle connected with the Arc function
    2-Extruding the mesh
    3-Adding Physical Groups for each side of the Mesh for example : top, bottom, left, right ...
    4-put the Mush in 3D and Export as msh version 2

    4-Open OpenFoam and copy the directory of $FOAM_TUTORIALS/incompressible/icoFoam/cavity/cavity 
    5-run the function gmshToFoam
    6-Modify the boundary conditions of p and U
    7-Run icoFoam and do the command : touch case.foam and open the file in Paraview
    8-Visualize the data 
    9-Run the filter plot over Line to get a graph of U and p

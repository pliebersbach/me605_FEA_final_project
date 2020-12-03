# me605_FEA_final_project

Author: Piotr Liebersbach

Final project for University of Wisconsin Madison mechanical engineering course ME 605 - Finite Element Analysis.  Project implements 4 node isoparametric quadrilateral element for thermal analysis.  Full and reduced Gauss Quadrature integration rules are implemented respectively for stiffness matrix assembly to observe effect of intergration rules on analysis solution.  Code is written in Fortran language, and is implemented within FEMCOD, an FEA code originally developed by Micheal E. Plesha (course instructor) et. al.

Usage:
  Compile with fortran compiler such as:
  
    gfortran femcod.f -o femcod.o
  Run the program with:
  
    ./femcod.o
    
  Follow directions as prompted and enter the mesh and problem data file name, then enter a name for an output file when prompted.

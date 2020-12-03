# me605_FEA_final_project

Author: Piotr Liebersbach

Final project for University of Wisconsin Madison mechanical engineering course ME 605 - Finite Element Analysis.  Project implements 4 node isoparametric quadrilateral element for thermal analysis.  Full and reduced Gauss Quadrature integration rules are implemented respectively for stiffness matrix assembly to observe effect of intergration rules on analysis solution.  Code is written in Fortran language, and is implemented within FEMCOD, an FEA code originally developed by Micheal E. Plesha (course instructor) et. al.

Usage:
  Compile with fortran compiler such as:
  
    gfortran femcod.f -o femcod.o
  Run the program with:
  
    ./femcod.o
    
  Follow directions as prompted and enter the mesh and problem data file name, then enter a name for an output file when prompted.
  
Files:
  1. FEMCOD.f - vanilla femcod.f fea code provided for project
  2. TwoBarData.txt - input data for simple fea mechanical analysis of a two bar truss system
  3. isquad_full.txt - Fortran subroutine that assembles stiffness matrix for 4 node isoparamtric quad element for heat transer, using full integration
  4. isquad_reduced.txt - Fortran subroutine that assembles stiffness matrix for 4 node isoparamtric quad element for heat transer, using reduced integration
  5. patch.txt - input data for thermal analysis patch test, consists distorted 4 element geometry and constant temperature boundary conditions
  6. patch2.txt - input data for thermal analysis patch test, consists 4 element geometry and constant temperature boundary conditions
  7. plfemcod.f - femcod.f code, includes subroutine for quad element thermal analysis with full integration
  8. plfemcod2.f - femcod.f code, include subroutine for quad element thermal analysis with reduced integration
  9. project_2_report_pl.pdf - summarized project findings and results
  10. quad_mesh.txt - input data for thermal analysis of plate with circular hole in the middle



The user inputs the initial machine parameters (flow rate, head, and rotational speed), and the program generates a meridional contour based on the theory of \citeonline{artigo:bovet1961}. This includes the meridional projection curves for the leading edge, trailing edge, shroud, and hub, as well as a number of meridional streamlines, which are defined by the user.
The program determines the hydraulic passage widths ($b$) for three specific stations: the trailing edge (TE) of the guide vanes, and the leading edge (LE) and trailing edge (TE) of the runner. Meridional velocities are calculated using the continuity equation (\ref{eq:conti}) and, for the leading edge, equation (\ref{eq:cm}).
Based on the flow rate, hydraulic passage widths, and the number of guide vanes (specified by the user), the program uses equations (\ref{eq:tan2}) and (\ref{eq:ct2}) to define the velocity triangle at the trailing edge of the guide vanes.
The program determines the velocity triangles at each intersection between the streamlines and the leading and trailing edges, applying the free-vortex relationship (equation \ref{eq:ct3}) and trigonometric principles (equation \ref{eq:ct4}).
Finally, the program calculates the blade angles using the trigonometric relationships provided in equations (\ref{eq:tan3}) and (\ref{eq:tan4}).

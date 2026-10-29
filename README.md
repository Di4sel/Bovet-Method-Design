Meanline design of Francis Turbines, based on the Bovet method (Contribution à l'étude du tracé d'aubage d'une turbine à réaction du type Francis - T. Bovet), by Rodolfo Dias.

Meridional contour design based on: https://github.com/newton-raphson/francis-runner-design

A easy-to-use in-browser version can be lauched through Google Collaboratory with: https://colab.research.google.com/drive/1WVGPDoRbQx1GHEFfpA5WqilT1Bm-kpY1?usp=sharing
In this link theres also an example input and output.

**Description of the main logic:**
1.  The user inputs the initial machine parameters (flow rate, head, and rotational speed), and the program generates a meridional contour based on the theory of Bovet. This includes the meridional projection curves for the leading edge, trailing edge, shroud, and hub, as well as a number of meridional streamlines, which are defined by the user.
2.  The program determines the hydraulic passage widths (b) for three specific stations: the trailing edge (TE) of the guide vanes, leading edge (LE) and trailing edge (TE) of the runner. Meridional velocities (cm) are calculated using the continuity equation and, for the leading edge, the *cm_factor* function is used (this function is also based on Bovet's article).
3.  Based on the flow rate, hydraulic passage widths, and the number of guide vanes (specified by the user), the program defines the velocity triangle at the trailing edge of the guide vanes.
4.  The program determines the velocity triangles at each intersection between the streamlines and the leading and trailing edges, applying the free-vortex relationship and trigonometric principles.
5.  Finally, the program calculates the blade angles using the trigonometric relationships.

**Known flaws:**
1.  The code doesn't work at every possible "Ns". There's a problem with the meridional contour generation.
2.  It is not well structured, a good software engineer could do a better job. Unfortunatelly I'm a amateur coder and I don't really know how to design a good function logic. 

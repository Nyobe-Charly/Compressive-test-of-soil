# Post-Soil Interaction Modeling for roadside safety barriers 
The four models are built on Ls - prepost (R) V4.3.20 from Ls - dyna. Calculations are performed on a calculation server.

## Compression_test.k
The test consists in compressing the soil contained in the tank by a rigid solid. All points of the solid in contact with the ground move by 200 mm. The resultant of the nodal forces exerted by the solid on the ground is extracted in RCFORC contained in the BINOUT file. The resultant force-displacement curve is plotted.

## mat147_model. k
This reference model simulates the impact of a wooden post in the ground. The ground is represented by a 3D finite element solid.

## kh_kv_model.k 
It represents the first simplified model. The soil is represented by nonlinear springs. These springs are arranged horizontally and vertically along the wooden post.

## kh_model.k 
The second model, is similar to the first simplified model except that the vertical springs are removed. For support in the vertical direction, the post is constrained at its central node at ground level: the vertical displacement of the post is zero at this node. 


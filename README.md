# Investigating Flood inundation uncertainty in a probablistic manner

Flood inundation uncertainty mainly stems from three parts:


1. Boundary condition  
2. Forcing data  
3. Model parameters  
4. Model structure (including physical representation, solver, meshes)  
5. Terrain data  

## Setup CREST model 

1. We used 10-m NED DEM downloaded from TNM USGS  
2. We upscale 10-m DEM to 90-m DEM to speed up hydrologic simulation  
3. The river channel is burned into DEM with Whitebox "FillBurn"  
4. Flow direction and Flow accumulation are generated with Whitebox tool "FlowAccumulationFullWorkflow", and ESRI pointer scheme is ticked  
5. Put everything into a folder, and calibrate CREST at gauge 08114000 for Imelda event  

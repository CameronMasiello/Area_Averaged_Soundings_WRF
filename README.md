# Area_Averaged_Soundings_WRF
Area averaged soundings for WRF outputs, specifically for a storm following inner nest.

The example codes use the inner nest, d02, of a storm following inner domain to calculate storm following area averaged soundings and point stationary area averaged soundings! 

The provided examples utilize python to compute these soundings. Imported packages include Xarray, WRFpython, and Matplotlib. The function that plots the figures centered around the pressure minimum of the tropical cyclone is adapted from previous research conducted with Dr. Sharanya Majumdar and his research group at the University of Miami.

The inner nest was 4km in my d02. To adjust the area sounding properly, you will need to pre-determine the desired length's of the sides of the box and the divide by the grid spacing. For example, if I am interested in a 100 x 100 km area averaged sounding, if my grid spacing is 1 degree, my 
Extent of box variable will be set to 50! that is because the extent of box variable is telling you how much distance in the x_y direction away from your inputted center point you want your box to extend. This works best utilizng a mercator projection.

![](https://github.com/CameronMasiello/Area_Averaged_Soundings_WRF/blob/main/20201116_iota_vis%20glm_0.gif)

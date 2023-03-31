# EE_3.07 Geodata Management Systems WS2022/23 - <br> Final Assignment

## 1. Warming Stripes (20 Points)

**Sub-Task 1.1:** <br>

Goal: Filter out stations according to desired criteria.


**Sub-Task 1.2:** <br>

Goal: Generate a geopackage that can be inserted into QGIS and design a nice map.


**Sub-Task 1.3:** <br>

Goal: Use ftplib for downloading the data online while on jupyter-lab.



**Sub-Task 1.4:** <br>

Goal: Visualize the annual demeaned temperatures from each station.

**Work Process**

1. I used ftplib to access all the necessary files from online (DWD). The codes were based on Prof Becker's "gdms0180_DWD_NRW_Annual_Temp_vs_Altitude/gnb0181_DWD_NRW_Annual_Temp_vs_Altitude_V001.ipynb"

2. First I got the a large data frame of all stations. I then imposed & operations to get stations fitting the description: in NRW, currently active, and active before 1950. This was saved to another dataframe named 'selected_df'.

3. To generate a geopackage layer, I used geopandas to instantiate a geodataframe called gdf which was exported as 'my_13_stations.gpkg'. The coordinates from DWD were used by the method points_from_xy() to create and concatenate a geometry column to my geodataframe. I confirmed that this particular data used WGS84/EPSG:4326, which should be automatically reprojected upon being inserted into my QGIS project whose CRS is EPSG:25832.

4. After adding the DTK layer and my stations layer, I designed my map in the QGIS Map Composer. I could export to either PDF or PNG image. I chose the latter. I also saved the map as a vector in case I might want to do more to my project in the future. The vector is selected_NRW_stations.qgz.

5. To plot the warming stripes, I sourced the code from and edited Prof. Becker's code from his notebook 'gdms0155_DWD_NRW_5_Warming_Stripes/gdms155_DWD_NRW_5_Warming_Stripes.ipynb.' I moved most of the imported necessary packages/library at the beginning of my code. The generated plot was as expected, i.e. showing increased annual mean temperatures overall.

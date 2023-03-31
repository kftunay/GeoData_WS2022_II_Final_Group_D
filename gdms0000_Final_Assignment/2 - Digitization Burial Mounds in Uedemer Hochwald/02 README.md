# EE_3.07 Geodata Management Systems WS2022/23 - <br> Final Assignment

2. Digitization: Burial Mounds in Uedemer Hochwald

Task 2.1:

After downloading the file from the assignment fodler, we did the task with the QGIS Georeferencer GDAL Plugin.
Steps:

- Firstly, in the QGIS (version 3.28.4) application, under the menu Plugins>>Manage and Install Plugins>> Installed Plugins>> Georeferencer Plugin, was activated.

- The Georeferencer was then opened from the Raster menu. The given image of the burial sites in Uedemer Hochwald was then loaded into the Georeferencer. At the same time, the given QGIS Project, which included a topographic map of the area, was opened in QGIS.

- The transformation settings were first configured in the Georeferencer. Polynomial was chosen as the transformation type. The Closest Neighbor Resampling method was used, and the target coordinate system was EPSG:25832. The output target folder was selected, and the rest was kept as default.

- The image's points were located on the map canvas and used as the image's ground control points. On the map canvas, street junctions and forest trail crossings were easy to identify and locate. As a result, these points were added one by one to the raster image, and their coordinates were taken from the underlying map canvas. In total, 11 points were chosen, and the screenshot for the specific taken points are named as: screenshot georeferencing CGP.JPG

- Afterwards, the georeferencer is run and the output for the final georeferenced picture with the alignment of the raster image in the map is retrieved. The screenshot for this image is named as: screenshot task output 2.1.JPG

Task 2.2:Hillshade model

The given DTM layer fromt the assignment folder was chosen to work for this task. We also used the OSM standard option fromt he quick map services to see the exact location even though we had the DTK layer; but we did not chose both the layers to work further (just to see the map and we found OSM standard option very intriguing). Using the layer styling option > hillshade, we got a nice hillshade model. We tried to do different color shading with the hillshade options. 6 screenshots were taken with different angles and they are named as follows:

screenshot task 2.2 part 1 DTM udemer hochwald.JPG
screenshot task 2.2 part 2 DTM udemer hochwald.JPG
screenshot task 2.2 part 3 DTM udemer hochwald.JPG
screenshot task 2.2 part 4 DTM udemer hochwald.JPG
screenshot task 2.2 part 5 DTM udemer hochwald.JPG
screenshot task 2.2 part 6 DTM udemer hochwald.JPG

Task 2.3: 

Difficulties 01:
The Terrain profile plugin was installed. It was difficult for us to find the terrain profile, because we did not know it is a separate plugin and we needed to isntall it. So, we spent quiet amoount of time to udnerstand that there are different kinds of plugins which is needed to be installed manually.

Difficulties 02:
Using the terrain profile and the DTM layer, it was difficult to measure the mounds. Thus, we had to take the help of the hillshade to see the mounds and then to proceed we deselect the hillshade.

Difficulties 03:
we tried everything possible for getting the measurement of the mounds but anyhow the measurements or the graph was not shown in the terrain pürofile. It is because we also did not know that we had to select the layer from the right side option. It was a minor issue but also it took us good amount of time to understand the problems.

2.3.1 Terrain Profile

Finally after many difficulties, we understood how to use the terrain profile and also got the measurement. We took 5 measurements of 5 different mounds and the screenshot of the graphs are as follows:

2.3 - 01 geodata.png
2.3 - 02 geodata.png
2.3 - 03 geodata.png
2.3 - 04 geodata.png
2.3 - 05 geodata.png

The typical average elevation of the 5 calculated mounds is between 36.96m. 

Task 2.4:

A consistent pattern of lines at nearly equal intervals could be seen on the east to north-east side of the burial mounds, which are not the typical pedestrian trails. We are assuming that the place was into deforestation or something related to the history from the world war II - it is becasue one of our group members has visited the LVR-Archäologischer Park Xanten which is 10,6 km from the Uedemer Hochwald. From the stories we have heard from our group member, the museum is a Roman museum with all Roman houses, temples & an amphitheater. The museum has everything or mostly related to the Roman history from the World war II. So, we are confident of our assumptions that something related to the history also happened in the Uedemer Hochwald for which reason some of the roads are not linked or not structured.
From the web reseearch about the Uedemer Hochwald, we found out that, A Dutch archaeologist discovered traces of Roman forts and training camps in the forest in November 2012. From 2021, 15 core areas and the surrounding area have been designated as part of the "Lower Germanic Limes" World Heritage Site by UNESCO.
Related to the above description, we decided to chose the amphitheater from the LVR-Archäologischer Park Xanten as one of the structure to digitize

2.4.1 Digitization:

For this task, we used the OSM layer from the QuickMap Service as it is easier to locate the location and the OSM layer has all the features and we were easily able to locate the Roman amphitheater from the LVR-Archäologischer Park. We onyl used the polygon shape for the theater to be digitized. Using the layer styling option and New Shapefile Layer, we digitized the structure with a polygon shape; and also we tried to learn different shapings. We tried several times because we did not know how to use the polygon different options and we spent quiet amount of time in it as well. We took 4 screenshots for the following output which are named as follows:
screenshot_task_2.4_Roman theatre_digitzed 01.JPG
screenshot_task_2.4_Roman theatre_digitzed 02.JPG
screenshot_task_2.4_Roman theatre_digitzed 03.JPG
screenshot_task_2.4_Roman theatre_digitzed 04.JPG

2.4.2 Geopackaging

After digitizing it, in order to save it as a geopackage layer, we used the option' New GeoPackage Layer. 
The screenshot for this specific geopackage is shown as: screenshot_task_2.4_Geopackage 05.JPG
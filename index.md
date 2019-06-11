## About
Last Updated *[06/11/2019]*   
Created by [OSU Maps and Spatial Data](https://info.library.okstate.edu/map-room)

![img example](images/OSULogo.png)

## Table of Contents
- Introduction 
- *[Digitizing in ArcGIS Pro]*
- - Starting a New Project
- - Adding Files
- - Digitizing
- - - Feature Dataset
- - - Feature Class
- - - Point Features
- - - Line Features
- - - Polygon Features
- - - Deleting Features
- - - Saving
- - Editing
- - - Auto-complete Digitizing
- - - Merge
- - - Split
- Conclusion
- Further Reading/Resources

## Introduction
Digitizing allows image data to be converted to vector digital data. This is accomplished by manually digitizing objects by tracing lines or adding points based on the source media. 

#### Starting a New Project
1. To begin a new project, open ArcGIS on your desktop.
2. Click **Map** under *New, Blank Templates*.
    
![New Project](images/NewProject.PNG)

3. Name the project and choose a file location that will be easy to access. Then click **OK**. A new world map should open. 

#### Adding Files
Now that a new project has been created, a folder connection must be added to import data. 
1. To do this, click **Add Folder** under the *Insert* tab of the toolbar to create a folder connection.

![Folder Connection](images/FolderConnection.PNG)

2. Select the desired folder and click **OK**.
3. The folder connection should appear under *Folders* in the *Catalog* pane. 

![Catalog Connection](images/CatalogConnection.PNG)

4. Locate desired data. Right click the file and click **Add to Current Map**. The selected file is now added to the project and should appear in the *Contents* pane. It is okay if the raster is not displayed on the map as long as the file is visible in the Contents pane.

![Added File](images/AddedFile.PNG)

*Note: For georeferencing in ArcGIS Pro, JPGs are the preferred file type.*

#### Digitizing
Images are turned into vector digital data through the proccess of manually digitizing the images. 

##### Feature Dataset
Why do we create feature data sets?
1. To create a feature dataset, right click the desired GDB file in the *Databases* folder of the *Catalog* pane. 
2. Select **NEW** and **Feature Dataset**.

![Feature dataset](images/FeatureDataset.PNG)

3. A *geoprocessing* pane should appear. Give the dataset a title and select the desired coordinate system. Then click **Run** at the bottom of the pane. Once this process is complete, a green box should appear at the bottom of the *geoprocessing* pane declaring success. 

![Feature dataset 2](images/FeatureDataset2.PNG)

##### Feature Class
Why do we create feature classes? 

1.To create a feature class, right click the desired GDB file in the *Databases* folder of the *Catalog* pane. 
2. Select **NEW** and **Feature Class**.

![Feature class](images/FeatureClass.PNG)

3. A *Create Feature Class* pane should appear. Give the class a name, select the desired feature class type and continue through the next few pages. These pages allow you to import fields, select the desired coordinate system, set tolerance, alter resolution and specify storage configuration. 

![Feature class 2](images/FeatureClass2.PNG)

4. The new feature class will appear in the *catalog* pane under the feature database that was previously created. To add the layer to the project, right click and select **Add to Current Map**. A new layer should appear in the *Contents* pane. 

![Add](images/Add.PNG)

##### Point Features
1. To add point features, be sure to select **Point** as the desired feature class when creating a feature class.
2. Go to the *Edit* tab of the toolbar and select **Create**. A *Create Features* pane should appear.

![CF](images/CF.PNG)

3. In the *Create Features* pane, select the layer you want to digitize (wording). A few tools will appear under the layer. Select **Point**. Points can now be added as desired.

![CF2](images/CF2.PNG)

4. To add a point, simply locate an object you would like to mark and click in the center 

5. Continue adding points as desired. 

![Point added](images/PointAdded.PNG)

##### Line Features
1. To add line features, be sure to select **Line** as the desired feature class when creating a feature class.
2. Go to the *Edit* tab of the toolbar and select **Create**. A *Create Features* pane should appear.
3. In the *Create Features* pane, select the layer you want to digitize (wording). A few tools will appear under the layer. Select **Line**. Lines can now be added as desired.

![CF3](images/CF3.PNG)

4. To create a line, decide where the line should start and click. A vertext should appear. Add another vertex to create a line.

![vertex](images./Vertex.PNG)

5. More vertexes can be added to create a longer line or to manipulate the shape of the line.

![Line](images/CompletedLines.PNG)

##### Polygon Features
1. To add polygon features, be sure to select *Polygon** as the desired feature class when creating a feature class.
2. Go to the *Edit* tab of the toolbar and select **Create**. A *Create Features* pane should appear.
3. In the *Create Features* pane, select the layer you want to digitize (wording). A few tools will appear under the layer. Select **Polygon**. Polygons can now be added as desired.

![Poly](images/Poly.PNG)

4. To create a polygon, decide where the polygon should start and click. A vertext should appear. Add another vertex to create a line and continue this process until the shape is closed.

![Poly2](images/Poly2.PNG)

5. To finish a polygon, double click on the last vertex that was placed. The polygon outline should appear highlighted. 

![Poly3](images/Poly3.PNG)

##### Deleting Features
1. To delete a digitized feature, click **Select** in the *Edit* tab of the toolbar.

![Select2](images/Select2.PNG)

2. Right click the feature and choose **Delete**. It should disappear. 

![Delete](images/Delete.PNG)

##### Saving
Be sure to save your work periodically. The save icon in the top left corner of the screen does not save digitized objects.

1. To ensure digitizing is saved, click **Save** in the *Edit* tab of the toolbar. 

![SaveEdit](images/SaveEdit.PNG)

2. A pop up should appear. Click **Yes** to save all edits.

![SaveEdits](images/SaveEdits.PNG)

#### Editing
Digitized features may be edited after they are created. The three most common editing tools involve auto-complete digizing, merging and splitting. 

##### Auto-Complete Digitizing
Auto-complete digitizing allows a polygon to be created that abudts another existing polygon. This means the same line does not have to be digitized more than once, which can lead to complications such a slivers. 

1. To autocomplete a polygon, open the *Create Features* pane and select **Autocomplete Polygon**.

![AutoC](images/AutoC.PNG)

2. Select a starting point on the existing polygon feature and outline the new feature that you would like to digitize. Be sure the end point is on the exisitng polygon feature.

![Draw](images/Draw.PNG)

3. Double click to complete the new polygon. Now two polygons have been created without duplicating a line. 

![AutoC2](images/AutoC2.PNG)

##### Merge
Merging a tool taht allows different features to be merged into one.

1. To merge digitized features, click **Merge** under the *Edit* tab. 

![Merge](images/Merge.PNG)

2. A *Modify Features* pane should appear. You can select the desired features in one of two ways:
- 1. With the **Merge** tool activated, click on the first desired feature. Hold down **CTRL** on the keyboard and select the remaining features. The features will appear highlighted.
- 2. Use the mouse to draw a box around the desired features by left clicking and holding as you drag the box over the desired area. The features will appear highlighted.

![Select](images/Select.PNG)

3. After the features have been selected, click **Merge** in the bottom right hand corner of the *Modify Features* pane. The features are now merged into one feature. 

![Merge 2](images/Merge2.PNG)

##### Split
Splitting polygons is the opposite of merging. 

1. To split polygons, select **Split** under the *Edit* tab. 

![Split](images/Split.PNG)

2. Draw a line where you would like to split the existing polygon.

![Split 2](images/Split2.PNG)

3. Double click at the end point to split the polygon into two seperate polygons. 

![Split3](images/Split3.PNG)

## Conclusion

## Further Reading/Resources


[Return to Top](#about)

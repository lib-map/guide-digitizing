## About
Last Updated *[06/06/2019]*   
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
- - - Snapping?
- - - Saving?
- - - Point Features
- - - Line Features
- - - Polygon Features
- - Editing
- - - Auto-complete Digitizing
- - - Merging
- - - Splitting
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

##### Snapping?

##### Saving?

##### Point Features
1. To add point features, be sure to select **Point** as the desired feature class when creating a feature class.
2. Go to the *Edit* tab of the toolbar and select **Create**. A *Create Features* pane should appear.

![CF](images/CF.PNG)

3. In the *Create Features* pane, select the layer you want to digitize (wording). A few tools will appear under the layer. Select **Point**. Points can now be added as desired.

4. To add a point, simply locate an object you would like to mark and click in the center 

![CF2](images/CF2.PNG)

5. Continue adding points as desired. 

![Points added](images/PointsAdded.PNG)

##### Line Features

##### Polygon Features

#### Editing

##### Auto-complete Digitizing

##### Merging

##### Splitting

##### Delete
1. To delete a misplaced point, click **Select** in the *Edit* tab of the toolbar.

![Select](images/Select.PNG)

2. Right click the point and choose **Delete**. The point should disappear. 

![Delete](images/Delete.PNG)

## Conclusion

## Further Reading/Resources


[Return to Top](#about)

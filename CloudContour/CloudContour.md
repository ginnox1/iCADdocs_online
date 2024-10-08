# Cloud Data and Contours
[Back to Home](..\index#online-documentation)

iCAD presents an easy to use module to process point cloud data from surveying, drone data or other sources, and creating contour plots. It includes powerful analysis tools for creating a surface mesh, data grids and outlier analysis.

To start using the **ContourCloud** module, one must have the point cloud data hosted on to an AutoCAD object. Refer to  [Data Processing & Presentation](..\DataProcessing\DataProcessing#host-data-to-autocad-objects) under the section *Hosting Data to AutoCAD Object*.


## Table of Contents
<!--TOC-->
  - [Defiing Boundaries](#defiing-boundaries)
  - [Creating Regions of Interest (RoIs)](#creating-regions-of-interest-rois)
    - [Automatic Boudndary creaion](#automatic-boudndary-creaion)
    - [Manuall Edit or creation.](#manuall-edit-or-creation.)
    - [Import from AutoCAD](#import-from-autocad)
  - [Point cloud processing](#point-cloud-processing)
    - [Filetering Data to RoIs](#filetering-data-to-rois)
    - [Identifying Outliers](#identifying-outliers)
    - [Generating Contours](#generating-contours)
  - [Generated AutoCAD Plots](#generated-autocad-plots)
    - [Working with large data sets](#working-with-large-data-sets)
<!--/TOC-->


## Defiing Boundaries
[Back to ToC](#table-of-contents)

Befor continuing make sure the cloud data is hosted on to an AutoCAD object, and your current iCAD session is linked to the AutoCAD file containing the object.

> :bulb: **Note**: It is always recommended to use standard host objects found in iCAD's latest release library. Avoid using arbitrary objects, especially when the work will persist, and may be shared with others.

1. Invoke the *New Session* process from `Session > Creare and Run New Session...` menu command. Alternatively, you can start it from the *Workspace Manager* by clicking on the toolbar button as shown.


    <img src="./media/Image 002.png" style="width:6in">

    *Figure: starting session browser from menu command.*

    <img src="./media/Image 003.png" style="width:3in">

    *Figure: starting session browser from the Workspace manager interface.*

1. In the *Module Browser* dialog, select **ContourCloud** module, and hit `Continue`.
    <img src="./media/Image 004.png" style="width:4in">

1. Provide a name for the session, and hit `Ok.`

    <img src="./media/Image 005.png" style="width:3.5in">

1. In the *New Session* dialog, click on the **Spot Data Host** list item. AutoCAD will be in select mode. Go and pick the host object refering to the cloud data for processing.

    <img src="./media/Image 006.png" style="width:6in">

    > :bulb: **Tip** The process will validate the object for expected data, and may throw an error message. Resolve the issue and try again, if this happens.

    <img src="./media/Image 007.png" style="width:2.8in">

    Upon succesful selection, and acceptance of the selected object, the list item will be checked, and the run button activated. Hit `Run Session` to continue.

    <img src="./media/Image 008.png" style="width:3in">

    This will start the module with the cloud data plotted on the main interface. Use the functions available under the **Workflow Menu** to process, present and export results.

    <img src="./media/Image 009.png" style="width:7in">

## Creating Regions of Interest (RoIs)
[Back to ToC](#table-of-contents)

A boundary information is required to execute any point cloud processing. The boundary area can be created in different ways.

### Automatic Boudndary creaion
[Back to ToC](#table-of-contents)

Use `Workflow > Auto Delineate Region` to create a boundary area around the data point automatically. 

<img src="./media/Image 010.png" style="width:7in">


The generated boundary can be made more tight or loose around the point cloud data using the shrink factor variable.

<img src="./media/Image 030.png" style="width:5in">

Choose a value close to 1, to make the boundary more tight around the points as shown below.

<img src="./media/Image 032.png" style="Width:5in">


Choose a value close to 0 for a more loose boundary.

<img src="./media/Image 031.png" style="Width:5in">

### Manuall Boundary creation or Edit
[Back to ToC](#table-of-contents)

One can also manually create new boundary data from `Workflow > Draw Region` menu command,

Any boundary area created, can be edited by using `Workflow > Add Region` and `Workflow > Subtract Region` menu commands.

<img src="./media/Image 011.png" style="width:7in">

<img src="./media/Image 012.png" style="width:7in">

When starting all the manual commands (creating, adding and subtracting) follow these steps.
- Select the desired points interactively by using `Left Mouse Click`.
- Use `BackSpace` key to delete the previously inserted point, and resume insertion.
- Use `Shift`+ `Left Click` or `Right Click` to insert the finalpoint. This will end the selection mode.
- Use `Enter` key to end point insertion process.

Upon completion, the new area is added or subtracted, depending on the menu command used to invoke the process.

> :bulb: **Tip**: Boundary data area saved along with any other relevant data with the session. Hit `Save` to save the data.

Previously defined and saved boundary data can be inserted using `Workflow > Load Existing Boundary` menu command.

### Import from AutoCAD
[Back to ToC](#table-of-contents)

If an RoI is defined in AutoCAD environment, this can be imported using the `Workflow > Pick from AutoCAD` menu command.

<img src="./media/Image 014.png" style="width:7in">


## Point cloud processing
[Back to ToC](#table-of-contents)


Once the boundary data is established different operations can be done on the cloud data set, as described below.

### Filetering Data to RoIs
[Back to ToC](#table-of-contents)

Filtering data can be very helpful, especially when dealing with a large point cloud data set. The `Workflow > Filter Cloud to Boundary` tool alows to id and filter all data points in or on the boundary area defined. 

The resuls are displayed on the *Data Table* interface, as noted on the statu bar.

<img src="./media/Image 015.png" style="width:7in">

The filtered data set can be copied for further processing with spreadsheet applications.

> :bulb: **Tip**: The copid data can be hosted on to any AutoCAD object directly from `Tools > Paste CSV data`.


### Identifying Outliers
[Back to ToC](#table-of-contents)

Statistical analysis can help deal with identifiying and dealing with Outlier data. Rarely, this can be an issue engineers enconter when dealing with raw surveyng data or from other sources.

Identifying outliers can be achieved from `Workflow > Data Statistics` menu command. The process will display the result using a box chart, a standard statistical visualization tool.

<img src="./media/Image 019.png" style="width:7in">

Where outliers are detected, the outlier points are also marked on the main interface with red circles. `Right-Click` on any outlier, and the context menu offers an option to remove the outlier.

<img src="./media/Image 023.png" style="width:4in">

> :warning: **Important Note**: The data is removed from the workspace. Save the session, to make sure the data is removed from the session data. 

> Note also that this will not remove data points from the source object.

To make sure the data from the host object is also clean, filter the data as outliened above to the bounding area containing all data points, and host it again to the source object.


### Generating Contours
[Back to ToC](#table-of-contents)

Contours can be generated using different specifications. These are found in the variables editor under the Contour Parameters group.

<img src="./media/Image 033.png" style="Width:4in">{br}

- Grid Intervals: Higher and lower ordeer grid intervals for calculating a regularly spaced mesh data for input to contour generation. The most important parameter is the lower value. For most uses, 20 is a good value.
- Method: Specifies the method for grid data creation method. The options available are
    - GridContour (default)
    - gridFit (usually faster and robust - under development)
    
- Contour Intervals: The values of contour levels to generate, specifying the contolr elements desired. There are two common methods:
  - [zi, zint, zend]: This format specifies starting level, the incremental level, and the final level. In the snap shot above 1090, 2000, 2010, ..., 1500 will be created.
  - [zi, zint, zint_major, zend]: This format specifies the desired contour lines for major levels.{br}


    <img src="./media/Image 036.png" style="width:4in">

- Smoothing Points per Grid: This value is by default 0, indicating no smoothing applied. Input an integer value between 1 and 4 to smoothen the contours. Each grid cell is subdivided in to smaller regions based on this setting, and cubic interpolation is applied on the grid data, resulting in a more smoother contour.
- Text Label: Show sparse or dense contour labels along the generated contours.

    > **Important Note:** If a surface data is loaded in to the iCAD workspace (see image below), this overrides the use of the specified methods and implements the interpolant generated from the surface data. 

   <img src="./media/Image 035.png" >

Once the settings for the session are all assigned, contours are generated using `Workflow > Create Contours` menu command. 

<img src="./media/Image 018.png" style="width:7in">

The interval for generating contours can be controlled from `Workflow > Edit Variables ` menu command. One can also specify if contour lables are needed, and how dense they should be.

> :bulb: **Tip**: For computational efficiency, boundary and grid data are calculated once and stored. This may some times cause contour plots to NOT respond to new boundary areas created. If this happens, use `Workflow > Clear Calcualted Data` and run again.

<img src="./media/Image 024.png" style="width:7in">

The following image shows contours generated for the same data, with and with out smooting. Smoothing gives a more presentable result, as can be seen in parts of the contour area.

<img src="./media/Image 034.png" style="width:5in">{br}

> **Note:** It is important to keep in mind that smoothed out contours are second level interpolations and DO NOT accurately represent surface variation. They are also not used in subsequent analysis in any way in iCAD and related products. 



## Generated AutoCAD Plots
[Back to ToC](#table-of-contents)

Contour plots and boundary data can be easily plotted to AutoCAD environment. FOllow below steps:
1. Start the `Workflow > Select Draw to AutoCAD` menu command.

    <img src="./media/Image 025.png" style="width:7in">

1. From the *Select Groups* dialog, select the objects to draw to AutoCAD. You can choose Contours, Boundy or both. Then follow the prompts.
   
   Note that, Contours are created as groups.

1. Once in AutoCAD environment, you can label contoures as follows. Start the AutoCAD addon tool as shown below.

    <img src="./media/Image 027.Png">

1. When prompted, pick a sample text. The Height of the sample text selected will be used to generate the contour labels. Note, the text style used will be the current style of AutoCAD. Simply hit ENTER to input a desired text height.

1. When prompted, pick all the contour line objects you want to label. Right Click when done. 
1. You will be prompted to draw a crossing line along the locations where you want contour labels. Pick a starting and ending ponts.

    <img src="./media/Image 028.png">

1. The contour labels will be generated as shown below.

     <img src="./media/Image 029.png" style="Width:5in">


1. Repeat from step 5 to continue generating more labels, or hit Enter key to finish.


For more information on generating drawings to AutoCAD see the [Data Processing and Presetation Section](.\DataProcessing\DataProcesssing).

> :bulb:    **Tip**: Controus are generated to AutoCAD with contour label information, and at the elevation matching the contour level. Use the *AutoCAD Addon*  tools to create the labels.




###  Working with large data sets
[Back to ToC](#table-of-contents)

> Note: Below tips apply to older versions (before Jul 2024), and may not be needed in recent versions. Algorithms and workflows have been optimized.

When working with larger data sets, contour generation to AutoCAD can take some time. The following workaround may help save some time, in such cases. Assuming the user needs a contour plot of 1.0 unit interval:

First, generate the contours with out the need for labeling, i.e., every 1unit interval, and export using *Render to File* option. This process should complete much faster.

Finally, generate the contours that require labeling, such as major contour lines at 5m intervals, and generate directly (with out the *render to file* option). This may take a while, but because the contour lines are much smaller in number, there is a timve saving.

<img src="./media/Image 026.png" style="width:7in">




END.
 
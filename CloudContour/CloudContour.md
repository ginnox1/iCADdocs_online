# Cloud Data and Contours
[Back to Home](..\index#online-documentation)

iCAD presents an easy to use module to process point cloud data from surveying, drone data or other sources, and creating contour plots. It includes powerful analysis tools for creating a surface mesh, data grids and outlier analysis.

To start using the **ContourCloud** module, one must have the point cloud data hosted on to an AutoCAD object. Refer to  [Data Processing & Presentation](..\DataProcessing\DataProcessing.md#host-data) under the section *Hosting Data to AutoCAD Object*.


## Table of Contents
<!--TOC-->
  - [Defining the module](#defining-the-module)
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
  - [](#)
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


> :bulb: **Tip**: Use the *Shrink Factor* variable setting to control how the boundary is created for the cloud point data set.

### Manuall Edit or creation.
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


Contours are generated using `Workflow > Create Contours` menu command. 

<img src="./media/Image 018.png" style="width:7in">

The interval for generating contours can be controlled from `Workflow > Edit Variables ` menu command. One can also specify if contour lables are needed, and how dense they should be.

> :bulb: **Tip**: For computational efficiency, boundary and grid data are calculated once and stored. This may some times cause contour plots to NOT respond to new boundary areas created. If this happens, use `Workflow > Clear Calcualted Data` and run again.

<img src="./media/Image 024.png" style="width:7in">



# Generated AutoCAD Plots
[Back to ToC](#table-of-contents)

Contour plots and boundary data can be easily plotted to AutoCAD environment using the `Workflow > Render to AutoCAD` menu command.

<img src="./media/Image 025.png" style="width:7in">

Select the objects to draw to AutoCAD and follow the prompts. For more information and guidance see the [Data Processing and Presetation Section](.\DataProcessing\DataProcesssing).

> :bulb:    **Tip**: Controus are generated to AutoCAD with contour label information. Use the *AutoCAD Addon*  tools to create the labels.


[Back to ToC](#table-of-contents)

END.
 
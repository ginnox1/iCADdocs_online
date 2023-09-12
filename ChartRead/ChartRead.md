# Digital Chart or Graph Reader
[Back to Home](..\index#online-documentation)

ChartView module can quickly digitize charts and read values at desired locations, increasing accuracy and reducing time. Using the tool is intutive. It requires that the source image be orthogonal (i.e., perpendicular abscisa and ordinate axis), and both are at their natural orientation (i.e., abscisa is horizontal, and ordinate is vertical).


## Table of Contents
<!--TOC-->
  - [Seting up and reading charts](#seting-up-and-reading-charts)
  - [Interpolated reading](#interpolated-reading)
  - [Exporting Data](#exporting-data)
<!--/TOC-->


## Seting up and reading charts
 [Back to Toc](#table-of-contents)

To use this module, you will need the image of the chart or graph to read ready in a file or open in some application on the computer. Then follow these steps.

1. Define the session, as you would normally do with any session. Use the standard ChartView host object provided from `Tools > Create Host Objects`. 
     The first time it opens, it displays an empty axis, or blank screen. That is ok.

1. Load the image from `Workflow > Load Image...`.

    <img src="./media/Image 001.png" style="Width:6in">


    > :bulb: **Tip**: Control the visibility of the image (its transparency) from the `Workflow > Variable Editor` by changing *Transparency Value* as desired.

1. Create the reference frame for the data set from `Workflow > Pick BBox Rectangle`. On the image, **click and drag ** from he left-bottom corner of the image to the top-right corner of the image. Start and finish accurately on the limits of the graph area. This will determine the accuracy of the chart reading process later.

1. Go to `Workflow > Variable Editor` and set the data range. Also, specify the scaling for each axis, i.e., whether linear or log.

    <img src="./media/Image 002.png" style="Width:6in">
    
1. Now create the data points. Go to `Workflow > Add Chart Element`. The interface will be in select mode, with a big cross-hair.
 Pick points along the graph representing the line to digitize, and use `Right-Click` to finish input.

     <img src="./media/Image 003.png" style="Width:6in">

The digital copy of the curve line is created using curvilinear interpolation for the data range defined earlier.

1. Edit selection points as needed.
    1. To remove a point, `Right-click` on it, and choose *Remove Point*.
        <img src="./media/Image 009.png" style="Width:3in">

    2. To add a point, `Right-click' on the line (NOT a Point). Use the context menu `Add Point`.



1. Read the graph element from `Workflow > Read Chart`. This will start the reader, with a vertical red line some where at the center. Click on it, and move the mouse to a desired location. The values are interactively displayed for the current location.

    <img src="./media/Image 004.png" style="Width:6in">

    Use the `esc` key to stop interactive reading.

    > :bulb: **Tip** As many chart elements as needed can be digitized in this way, and saved for latter use.

1. Save the work if desired.

## Interpolated reading
 [Back to Toc](#table-of-contents)


The chart reader can interpolate and display values for paramters whose chart if not available. For instance in the current exaple, values are only available for parameters of 1:3, 2: 3 and 3: 3. Interplated reading comes in handy when the user needs values for, say, 1:2.5.

To achieve this, follow below steps.

1. Create the lower and upper bounding charts for the desired value following the above listed steps. For this example, we will need the curves for 3:3 and 2:3.


1. Name the chart elements by right-clicking on each char line, and choosing `Rename`. For each input the name as z3 and z2.

    <img src="./media/Image 011.png" style="Width:3in">


1. Test the input values, by reading the chart from `Workflow > Read Chart`. Make any edits or adjustments needed to get correct results.

    <img src="./media/Image 012.png" style="Width:6in">


1. Go to `Workflow > Variable Editor` and edit the *Z Interpolation Value* parameter. Input 2.5, the desired parameter value needed.

    <img src="./media/Image 013.png" style="Width:4in">

1. Now, start the reader from `Workflow > Read Chart`, and hover arround. The values are interpolated for the desired value and displayed.

    <img src="./media/Image 014.png" style="Width:6in">

> :notebook: **Note**: If more than two series data are found, then the interpolation method used to calcualte the new value will use that specified in the *Variable Editor.*



## Exporting Data
[Back to Toc](#table-of-contents)


If desired, the digitized data points can be exported to the windows clipboard as a list. Right-Click on any one of the chart elements created, and choose *List Series*.

<img src="./media/Image 015.png" style="Width:4in">


Choose desired resolution from the dialog. The data is displayed on the data table viewer interface.

If a list of all chart elements is desired, use the `Workflow > List Elements` menu command, and choose the desired resolution. The data is displayed as needed.

<img src="./media/Image 016.png" style="Width:3n">


[Back to Toc](#table-of-contents)


END.






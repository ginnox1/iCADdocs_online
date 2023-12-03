# iCAD Update Notes (Nov 2023)

[Back to Home](..\index#updates-for-this-release)

**Hello There,** 

Well come to this update. We are excited to bring more functions and features to our users. This release marks a milestone, where we have included new modules for the design of diversion weirs and embankement analysis modules. We have also refined previously existing modules to meet the work needs of practitioners.

The current release is **Version 2.8.3.9040**.

:bulb: **Note:** The release is currently released for validation purposed. It will be available on 06Dec2023.




Key in this release include new modules for diversion weir design and embankment works analysis.

## Table of Contents
<!--TOC-->
  - [Data Table View](#data-table-view)
  - [Retwall Module](#retwall-module)
  - [ChannelRating_WSPRO](#channelrating_wspro)
  - [Diversion Weir Design :new:](#diversion-weir-design-new)
  - [TerraForm module for embankment works analysis :new:](#terraform-module-for-embankment-works-analysis-new)
  - [Advanced Stream rating curve development using WSPRO](#advanced-stream-rating-curve-development-using-wspro)
  - [Enhanced ChartView](#enhanced-chartview)
  - [Support for Latest AutoCAD Releases](#support-for-latest-autocad-releases)
<!--/TOC-->

## Data Table View
iCAD's Data viewer table interface is frequently used to explore data contents of AutoCAD objects. In this update, it can directly call on AutoCAD objects to see if CsvData is hosted and its contents, if any.
* Choose **Tools > Show Csv Data** menu command or the toolbar item to start the command. Go to AutoCAD, and pick the object whose data you want to explore.

	<img src= "./media/Image 004.png" style="width:5in">

## Retwall Module
Retaining wall module is enhanced to indlude the following features, particularly suited for designing long retaining wall.



* New variable included to allow Segment identification from Wall Top and bottom profiles. This is a useful feature giving the user additional flexibility to define and solve practical problems.

	<img src="./media/Image 001.png" style="width:5in">


* New variable included to allow flexible BoQ extraction (summarized or detailed). The summary will generate BoQ for all Segments in the wall.

	<img src="./media/Image 002.png" style="width:5in">


* A new safety criteria included on the Design Scene selector showing trends on eccentriciy and aiding in desin width selection.

	<img src="./media/Image 003.png" style= "width:5in">






## ChannelRating_WSPRO
Recent updates to ChannelRate_WSPRO are included to make the module more interactive and generate rich information to AutoCAD.
The following are key features:
- New variable included to show flood levels for upto two discharges

	<img src="./media/Image24.png" style="width:6in">

- Show the solutoin method used for analysis
- Generate texts and annotations to AutoCAD
    <img src="./media/Image25.png" style="width:6in">
- Improved error handling for disxharge ranges.


	


## Diversion Weir Design :new:
[Back to ToC](#table-of-contents)

A flexible and easy to use diversion weir design module is now integrated and available as part of the Professional iCAD Software edition. It offers up to 8 different views to work with different compoentns of the structure.
<img src="./media/image11.png">

It has the following features:
- Automatic link to channel rating data
- Longitudinal cross-section views across overflow span, sluice bays with piers, and outlets
- Dynamic weir overflow sizing
- Automatic and full stability analysis for the weir body
- Trapezoidal or ogee shaped weir
- Full surface, and sub-surface flow hydraulis, with appron sizing and design features
- and more.

## TerraForm module for embankment works analysis :new:
[Back to ToC](#table-of-contents)

We have designed and implemented an ambitious workflow in formation analysis and work volume estimation for embankement works. TerraForm module builds on previous versions of surface analysis to give users the computational edge and easy workflow to tackle earth work estimation and drawing generation tasks.

<img src="./media/image22.png">

This version includes the follwing features:
- Easy definition of complex shape assemblies
- Parameteric assemblies for even more complex assemblies
- Ability to reduce surfaces (to emulate excavation works), before computing fill works
- Interactive cross-sections
- Full drawing generation capability
- and more.

<img src="./media/image19.png">

## Advanced Stream rating curve development using WSPRO
[Back to ToC](#table-of-contents)

ChannelRating module is upgraded to include complex analyis features that enable determination of a stage discharge curve from multiple river or stream cross-sections. This methos is known to be more accurate than the conventional method that used one cross-section only.

<img src="./media/image16.png" style="width:5in">

This feature is validated using data provided by WSPRO/USGS and found to be accurate. Read the validation document [here]().

<img src="./media/Image 8.png" style="width:5in">

## Enhanced ChartView
[Back to ToC](#table-of-contents)

iCAD introduces a novel and handy solution to digitally read complex charts. Charts of different sorts are used by engineers to determine design paramters or performance data. Often reading these charts are challenging, and subject to significant human error. Where parameteric charts are involved, shch as the one below, the challenge becomes evern more concetning.

ChartView module is enhanced to quickly digitize charts, read interpolated values, and save capability. It also accepts importing chart images from the windows Clipboad.

<img src="./media/Image 1.png" style="width:6in">

In this demo, it was easy to read values for parameter z=2.5, based on values for z=1, 2, and 3.




## Support for Latest AutoCAD Releases
We are continually integrating latest versions of AutoCAD to our products. AutoCAD 2o22 and 23 are now supported with our applications.

> :warning: **NOTE**: The applications are being fully tested on these latest AutoDESK products, and the test is not completed. Please let us know if you encounter any issues, and we will be glad to help.

[Back to ToC](#table-of-contents)

END.

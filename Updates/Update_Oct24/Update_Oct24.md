# iCAD Update Notes (Oct-2024)


**Hello, and welcome again,** 

We are excited to bring more functions and features to our users. This release includes major and minor enhancements to the iCAD product suite - mainly Diversion Weir Design module and Surface modelling modules. Learn about the update features and functions included in this release below.




## Table of Contents

Key in this release include new modules for diversion weir design and embankment works analysis.

<!--TOC-->
  - [What's New](#whats-new)
    - [General](#general)
    - [Surface Modelling](#surface-modelling)
    - [TeraForm](#teraform)
    - [Diversion weir](#diversion-weir)
  - [Support for Latest AutoCAD Releases](#support-for-latest-autocad-releases)
<!--/TOC-->
## What's New

### General
- Data tip in iCAD interface is enhanced to reduce repetition, and show data tips in context.
- Status bar timer is reduced to avoid unwanted interuption to the user when performing different tasks. It can also be set permanently on if needed.
- Removed plot sheet generator funciton (previously designed for CanalNET products).


### Surface Modelling
- Major and minor contours can now be generated in one go, reducing the number of steps needed to achieve a complete presentation drawing.

    <img src="./media/Image 011.png" style="width:6in">

- Production of contour lines to AutoCAD environment now transfers elevation information in both **individual** and **via buffer** options.



- A new algorithm called **GridFit** is included for contour generation. The developers claim that it is a better algorithm that can overcome the inherent limitations of GridContour. It offers better control of smoothness, fail safe computation.

    <img src="./media/Image 009.png" style="width:4in">

    For a quick preview of differences, compare below figure with that shown above.
  
    <img src="./media/Image 010.png" style="width:4in">

Reference: John D'Errico (2024). Surface Fitting using gridfit (https://www.mathworks.com/matlabcentral/fileexchange/8998-surface-fitting-using-gridfit), MATLAB Central File Exchange. Retrieved September 28, 2024.


### TeraForm 

TeraForm module is enhanced as follows:

1. Simplified data input for assemblies and their design levels, and/or tracers. This saves time for inputs of constant value assembly components. The dialog checks automatically user inputs for validity with in the usable elevation range from the cross-section data.

    <img src="./media/Image 012.png" style="width:6in">


1. The same funtion is included for tracer bee inputs as shown below. Here also, automatic data verification is carried out based on the available cross-section data. Both +ve and -ve values are acceptable.

    <img src="./media/Image 013.png" style="width:6in">


1. Additionally, a key enhancement is included to avoid the need to reference assembly elements from AutoCAD. Sloped berms are also acceptable, and the strict requirement to have perfectly horizontal berms is removed.

    <img src="./media/Image 014.png" style="width:4in">


### Diversion weir

1. Added flexibility of design with `Workflow > Relaease pool length` menu command. This command allows interactive positoning for the downstream appron end (applicable for TypeI jumps only).

    <img src="./media/Image 015.png" style="width:6in">

2. Automatic check for Free flow condition at outlet by using modularity ratio. The result is shown in the text summary.

    <img src="./media/Image 016.png" style="width:6in">

3. Improved report contents (removed inconsistencies, and missing values for baffle blocks). 


1. Rating curves are now computed for provided input values and reported accordingly.

    <img src="./media/Image 017.png" style="width:6in">

1. Broad crested weir performance indicator is included, and a text report shown in longitudinal profile view.

    <img src="./media/Image 018.png" style="width:6in">

1. Included a guide marker for cutoff depth fulfilling safe exit gradient criteria in HFL and NPL flow conditions. Similarly, a marker is provided for end of pool location (for Type I jumps).

    <img src="./media/Image 019.png" style="width:6in">

1. Staged bottom profile can now be created by providing the proper option in `Workflow > Variable Editor'.

    <img src="./media/Image 020.png" style="width:6in">

1. An elevation view is introduced for outlets (available for both Left and Right outlets). The variables involved are also reviewd to allow flexible design. A new variable is included for abutment extension length to accomdate longer outlet walls that may be needed.

    <img src="./media/Image 021.png" style="width:6in">

1. A bug is resolved on jump length calculation, maintaining design ONLY for design discharge value. Also improved contents of reports for baffle block designs.


## Support for Latest AutoCAD Releases
[Back to ToC](#table-of-contents)

We are continually integrating latest versions of AutoCAD to our products. AutoCAD 2022 and 23 are now supported with our applications.

> :warning: **NOTE**: The applications are being fully tested on these latest AutoDESK products, and the test is not completed. Please let us know if you encounter any issues, and we will be glad to help.

[Back to ToC](#table-of-contents)

END.

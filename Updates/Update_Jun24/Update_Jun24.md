# iCAD Update Notes (Jun2024)


**Hello, and welcome again,** 

We are excited to bring more functions and features to our users. This release marks a milestone, where we have included new modules for the design of diversion weirs and embankement analysis modules. We have also refined previously existing modules to meet the work needs of practitioners.

The current release is **Version 2.8.3.9270**.

## Table of Contents

Key in this release include new modules for diversion weir design and embankment works analysis.
<!--TOC-->
  - [TerraForm Enhancement](#terraform-enhancement)
    - [Terraform](#terraform)
    - [Diversion Weir](#diversion-weir)
  - [Support for Latest AutoCAD Releases](#support-for-latest-autocad-releases)
<!--/TOC-->

## What's New

### Terraform
[Back to ToC](#table-of-contents)

- A key improvement is made to the algorithm, to allow more complex shapes for defining intricate fill layers that can represent dam/embankment construction design.{br}

    <img src= "./media/Image 001.png">

    The above filter layer is created using an assembly shape in AutoCAD shown below. Such a shape (a fill shape containing positive slope) is now acceptable.


    Key algorithms are improved to better understand complex shapes accurately, and return accurate measures of areas involved.
  
    <img src="./media/Image 6.png" style= "width:7in">



### Diversion Weir
[Back to ToC](#table-of-contents)

- The sub-surface pressure variation algorithm is enhanced to account for interference due to intermediate cutoff walls. Results now show values that are modified accordingly.
<img src="./media/Image 003.png" style="width:6in">

- A new report is included for stilling pools, now generating complete design information for selected energy dissipater mechanism.

    <img src="./media/Image 5.png" style="width:6in">

- Plan views now include detailed energy dissipater block dimension and placement dimension for all jump mechanisms.
  
  <img src="./media/Image66.png">

- Different views of the design session now retain display extents, for smoother navigation experience.


Bug fixes:
- Cd Selection for Ogee shaped weirs
- Subsurface hydraulic calculation, and exit gradient values corrected.
- Report for ogee type weir corrected and displayed
- Hydraulic grade lines for USBR type basins corrected.
- Rare NaN values displayed for prejump depth corrected.



## Support for Latest AutoCAD Releases
We are continually integrating latest versions of AutoCAD to our products. AutoCAD 2022 and 23 are now supported with our applications.

> :warning: **NOTE**: The applications are being fully tested on these latest AutoDESK products, and the test is not completed. Please let us know if you encounter any issues, and we will be glad to help.

[Back to ToC](#table-of-contents)

END.

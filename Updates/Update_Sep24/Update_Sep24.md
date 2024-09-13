# iCAD Update Notes (Sep-2024)


**Hello, and welcome again,** 

We are excited to bring more functions and features to our users. This release marks a milestone, where we have included new modules for the design of diversion weirs and embankement analysis modules. We have also refined previously existing modules to meet the work needs of practitioners.


## Table of Contents

Key in this release include new modules for diversion weir design and embankment works analysis.

<!--TOC-->
  - [What's New](#whats-new)
    - [TerraForm Module](#terraform-module)
    - [ChannelRate_WSPRO](#channelrate_wspro)
    - [DiversionWeir Design Module](#diversionweir-design-module)
  - [Support for Latest AutoCAD Releases](#support-for-latest-autocad-releases)
<!--/TOC-->
## What's New

### TerraForm Module
[Back to ToC](#table-of-contents)

- Improved handling of assembly data from AutoCAD environment. The data filtering is now adjusted to accomodate up +/-1Degree on horizontal berms. PRevious versions used to block assemblies with out perfectly horizontal berms.

    <img src="./media/Image 001.png">
  


### ChannelRate_WSPRO
[Back to ToC](#table-of-contents)

- Corrected legend for rating daata of critical flow and normal flow curves
- Improved interpolation method implemented, avoiding variations noted when plotting discharge curves
- Improved menu interaction with different view modes. A short cut is also included for the menu command `Workflow > Manage Stream Profile...` to allow fast access to manage multiple cross-sections import and editing.

    <img src="./media/Image 002.png">

    <img src="./media/Image 003.png">



### DiversionWeir Design Module
[Back to ToC](#table-of-contents)

This module is evolving to accomodate more functionality needs, as we continue to test it for verificaiton and application to real world projects. In this release:

- Inputing a list of discharge values is now possible, that are used upstream rating curve generation and outlet design works effectively.

    <img src="./media/Image 007.png">


- Additional design guides included to show broad-crested weir flow limits, and downstream cutoff wall depth limits.

    <img src="./media/Image 005.png">

    <img src="./media/Image 006.png">


- Easier navigation between transverse view and longitudinal view, using Ctrl+T and Ctrl+L keyboard shortcuts.

    <img src="./media/Image 008.png">


## Support for Latest AutoCAD Releases
[Back to ToC](#table-of-contents)

We are continually integrating latest versions of AutoCAD to our products. AutoCAD 2022 and 23 are now supported with our applications.

> :warning: **NOTE**: The applications are being fully tested on these latest AutoDESK products, and the test is not completed. Please let us know if you encounter any issues, and we will be glad to help.

[Back to ToC](#table-of-contents)

END.

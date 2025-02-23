# iCAD Update Notes (February 2025)



**Hello, and welcome again,** 

We are excited to bring more functions and features to our users. This release includes major and minor enhancements to the iCAD product suite - mainly Data Processing tools, Diversion Weir Design and TeraForm modules.

Learn about the update features and functions included in this release below.


## Table of Contents

<!--TOC-->
  - [Update to Current Release](#update-to-current-release)
  - [What's New](#whats-new)
  - [General](#general)
  - [Terraform](#terraform)
  - [ChannelRate](#channelrate)
  - [Bug Fixes](#bug-fixes)
<!--/TOC-->


## Update to Current Release

The current release of iCAD Software is **Version 2.9.0.10683**. 

The acompanying iCAD Bridge application version is **Version 4.9.5**


> IMPORTANT: Make sure AutoCAD is closed when updating. If not, the update process will fail to install the latest resources. We encourage you to review below links for guidance on how to install updates.

Follow below steps to update your installation to the latest release:


* **Download** the [Latest update Resource for iCAD Software](https://drive.google.com/uc?export=download&id=1mSZVIIXOgk0yGErVAzAHIH8eWm1x0gZ6)


* Follow the update instructions [Installing Update Resources here](SetupAndLicensingGuide/setupguide.md#installing-update-resources) to update your application. 

**NB:** If you encounter issues on licensing and installation, You can find guidelines following the steps in the **Introduction to iCAD Software** document, chapter on [Setup And Licensing Guide](SetupAndLicensingGuide/setupguide.md#installation-and-setup-guide)

## What's New
For this update the following major functionalities and capabilities are included, along with some bug fixes.


## General

1. Session defintion process is enhanced with a feature to apply host sketches on the fly.


     <img src="./media/Image 004.png" style="width:4in">

    


    The sketch and user defined tag are applied upon setting the Object Types for the session.
      
   <img src="./media/Image 005.png" style="width:4in">

 
     Note: Surface data host sketches are automatically applied upon hosting valid data to objects.

     This reduces modelling time, and improves efficiency.


## Terraform
[Back to ToC](#table-of-contents)

1. Design level values are displayed on Elevation view.
    
    <img src="./media/Image 006.png">

    Similarly, on a cross-seciton view, elevation values are displayed.

   
   <img src="./media/Image 10.png" style="width:6in">


1. Teraform is enhanced to allow generation of multiple cross-sections to AutoCAD at once. 

    <img src="./media/Image 008.png" style="width:5in">


1. In addition to enhanced color management tool (started in previous update), save as feature is included and enhanced.

    <img src="./media/Image 009.png" style="width:5in">

    This allows working on, and comparing, different models of the same design problem. Giving users maximum flexibility.




## ChannelRate
[Back to ToC](#table-of-contents)



1. Allow release flood mark levels (variable editor now accepts 0 value)

    <img src="./media/Image 001.png">

1. Show water levels in multiple sections, if available. This updae shows water surface levels in sections other than the base cross-section, if the multiSection method is used to solve for the rating curve.

    <img src="./media/Image 002.png">

   *Figure: showing a cross-section downstream, but solved with Manning's method.*

 1. Enhanced visual to identify if current displayed cross-section is the base cross-section or not. Those other than base cross-section are now drawn in broken lines. The water surface level and shades are also lightened a bit for better visualization.
 
     <img src="./media/Image 003.png">

 




## Bug Fixes
[Back to ToC](#table-of-contents)


- Data and AutoCAD object selection handling refined.





END.
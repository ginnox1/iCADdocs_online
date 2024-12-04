# iCAD Update Notes (Dec-2024)


**Hello, and welcome again,** 

We are excited to bring more functions and features to our users. This release includes major and minor enhancements to the iCAD product suite - mainly Data Processing tools, Diversion Weir Design and TeraForm modules.

Learn about the update features and functions included in this release below.


## Table of Contents

Key in this release include new modules for diversion weir design and embankment works analysis.

<!--TOC-->
  - [Update to Current Release](#update-to-current-release)
  - [What's New](#whats-new)
  - [Data Processing](#data-processing)
  - [Terraform](#terraform)
  - [Surface Data Processing, Profile Extraction](#surface-data-processing-profile-extraction)
  - [ChannelRate](#channelrate)
  - [Diversion Weir Design](#diversion-weir-design)
  - [Bug Fixes](#bug-fixes)
<!--/TOC-->


## Update to Current Release

The current release of iCAD Software is **Version 2.9.0.10464**. 

The acompanying iCAD Bridge application version is **Version 4.9.5**


> IMPORTANT: Make sure AutoCAD is closed when updating. If not, the update process will fail to install the latest resources. We encourage you to review below links for guidance on how to install updates.

Follow below steps to update your installation to the latest release:


* **Download** the [Latest update Resource for iCAD Software](https://drive.google.com/uc?export=download&id=1mSZVIIXOgk0yGErVAzAHIH8eWm1x0gZ6)


* Follow the update instructions [Installing Update Resources here](SetupAndLicensingGuide/setupguide.md#installing-update-resources) to update your application. 

**NB:** If you encounter issues on licensing and installation, You can find guidelines following the steps in the **Introduction to iCAD Software** document, chapter on [Setup And Licensing Guide](SetupAndLicensingGuide/setupguide.md#installation-and-setup-guide)

## What's New
For this update the following major functionalities and capabilities are included, along with some bug fixes.

## Data Processing
[Back to ToC](#table-of-contents)

- Apply host sketches in process, removing the need to manually change them after/before session definition, and improving speed.

    <img src="./media/Image 2.png">


- Additional options to plot to AutoCAD, allowing more flexibility in drawing generation from iCAD environment.

    <img src="./media/Image 1.png">


## Terraform
[Back to ToC](#table-of-contents)

1. Overhaul assembly editor interface for greater flexibility in defining, editing and visualizing assembly information.

    <img src="./media/Image 14.png">

    Two key functionalities are
    - ability to manage visuals with speed (not requiring to go to the main interface)
    - ability to assign and edit materials, allowing flexible area calculation and extraction to bill of quantity.

2. Bill of quantity generation capabilty included, collecting zone items by material is possible for seamless quantity extraction.

    <img src="./media/Image 15.png">


2. Editing design level source objects (CAD) now made possible, greately improving efficiency and speed of assembly definition and editing processes.


2. Capability to process subsurface layer/zone information integrated, allowing extraction of volumes by material.

    <img src="./media/Image 16.png">

4. Enhanced plan view with major and minor contours, and different alpha values for better visual presentation.

    <img src="./media/Image 17.png">


5. Reduced assembly approximation tolerance to 1/10th of a milimeter, to allow more precise profile creation and quantity estimates.

    
    <img src="./media/Image 18.png">

6. Check for existing names before accepting new assembly data.

    <img src="./media/Image 19.png">
    
7. Abilityy to generate plan view from modified ground level, a key feature for realistic representation of expected construction processes and resulting formation of fill works.


Imrpoved and accurate cross-sections (removng discontinuities)



## Surface Data Processing, Profile Extraction
[Back to ToC](#table-of-contents)

1. Allow collecting cross-sections on plan view, for further processing (e.g., Channel Rating)

    <img src="./media/Image 6.png">

    The cross-sections can be viewed in a separate viewer.

    <img src="./media/Image 7.png">

2. Improved algorithm to handle contour creation for multiple regions of interest

    <img src="./media/Image 10.png">


3. Contour labels algorithm applies on existing contour

   <img src="./media/Image 12.png">

4. Show traingulation along with area statistics

    <img src="./media/Image 11.png">


5. Contour labels in AutoCAD are now grouped for easy editing and processing.

    <img src="./media/Image 13.png">




## ChannelRate
[Back to ToC](#table-of-contents)

1. 1. Direct access to cross-section data saved on workspace to populate multiple cross-sections downstream or upstream, significantly reducing the time needed to model multi-section water surface profile computation.

    <img src="./media/Image 8.png">






## Diversion Weir Design
[Back to ToC](#table-of-contents)

1. A major feature is added to DiversionWeir Design module allowing transfer of data with Retwall design module and back. This feature makes design processes complete and easy to manage.

    <img src="./media/Image 20.png">




## Bug Fixes

- Terraform - crosssection discontinuities resolved on section view generation for plotting to AutoCAD.
- TerraForm Failing interpolation on vertical elements of an assembly, resolved.
- Terraform Improved cross-section Fix area addition, subtraction algorithm



[Back to ToC](#table-of-contents)

END.
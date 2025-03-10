# iCAD Update Notes (March 2025)



**Hello, and welcome again,** 

We are excited to bring more functions and features to our users. This release includes major and minor enhancements to the iCAD product suite - mainly Data Processing tools, Diversion Weir Design and TeraForm modules.

Learn about the update features and functions included in this release below.


## Table of Contents

<!--TOC-->
  - [Update to Current Release](#update-to-current-release)
  - [What's New](#whats-new)
  - [Terraform](#terraform)
  - [ChannelRate](#channelrate)
  - [Bug Fixes](#bug-fixes)
<!--/TOC-->
## Update to Current Release

> IMPORTANT: Make sure AutoCAD and iCAD is closed when updating. If not, the update process may fail to install the latest resources. We encourage you to review below links for guidance on how to install updates.


<div style="max-width: 600px; margin: 2rem auto; padding: 2rem; background: #f8f9fa; border-radius: 12px; box-shadow: 0 4px 6px rgba(0,0,0,0.1); text-align: center;">
  <h2 style="color: #2d3436; margin-bottom: 1rem; font-family: 'Arial', sans-serif;">
    📅 Latest Monthly Package
  </h2>
  
  <p style="color: #636e72; margin-bottom: 1.5rem; line-height: 1.6;">
    Get the recent updates for your system. This month's release includes:<br>
    • New features to modules, and <br>
    • Bug fixes and optimizations<br>

  </p>

  <a href="https://drive.google.com/uc?export=download&id=1mSZVIIXOgk0yGErVAzAHIH8eWm1x0gZ6" 
     style="display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 12px 24px;
            background: #0984e3;
            color: white;
            border-radius: 8px;
            text-decoration: none;
            transition: transform 0.2s ease;
            font-weight: 500;"
     onmouseover="this.style.transform='translateY(-2px)'"
     onmouseout="this.style.transform='translateY(0)'">
    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
      <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
      <polyline points="7 10 12 15 17 10"></polyline>
      <line x1="12" y1="15" x2="12" y2="3"></line>
    </svg>
    Download Update
  </a>

  <p style="margin-top: 1.5rem; color: #636e72; font-size: 0.9em;">
    🔖 Version 2.9.10354 | 📦 ~20Mb | ✅ Verified Build
  </p>
</div>

* Follow the update instructions [Installing Update Resources here](SetupAndLicensingGuide/setupguide.md#installing-update-resources) to update your application. 

* **NB:** This update requires, reinstalling iCAD application. Download from the link below.For guidance on installation, You can find guidelines following the steps in the **Introduction to iCAD Software** document, chapter on [Setup And Licensing Guide](SetupAndLicensingGuide/setupguide.md#installation-and-setup-guide)

    [![Download](https://img.shields.io/badge/Download-iCAD%20Installer-blue?style=for-the-badge&logo=google-drive)](https://drive.google.com/uc?export=download&id=1GpF1l7ovDPOa6QWdov8uqKWfcsfjy8M4)



## What's New
For this update the following major functionalities and capabilities are included, along with some bug fixes.


## Terraform
[Back to ToC](#table-of-contents)

1. A new feature is integrated, that allows to incoproporate cap levels for volume calculation. The command is available from the workflow menu, as shown below.

    <img src="./media/Image 001.png" style="width:6in">

    Users can define design levels either from AutoCAD or provide a fixed elevation value for cap level information.

2. Updates to allow volume extraction using cap levels. Cap levels can be toggled on to generate new volume informaitons considering defined cap levels.

     <img src="./media/Image 002.png" style="width:6in">

     The fill volumes are calcualted for each zone below the cap level at the station of interest.
 
     <img src="./media/Image 003.png" style="width:6in">

3. A new feature is included to process two assemblies, and extract geometries. This feature allows versatility in defining complex assembly shapes.

    
     <img src="./media/Image 004.png" style="width:6in">

     THe results are presented on the table view interface as shown below. These can be copied and directly applied as tracer bees. Alternatively, they can be processed further in a spreadsheet application and used as tracer data.
    
      <img src="./media/Image 005.png" style="width:6in">

 4. Related feature allowing the use of table data as tracer bee sources, to define complex shapes.

    <img src="./media/Image 006.png" style="width:6in">

    With this method complex shapes can be modelled effectively.

    <img src="./media/Image 007.png" style="width:6in">




## ChannelRate
[Back to ToC](#table-of-contents)


1. The multiple cross-sectoin manager now displays segment slope information automatically, providing additional guide to the user.

    <img src="./media/Image 008.png" style="width:6in">

2. A new button is included to import bed level information, and auto genrate average slope information from the data.

    <img src="./media/Image 009.png" style="width:6in">




## Bug Fixes
[Back to ToC](#table-of-contents)


- Major compatibility issue fixed.
- Data and AutoCAD object selection handling refined.


END.
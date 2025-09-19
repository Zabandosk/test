

# FILE ORGANISATION SCHEME
## FILE NAMING

File names can carry important information about the file itself, without needing to open it or read documentation. The main types of information a file name can convey include the date, the collection or group it belongs to (if any), the file’s title, the initials of the person who prepared it, and the version number.

Here is an example format:
yyyymmdd_Group_Title_Initials_version.format
20250806_GAM_SitePoints_LB_v01.shp

The reason for using the year-month-day system (YYYYMMDD) is to ensure that files are sorted chronologically when read by machines, since sorting is typically done from left to right. Using this naming system will help your files be ordered automatically by date.
Avoid using spaces and special characters (such as ^, &, %, ‘, “ etc.) in file and folder names. These may prevent systems from detecting or reading the files correctly, and in some cases, files may not upload or be analysed properly, especially when you're dealing with a large number of files. This is also a common reason for issues with Arches when reading spreadsheet cells that include such characters.

If you have a good version of a file and later need to make even a small change, always create a new copy. This way, if something goes wrong in the new version, you still have the previous, working version saved.
These file naming standards can be applied to all types of data and are especially useful during ongoing work, as they make it easier to manage files on the path to a final version.
In special cases, such as image files or resources related to a site where you are not the file’s creator, there is no need to include the creation date, initials, or version number. Instead, you can assign a unique ID and a short descriptive name to improve findability.

Example:
GAM-MED-000001_Wassu01.jpg
GAM-MED-000002_Wassu02.jpg

This approach avoids long names, spaces, and special characters, making your file names machine-readable and ensuring compatibility with Arches and other systems.
The same logic applies to other information resources, e.g.:
GAM-RES-000001_TitleOfDocument.pdf

## FOLDER HIERARCHY

There are two main categories of data you will produce during the process:

Heritage Data, which includes:
Sites
Remote Sensing
Media (e.g. images)
Resources

Documentation, which includes:
Reports
Feedback
Dataset Details
Templates

Organizing your data in this way makes it easier to manage. Below is a brief overview of what kind of information should be in each folder and the formats expected, to help me check and prepare the data for final delivery.

### HERITAGE DATA
This is the main group containing files and folders that represent heritage data in various formats and types.

#### Sites
Includes a Metadata folder (for spreadsheets) and a Geometry folder (for spatial data).
In the Metadata folder, the working file should be in .xlsx format and named like:
yyyymmdd_GAM_SiteMetadata_LB.xlsx
Geometry/Points, Geometry/Polygons and Geometry/Lines folders must include each of the following file formats:
.cpg, .dbf, .prj, .shp, .kml
Each folder must have subfolder named as, so that we can follow the same 
Example:
yyyymmdd_GAM_SitePoints_LB.dbf
yyyymmdd_GAM_SitePolygons_LB.shp
…
#### Remote Sensing
Same structure as Sites: contains Metadata and Geometry folders.
Metadata folder requires .xlsx as format and naming should be similar, just different in the title of the document part with RS (short for Remote Sensing).
yyyymmdd_GAM_RSMetadata_LB.xlsx
Geometry has two subfolders: Points (for specific locations) and Footprints (for area coverage). Files should follow the same naming conventions and formats  as above.
Each folder has subfolder named as, so that we can follow the same 
	yyyymmdd_GAM_ RSPoints_LB
Files in “Geometry/Points” should be named as:
yyyymmdd_GAM_RSPoints_LB.cpg
yyyymmdd_GAM_RSPoints_LB.dbf
…
Files in “Geometry/Footprints” should be named as:
yyyymmdd_GAM_RSFootprints_LB.cpg
yyyymmdd_GAM_RSFootprints_LB.dbf
…
#### Media
Used for images or maybe for other media files in the future (e.g. 3D models, videos, audio).
Contains a metadata spreadsheet:
01_GAM_MediaMetadata_LB.xlsx
(Using 01_ ensures it appears at the top of the folder list.)
Media files should be named with unique IDs:
GAM-MED-000001_Wassu01.jpg
For now, considering the limited time, you may upload your files as they are. Just ensure they are in one of the accepted formats: .jpg, .jpeg, .png, .tiff.
#### Resources
This folder includes source materials used while creating your metadata.

Requires a metadata file:
01_GAM_ResourceMetadata_LB.xlsx
Documents should be stored in open, sustainable formats like .pdf, .pdf/a, .csv, .jpg, .jpeg, .png, .tiff, depending on content.
Example:
GAM-RES-000001_TitleOfResource.pdf
Since you're also using Zotero, and I’m not fully familiar with your setup, feel free to drop the documents directly for now.

### DOCUMENTATION

This main group is for related documents for your heritage data which enable us to communicate during the process and learn more about the dataset you manage. 
#### Dataset Details
Dataset details is a required document. It should include:
Responsible person(s)
Contact information
Dataset description (number of files, formats, associated media, etc.)
Access and rights information
This document allows me, or any future archaeologist, archivist, or even yourself, to understand the contents of your dataset. It also helps you keep track of your progress, especially when returning to the project after some time away.
Use .docx during drafting and save the final version as .pdf or .pdf/a.
Naming example:
yyyymmdd_GAM_DatasetDetails_LB.pdf

#### Feedback
This is where both of us will leave feedback.
I will upload my reviews and feedback on specific files to this folder.
Renier may also add feedback on Arches ingestion results.
Feedback files should be named similarly to the original file, with “Feedback” and initials added.
Examples:
yyyymmdd_GAM_SiteMetadata_Feedback_OU.pdf
yyyymmdd_GAM_SiteMetadata_Feedback_OU.xlsx
My current feedback file on your Arches manual entries will be shared as:
20250807_GAM_ArchesManualEntry_Feedback_OU.pdf

#### Templates
Contains the latest versions of metadata schemas for:
Sites
Remote Sensing
Media
Dataset Details
Please check this folder regularly to ensure you are using the correct version. I will also update you if we created new versions of our templates.

#### Reports
This folder is for:
Major updates about data lifecycle stages
Virus scan reports
Checksum reports (data integrity)
You can skip this for now (Phase 1), but it's important for later phases.
 
HIERARCHY TREE
Here is the link for the sample folder: https://drive.google.com/drive/u/1/folders/1QStNkjUmF8AfAXeaEsC48V0jMpJlGpzi
Here is a way to show the structure:
PHASE 1
---GAM (Folder)
------Heritage Data (Folder)
---------Sites (Folder)
------------Geometry (Folder)
---------------Points (Folder)
------------------yyyymmdd_CountryCode_SitePoints_PersonInitials.cpg
------------------yyyymmdd_CountryCode_SitePoints_PersonInitials.dbf
------------------yyyymmdd_CountryCode_SitePoints_PersonInitials.prj
------------------yyyymmdd_CountryCode_SitePoints_PersonInitials.shp
------------------yyyymmdd_CountryCode_SitePoints_PersonInitials.kml
---------------Polygons (Folder)
------------------yyyymmdd_CountryCode_SitePolygons_PersonInitials.cpg
------------------yyyymmdd_CountryCode_SitePolygons_PersonInitials.dbf
------------------yyyymmdd_CountryCode_SitePolygons_PersonInitials.prj
------------------yyyymmdd_CountryCode_SitePolygons_PersonInitials.shp
------------------yyyymmdd_CountryCode_SitePolygons_PersonInitials.kml
---------------Lines (Folder)
------------Metadata (Folder)
---------------“yyyymmdd_CountryCode_SiteMetadata_PersonInitials.xlsx”
---------Remote Sensing (Folder)
------------Metadata (Folder)
---------------“yyyymmdd_CountryCode _RSMetadata_PersonInitials.xlsx”
------------Geometry (Folder)
---------------Points (Folder)
------------------yyyymmdd_CountryCode_RSPoints_PersonInitials.cpg
------------------yyyymmdd_CountryCode_RSPoints_PersonInitials.dbf
------------------yyyymmdd_CountryCode_RSPoints_PersonInitials.prj
------------------yyyymmdd_CountryCode_RSPoints_PersonInitials.shp
------------------yyyymmdd_CountryCode_RSPoints_PersonInitials.kml
---------------Footprints (Folder)
------------------yyyymmdd_CountryCode_RSFootprints_PersonInitials.cpg
------------------yyyymmdd_CountryCode_RSFootprints_PersonInitials.dbf
------------------yyyymmdd_CountryCode_RSFootprints_PersonInitials.prj
------------------yyyymmdd_CountryCode_RSFootprints_PersonInitials.shp
------------------yyyymmdd_CountryCode_RSFootprints_PersonInitials.kml
---------Media (Folder)
------------yyyymmdd_CountryCode_MediaMetadata_PersonInitials.jpg
------------MediaID_MediaName.jpg
---------Resources (Folder)
------------yyyymmdd_CountryCode_ResourceMetadata_PersonInitials.jpg
------------ResourceID_TitleOfResource.pdf
------Documentation (Folder)
---------Dataset Details (Folder)
---------Reports (Folder)
---------Feedback (Folder)
---------Templates (Folder)

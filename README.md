# LICSS
##Introduction

The *LICSS System (Excel-CDK)* constructs a bridge between MS Excel for Windows and the Chemistry Development Kit (CDK) Java code tools enabling users to chemically enable existing spreadsheets which contain representations of chemical structures as SMILES strings.

Once enabled, Excel spreadsheets have easy access to CDK functionality currently (v3.2) including Structure Display, Substructure/Similarity searching, R Group Table creation, Clustering, Diverse Compound Picking, Sammon Projections, Molecular Property calculation, SDF file import/export, Library enumeration and Name to Smiles conversion.  Structure display is activated by directly selecting cells containing SMILES strings but also by mouse hover over chart points charting data from an enabled spreadsheet.  Structures are displayed in a pop-up Java window using CDK/J Chem Paint rendering capabilities.  In version 2.0 onwards, this window may be resized/repositioned by the user and its new setting will be remembered for the current Excel session. Display of *all* structures on enabled worksheets is available as a toggle.

Substructure searching of very large spreadsheets may be speeded up by pre-calculation of CDK fingerprints (which are stored compactly in the sheets as hex strings).  In this way, substructure searching of sheets containing many tens of thousands of structures is eminently feasible (tested with 250k structures).

The system requires no installation beyond file copying and the full installer exe file will normally run even on 'locked-down' workstations.

## Downloads
(Please click [Releases](https://github.com/KevinLawson/excel-cdk/releases) for the latest full-installer and source code downloads

## Latest News
*_New (May 2015)_*:
Project now moved to GitHub. Use the Releases feature to get hold of the latest version (3.2 - Installer and Source Code)

*_New (January 2015)_*:
Google drive now contains zip file with all the source code for LICSS 3.2 together with build instructions

*_New (November 2014)_*:
LICSS 3.2 has been upgraded to work with 64bit versions of MSExcel in addition to the 32bit versions. Only tested on one machine so far so feedback very welcome!

*_New (September 2014)_*: 
Development version of LICSS 3.2 is now available on the Google Drive. This uses the latest development version of the CDK and provides for very much faster substructure searching and support for chiral representation of molecules and chiral substructure searching

February 2014: LICSS 3.1 is now stable. Please download from the google drive (link below) as the version under 'Downloads' is no longer current

December 2013: As of January 15th 2014, Google Projects is no longer supporting new project downloads. From this date, the latest LICSS downloads will be available here:

https://drive.google.com/folderview?id=0BxMZMNsy7g3oRkx0Rl9aQUtPSG8&usp=sharing

November 2013: Version 3.1 now available as a development version. New features include a modelling capability (using Support Vector Machines) and the display of the biggest element of 'dot disconnect' Smiles structures. The installer now prompts for an install directory (to help those users who don't have C: drive write access). The NSIS installer is now the only supported way of installing LICSS - redundant features such as self-installation from a local share or from the internet have been removed. Please feedback via the user group on whether this version works for you or if you have any problems with it.

July 2013: Version 3.0 now stable.

June 2013: Update of development version 3.0 now has enumeration facilities for libraries. Extra error-checking gives better stability - worth updating. Hope to provide final version shortly.

March 2013: Version 3.0 of LICSS is now available as a development version. Version 3.0 has the same functionality as version 2.3. However, instead of copying code to enabled workbooks, a single Excel AddIn is installed and enabled workbooks contain no code (and so may be stored in the macro-free formats such as .xlsx). To try this out, run the installation program (with Excel closed) then, to enable workbooks, just press <Ctrl E> and label columns containing Smiles by selecting them and choosing <Ctrl Shift M>. The implementation of LICSS as an AddIn has several advantages such as avoiding the security issues referred to in [GettingStarted] and avoiding the need to close and open workbooks every time new worksheet/chart elements are enabled.

March 2013: Version 2.3 of LICSS is now available as development version. Changes include ability to visualise multiple columns of Smiles, better SD File export, and 'One Time' enabling in which an entire workbook is enabled as a single operation and any sheets containing the sheet name Smiles (and all associated charts) are automatically LICSS aware

July 2012: Version 2.2 of LICSS is released.  New functionality includes import/export of SD files and improvements to structure display and R Group Table creation.  The Names to Smiles facility has been expanded to optionally use the CIR lookup web service enabling conversion of, for example, CAS numbers to Smiles strings.

February 2012: LICSS paper published in the Journal of Cheminformatics: http://www.jcheminf.com/content/4/1/3 (Nb - referred to LICSS 1.x versions)

Slides from lecture given to the MIOSS meeting at EBI:
http://www.hinxton.wellcome.ac.uk/advancedcourses/MIOSS%20Kevin%20Lawson.pdf

Take a look at a 'taster' video for LICSS 2.1: http://www.screencast.com/t/Oy1cwtO0ht

Version 2.1 of LICSS was released 10 October 2011. This adds Similarity searching and new Diverse Compound Picking functionality to that of version 2.0.  There are several bug fixes also including more robust structure display toggling and eliminating Excel crashes caused by attempted multiple initialisation.

Version 2.0 of LICSS was released 1 August 2011.  This uses a new method for calls to Java where Java Classes are proxied in a CPP Dll.  This allows very fast access to CDK/J Chem Paint functionality and has made possible on-the-fly visualisation of structures for all visible Smiles strings on a worksheet.  Excel functions to calculate molecular properties (using the new technology) have also been introduced.  Other new features include conversion of IUPAC names to Smiles and automatic LICSS installation for shared workbooks _via_ download from this project site.

## Limitations
LICSS only currently works with 32 bit MS Excel for Windows (although there is no reason why the code could not be adapted for other operating systems).  See also section on compatibility within GettingStarted https://github.com/KevinLawson/excel-cdk/blob/master/wiki/GettingStarted.wiki.

## Security Errors when using LICSS
LICSS needs your Excel security settings to be set correctly to allow it to work properly.  If you get a runtime error when trying to use it which appears to be security related then take a look at [GettingStarted](https://github.com/KevinLawson/excel-cdk/blob/master/wiki/GettingStarted.wiki)

## Contact
You are welcome to contact the developer with issues, suggestions and comments: kevin.lawson@syngenta.com.  Better still, join and post to the new Google Group for the project: [https://groups.google.com/forum/?fromgroups#!forum/licss-users].

New code created by Syngenta Ltd and licensed under GPL v2

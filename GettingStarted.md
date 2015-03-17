# Introduction #

How to get started with the **LICSS System**

# Details #

  1. Download and run **LICSS-3.2-FullInstaller.exe**
  1. Open the spreadsheet you want to enable in MS Excel and select <Ctrl E>...

You might like to have a look at the IntroductoryVideo showing the features of the system and how to use them (though please note that this was made with version 1.0 and does not show all the more recent features).  Alternatively have a look at the taster video: http://www.screencast.com/t/Oy1cwtO0ht. Note that both these videos feature versions of LICSS in which code is copied to the enabled workbook - the enabling process (with the LICSS AddIn) no longer requires selection of sheets/charts.

# Links for Previous Version support files #

**For version 2.0**

[Version 1.4.0 of the CDK](http://sourceforge.net/projects/cdk/files/cdk/1.4.0/cdk-1.4.0.jar/download)

[Version 3.1.3 of J Chem Paint](http://sourceforge.net/projects/cdk/files/JChemPaint%20%28development%29/3.1.3/jchempaint-3.1.3.jar/download)

[Version 1.0.0 of Opsin](https://bitbucket.org/dan2097/opsin/downloads/opsin-1.0.0-jar-with-dependencies.jar)

**For version 1.1**

[Version 1.2.5 of the CDK](http://sourceforge.net/projects/cdk/files/cdk/1.2.5/cdk-1.2.5.jar/download)

[Version 2.4.0 of the J Chem Paint Applet](http://sourceforge.net/projects/cdk/files/JChemPaint/2.4.0/jchempaint-applet-2.4.0.zip/download)

# Security Issues #
LICSS uses VBA code ('macros') and so needs macros enabled for any LICSS sheet to work.  In addition, **for version 2.3 and below**, if you are enabling your own spreadsheets, then LICSS needs 'Programmatic access to the VBA Project Model' (the ability to create code from VBA).  If you get the error described above ("Runtime error '1004': Programmatic access to Visual Basic Project not trusted") then
(for Excel 2010) select the Office button (top left), then Excel Options - Trust Center - Trust Center Settings - Macro Settings.  Under Macro Settings, check the box for 'Enable All Macros' and under Developer Macro Settings, check the box for 'Trust access to the VBA project model'.  This will allow LICSS to copy the necessary code to your workbook.  In other versions of Excel the fix is similar (under Excel - Options)

# Compatibility #

LICSSV3.2.xla was written in 32 bit MS Excel 2010 for Windows. It has been tested with MS Excel 2003 running under Windows XP, with MS Excel 2010 running under Vista and with MS Excel 2013 (32 bit and 64 bit versions) running under both Windows 7 and Windows 8.

The main Excel enabling file for versions 2.3 and below, `EnableChemicalSpreadsheet(v#).xls` was written using MS Excel 2007 for Windows.  It is saved in Excel for Windows, 1997-2003 format.  The system has been tested with Excel 2007 running under Windows Vista and with Excel 2000 and Excel 2003 running under Windows XP and Windows 7 (64 bit)
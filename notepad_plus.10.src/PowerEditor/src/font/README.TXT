======================================================================
  Microsoft(R) Product Support Services Application Note (Text File)
              GC0651: MS(R) LineDraw (TrueType[TM]) Font
======================================================================
                                                   Revision Date: 1/93
                                                         Disk Included

The following information applies to Microsoft Word for Windows(TM)
version 2.0.

 --------------------------------------------------------------------
| INFORMATION PROVIDED IN THIS DOCUMENT AND ANY SOFTWARE THAT MAY    |
| ACCOMPANY THIS DOCUMENT (collectively referred to as an            |
| Application Note) IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY      |
| KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING BUT NOT LIMITED TO    |
| THE IMPLIED WARRANTIES OF MERCHANTABILITY AND/OR FITNESS FOR A     |
| PARTICULAR PURPOSE. The user assumes the entire risk as to the     |
| accuracy and the use of this Application Note. This Application    |
| Note may be copied and distributed subject to the following        |
| conditions: 1) All text must be copied without modification and    |
| all pages must be included; 2) If software is included, all files  |
| on the disk(s) must be copied without modification [the MS-DOS(R)  |
| utility DISKCOPY is appropriate for this purpose]; 3) All          |
| components of this Application Note must be distributed together;  |
| and 4) This Application Note may not be distributed for profit.    |
|                                                                    |
| Copyright 1993 Microsoft Corporation. All Rights Reserved.         |
| Microsoft, MS, and MS-DOS are registered trademarks and Windows    |
| is a trademark of Microsoft Corporation.                           |
| TrueType is a trademark of Apple Computer, Inc. DisplayWrite is a  |
| registered trademark of International Business Machines            |
| Corporation. WordPerfect is a registered trademark of WordPerfect  |
| Corporation.                                                       |
 --------------------------------------------------------------------

INTRODUCTION
============

This package contains the latest update of the MS LineDraw font for
Microsoft Word for Windows. This is the first update of the MS
LineDraw font since Word for Windows version 2.0 was released in
October 1991. The update consists of a TrueType version of the MS
LineDraw (TrueType) font and a complete extended ASCII (code page 437)
symbol set.

If this shipment has arrived in unsatisfactory condition or you have
questions about installing or using the MS LineDraw (TrueType) font,
please call Microsoft Product Support Services (PSS). In the United
States, call (206) 462-WORD between 6:00 A.M. and 6:00 P.M. Pacific
time. Outside the United States, contact the Microsoft subsidiary for
your area. To locate your subsidiary, call Microsoft International
Customer Service at (206) 936-8661.

  NOTE: To use the MS LineDraw (TrueType) font, you must be running
  Microsoft Windows version 3.1 or later and Word version 1.0 or later
  for Windows.

Once you install the MS LineDraw (TrueType) font, Word versions 2.0
and later for Windows will convert line-draw fonts in Word for MS-DOS,
WordPerfect(R), and RFT-DCA documents to the new MS LineDraw
(TrueType) font. Using the new MS LineDraw (TrueType) font may help
decrease printing time for documents that are converted to Word for
Windows from the Word for MS-DOS, WordPerfect, and RFT-DCA formats if
the documents contain a significant number of line-drawing characters.

TO UPDATE THE MS LINEDRAW (TRUETYPE) FONT
=========================================

1. Insert the enclosed GC0651 disk in your floppy disk drive.

2. At the MS-DOS command prompt, type the following and press ENTER
      
      copy <drive>:\linedraw.ttf <destination>
   
   where <drive> is the floppy disk drive containing the GC0651 disk
   and <destination> is the drive and directory where your Windows
   SYSTEM subdirectory is located. For example, if your Windows
   directory is named WINDOWS and is on drive C and the GC0651 disk is
   in drive A, type the following command:
      
      copy a:\linedraw.ttf c:\windows\system

3. From the Main group in Windows Program Manager, choose the Control
   Panel icon.

4. In the Control Panel window, choose the Fonts icon.

   The Fonts dialog box appears.

5. Choose the Add button.

   The Add Fonts dialog box appears.

6. From the Directories list, select the Windows SYSTEM subdirectory.

   All fonts in the SYSTEM subdirectory appear in the List Of Fonts
   box.

7. From the List Of Fonts box, select the font named MS LineDraw
   (TrueType).

8. Choose the OK button to add the MS LineDraw (TrueType) font.

9. Choose the Close button to exit the Fonts dialog box.

Once the new font is installed, you can remove the MS LineDraw (All
res) font. Whether or not you remove this font, it will no longer
appear as an option in the Word for Windows Format Character or Import
Symbol dialog box. Instead, the new MS LineDraw (TrueType) font will
appear in both dialog boxes. For more information on removing the MS
LineDraw (All res) font, see the section "Removing a Font" in Chapter
5 of the "Microsoft Windows User's Guide" for version 3.1.

TROUBLESHOOTING
===============

This section describes situations you may encounter when importing
line-drawing characters created in other applications into Word for
Windows.

Line-Drawing Characters in Text File
Opened As Text Only Map to Different ANSI Characters
----------------------------------------------------

Line-drawing or other extended ASCII characters map to different ANSI
characters when a text file (originating from the Word for MS-DOS
CAPTURE.COM utility or any other source) is opened as Text Only.

Resolution
----------

You can address this problem by doing one of the following:

 - After you have converted a document, choose Select All from the
   Edit menu and change the font to MS LineDraw (TrueType).

 - If you are using Word version 2.0b or later for Windows, create a
   special-purpose template in which MS LineDraw (TrueType) is the
   default font. Using this option, to open a text file, do the
   following:

   1. From the File menu, choose New, and use the template you just
      created.
   
   2. From the Insert menu, choose File, and then select the text file
      from the list of files.
   
   3. If you are prompted to open the file as Text Only, choose the OK
      button.
   
      Do not choose to open the file as DOS Text. Doing so uses an
      ASCII-to-ANSI mapping process that is less complete than the
      solution provided by the MS LineDraw (TrueType) font.
   
You can automate either of these options by creating a macro. To fully
automate the process, you can assign the macro to the File menu as an
Open Text command.

For more information on changing the default font in either your
global template or a custom template, see "Changing Default
Formatting" in Chapter 6 of the "Microsoft Word for Windows User's
Guide" for version 2.0.

For more information on assigning a macro to a Word menu or the
toolbar, see Chapters 38 and 42 of the user's guide.

Line-Drawing Characters from
CAPTURE.COM Map to Different ANSI Characters
--------------------------------------------

Line-drawing characters captured using the CAPTURE.COM ASCII-text
screen-capture utility and then embedded in Word for MS-DOS documents
map to different ANSI characters when a Word for MS-DOS document is
opened in Word for Windows.

Resolution
----------

Word for Windows cannot automatically detect line-drawing characters
in ASCII CAPTURE.COM screen captures that are embedded in Word for 
MS-DOS documents. To work around this problem, you can create a font-
mapping file that maps the Courier font (used to represent line-
drawing characters in Word for MS-DOS) to the MS LineDraw (TrueType)
font in Word for Windows.

To create the font-mapping file:

1. Open a new file in a text editor, such as Windows Notepad, and type
   the following:

      1;MS LineDraw
      5;MS LineDraw

    NOTE: If you already have a font-mapping file, you can add these
    two lines to it.

2. Save this file as PCW_RTF.DAT in your Word for Windows directory.

For more information on creating a custom font-mapping file for
documents created in Word for MS-DOS, see the sample mapping file
PCW_RTF.TXT in your Word for Windows directory.

Line-Drawing Characters in WordPerfect Documents Misalign Horizontally
----------------------------------------------------------------------

Line-drawing characters in WordPerfect documents (either inside or
outside user or text boxes) misalign horizontally when a WordPerfect
document is opened in Word for Windows.

Resolution
----------

Word for Windows does detect and correctly map line-drawing characters
originally entered either by the CTRL+F3 WordPerfect line-drawing
command or by the CTRL+2 WordPerfect Compose command to their MS
LineDraw (TrueType) font equivalents in Word. However, you may see
some horizontal misalignment in your document on screen or when it is
printed.

To ensure that no horizontal misalignment of vertical line-drawing
characters appears either on screen or when printing a converted
WordPerfect document, you can create a font-mapping file that maps all
variations of the Courier font in WordPerfect to the Courier New
TrueType font in Word.

To create the font-mapping file:

1. Open a new file in a text editor, such as Windows Notepad, and type
   the following:
      
      Courier;Courier New

    NOTE: If you already have a font-mapping file, you can add this
    line to it.

2. Save this file as WP5_RTF.DAT in your Word for Windows directory.

For more information about creating a custom font-mapping file for
documents created in WordPerfect, see the sample mapping file
WP5_RTF.TXT in your Word for Windows directory.

Line-Drawing Characters in RFT-DCA Documents Misalign Horizontally
------------------------------------------------------------------

Line-drawing characters in DisplayWrite(R)/RFT-DCA (or other Extended
Binary Coded Decimal Interchange Code [EBCDIC]-based) documents,
created either manually or by the DisplayWrite Cursor Draw command,
misalign horizontally when the document is opened in Word for Windows.

Resolution
----------

Word for Windows does detect and correctly map line-drawing characters
originally entered in DisplayWrite to their MS LineDraw (TrueType)
font equivalents in Word. However, you may see some horizontal
misalignment in your document on screen or when it is printed.

To ensure that no horizontal misalignment of vertical line-drawing
characters appears either on screen or when printing a converted RFT-
DCA document, you can create a font-mapping file that maps the
DisplayWrite/RFT-DCA Courier font to the Courier New TrueType font in
Word for Windows.

To create the font-mapping file:

1. Open a new file in a text editor, such as Windows Notepad, and type
   the following:

      26;Courier New,,24

    NOTE: If you already have a font-mapping file, you can add this
    line to it.

2. Save this file as DCA_RTF.DAT in your Word for Windows directory.

For more information about creating a custom font-mapping file for
documents created in DisplayWrite, see the sample mapping file
DCA_RTF.TXT in your Word for Windows directory.

OEM Text from Clipboard Appears Incorrectly
-------------------------------------------

ASCII (OEM) text pasted from the Windows Clipboard and then converted
to the MS LineDraw (TrueType) font does not regain the appearance of
extended ASCII characters.

Resolution
----------

Currently, Word for Windows does not support pasting ASCII text
(called "OEM Text" on the Display menu) from the Windows Clipboard.
Instead of pasting the text from the Clipboard, export the text to an
ASCII text file and then open the file as Text Only in Word, using the
steps described in the first troubleshooting scenario.

Vertical Lines of Line-Drawing Region Contain Gaps
--------------------------------------------------

Slight gaps appear in the vertical lines of a line-drawing region in
Word for Windows.

Resolution
----------

1. Highlight the line-drawing region in Word.

2. From the Format menu, choose Paragraph.

3. If the font size for the line-drawing region is 10 point, change
   the line spacing from Auto to Exactly .7 li. If the font size for
   the line-drawing region is 12 point, change the line spacing from
   Auto to Exactly .9 li. (For other font sizes, you may need to
   experiment to obtain the desired result.)

Line-Drawing Characters Display Incorrectly in Print Preview
------------------------------------------------------------

MS LineDraw (TrueType) line-drawing characters do not display as
expected in Word for Windows print preview.

Resolution
----------

MS LineDraw (TrueType) line-drawing characters are not currently
supported in print preview. What you see instead are the ANSI
characters with their equivalent numeric values. This only affects
print preview, not your printed output.

Bold Text in Line-Drawing Region
Appears Normal; Vertical Characters Shift Right
-----------------------------------------------

Bold text appears normal inside a line-drawing region, and vertical
line-drawing characters shift to the right.

Resolution
----------

The MS LineDraw (TrueType) font does not currently support bold text
within a line-drawing region. If you use one of the font-mapping files
as described previously, this problem does not occur. This problem
occurs only if you open a file as Text Only and later apply bold
formatting. To restore the horizontal alignment of the line-drawing
characters in this situation, either remove the bold formatting or do
the following:

1. Select the bold text in the line-drawing region.

2. From the Format menu, choose Character, and select Courier New from
   the Font box.

3. Choose the OK button.


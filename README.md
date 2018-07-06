# PdfScribe v1.0.5

PdfScribe is a PDF virtual printer. Check the [releases](https://github.com/matthewgregg/PdfScribe/releases) page for this project to download a prebuilt MSI package.

## System Requirements

* 64-bit Windows Vista or later
* .NET Framework 4.0 or later

## Building from source

Visual Studio 2015, Wix 3.11, and Votive 2015 are required to build PdfScribe.

PdfScribe links to, and distributes the following third party components:

* Microsoft Postscript Printer Driver (V3)
* Ghostscript (64-bit)
* Redmon 1.9 (64-bit)

## License

Redmon is distributed under the GPL v3. Ghostscript is AGPL (more restrictive than GPLv3), so PdfScribe is bound by that license.



## Configuration
 
In the application config file (PdfScribe.exe.config), there are two settings in the "applicationSettings" element:

* ****AskUserForOutputFilename**** - set value to *true* if you want PdfScribe to ask the user where to save the PDF.
* ****OutputFile**** - if there is a constant filename you want the PDF to be saved to, set its value here. Environment variables can be used. PdfScribe will overwrite each time. This setting is ignored if  **AskUserForOutputFilename** is set to *true*. 
* ****RunFileDisabled**** - set value to *false* if you want PdfScribe to run a batch file (or any command)
* ****RunFile**** - specify batch file to run. This setting is ignored if **RunFileDisabled** is set to *true*.


## To do

* Add more page sizes (currently only US Letter is supported)
* Allow auto-generated filenames with sequence numbers if the user doesn't want to overwrite (ex: OUTPUT-001.PDF, OUTPUT-002.PDF, etc)
* Allow file appending if **OutputFile** setting is used.
* GUI for configuration
* Watermarking output

 



# LabVIEW_LJM
This is the public repository for LabVIEW code to use the LabJack LJM library.

LabVIEW_LJM - LabVIEW drivers/examples for LJM
support@labjack.com

March 16, 2021

Compatible with LabVIEW 7.1 or higher.  Requires the
LabJack UD driver.

Note that National Instruments provides a driver called NI-DAQ
for their hardware.  We have to provide our own library, called
LJM, for our hardware.  LabVIEW can talk to either driver/library,
but realize that some NI tools like Measurement & Automation
Explorer and DAQ Assistant are part of NI-DAQ and thus do
not apply to LabJacks.

These VIs use the LJM library for Windows.  Before using
the VIs, you should look at the LJM User's Guide and the
datasheet for your LJM compatible device.

LabVIEW is a programming language like C++, not a tool like
Excel.  At its core, LabVIEW is just a graphical representation of
C or similar, so any text based examples you see in our documentation
will usually map easily to LabVIEW.

The downloadable zip file "LabVIEW_LJM.zip" extracts to a single
folder called "LabVIEW_LJM" which contains this readme file and a
few subfolders.  The folder can be stored anywhere, but if you want
icons to show up on the LabVIEW function palette (after restarting
LabVIEW), place this folder under:

...\national instruments\labview #\vi.lib\addons\

If the function palette icons are not required, put the LabVIEW_LJM
folder wherever you want.  We have found that most people, including
us, just do this.  Instead of using palette icons to select LJM VIs,
most people just:

   1)  copy and paste from examples,

... and

   2) use the "Select a VI..." balloon from the function palette.

We recommend not having more than one copy of the VIs,and not changing
these VIs.  Make a copy in a different folder if, for instance, you
wish to modify one of the example VIs.  If you download new VIs
from labjack.com, delete and replace the entire LabVIEW_LJM folder.

6000 is added to the LabJack errorcodes to shift them into the LabVIEW
user range of 5000-9999.

The \Functions\ folder contains simple VIs that do little
more than call functions from LJM.  Most of these need a valid Handle
input so are usually not used standalone.

The \LVUtilities\ folder contains VIs that encapsulate some useful
functions.  You find these used in other VIs from the \Functions\ and
\Examples\ folders to handle things unique to LabVIEW.

The \Examples\ folder has various examples.  Generally these can
be run stand-alone.  Generally examples cannot be dropped into your
program as a sub-VI.  Rather, they demonstrate how to incorporate
the LJM sub-VIs in your VI, or serve as a starting point for your
own VI.

The \LJLogM\ and \LJStreamM\ folders contain the source code for
those sample programs.  The executable versions (.exe) are part
of the main LabJack software installer for Windows.

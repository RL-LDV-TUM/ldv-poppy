# Print

## 3D Models

The *.STL* files for all parts are contained in the [stl](/3D/stl) folder, respectively the *.SDLPRT* (Solidworks Source Files) are in the [solidworks](3D/solidworks) folder.
As noted in the [Parts Table](3D/partsTable.md) not all parts are needed to print the LDV-Poppy.
Furthermore there are redesigned versions of some parts, which are more durable or more comfortable to assemble. 
The newest version is documented in the [Parts Table](3D/partsTable.md)

## Software
The Software which is used to bring the 3D files to the printer is Repetier Host.
Before the first use of Repetier Host with a new printer make sure that the programm has the right printer settings.

### Object Placement
You can easily drag a *.STL* or *.OBJ* file into the main windown of Repertier Host to add this object to the print job.
In order to find the right orientation to print the object refer to [Print Orientation](3D/defects.md#print-orientation) on the defects site.

### Slicer
The best tuned slicer for this project was curaengine. Make sure that curaengine is selected before changing any other thing in the slicer configuration.
All slicer configuration files can be found in the [PrinterSettings](3D/PrinterSettings) folder.
Use *cura_poppy_300* as Print Configuration. If you use ABS as filament select *ABS_poppy1* as Filament Setting for Extruder 1.
Choose the *PLA_poppy1* in the case you use PLA material.
Detailed settings for each object can be found in the [Parts Table](3D/partsTable.md)

## Printer Settings
Settings for using Repetier Host with the RF1000

Connections Tab:

![Connections](images/printerSettings/Printer_Settings_Connections.png)

Extruder Tab:

![Extruder](images/printerSettings/Printer_Settings_Extruder.png)

Printer Tab:

![Printer](images/printerSettings/Printer_Settings_Printer.png)

PrinterShape Tab:

![PrinterShape](images/printerSettings/Printer_Settings_PrinterShape.png)





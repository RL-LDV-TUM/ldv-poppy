# LDV Poppy

The LDV Poppy is a customized version of the [Poppy Humanoid](https://www.poppy-project.org/en/robots/poppy-humanoid) by poppy-project.
The original Github repository containing the Solidworks 3D files and Software can be found [here](https://github.com/poppy-project/poppy-humanoid).
There is also a Onshape project where all Solidworks files are imported: [Poppy humanoid v1.0.1](https://cad.onshape.com/documents/77a0f84dc57f40418500cc3e/w/5e73b9c6a1ca45368c6251fc/e/ed6b82f994b249e388f92c2e).
This Onshape project can be cloned and edited. However it is sometimes easier to import only single Solidworks files from this repository to onshape.

## 3D Models

The Onshape project for the [LDV Poppy can be found here.](https://cad.onshape.com/documents/56d596aee4b004367d90f087/w/5446e589942f217504b25eb7/e/aac52fdb51e2f46d7fa4375f).
This project contains a full clone of the original Onshape project and the optimized files. Optimizations were nescessary to improve the 3D print outcome
on the Renforce RF1000 3D-Printer available at the LDV.
Currently there are still parts which need a redesign or can only be printed in a certain orientation: [Errors and Defects](3D/defects.md)

Instructions for printing can be found [here](3D/print.md).
Solidworks source files for editing: [solidworks](3D/solidworks)
STL files for printing: [stl](3D/stl)

## Programming

Poppy provides his own websever: [poppy.clients.ldv.ei.tum.de](http://poppy.clients.ldv.ei.tum.de)

Several *jupyter* notebooks are provided to controll the robot using the *odroid* mini PC.

Connecting poppy to the network: [Network](Software/network.md)

Getting started with poppy: [Working with poppy](Software/gettingStarted.md)


# tinyFrame
<div align="center">

![logo](repodata/logo.png)

tinyFrame is a modular tooling framing system focused on ease of manufacture, reusability and accuracy.
</div>

# Modular, Customizable and Open Source Tooling
## Cost effective
At $1/foot, this system is more afforadble than PVC tubing.
## Accurate
Modern 3D printers such as the Bambu P1P can hit roughly 250 micron of profile and positional tolerance.
## Customizable
CAD is provided and users can model and customize their designs before manufacture.
## Open Source
Free to use. Improves over time with contribution.

# Example
Frame members (T230-X-X) are joined together by connectors (CX-X-X) and adapters (M1-X-X). Below is 1 x 1 x 1 frame.

![1](repodata/SS1.png)

This example frame is stored in the assemblies folder. Use ![Ondsel](www.ondsel.com) (a free CAD software) to open it.

Slice and print individual parts in the right quantities to make the frame on a 3D printer.

![sample frame](repodata/SS2.png)

Break apart and use these parts to create the frame you designed. Save your parts for later - they're interchangeable and can be easily reused. In the below example, roughly 22 feet was printed in a single Bambu P1P print bed with one 1 kg spool of filament.

![printed parts](repodata/SS3.png)

# Getting Started
TBD.
# Use
TBD.

# FAQs
## Why isn't tinyFrame ratable for structural use?
### FDM 3D printed parts are anisotropic which makes them difficult to analyze. Additionally, they are not controllable for key mechanical properties because the process is heavily dependent on several factors (humidty, slicing configuration, temperatures, etc.)

## Why Ondsel and not FreeCAD?
### FreeCAD does not natively support assemblies yet, but does support Workbenches that do. Ondsel, an interoperable FreeCAD derivative which is actively supported, supports and is building on assembly support. With that said - Ondsel is backwards compatible at the part level. Contributions or changes can be made using FreeCAD or Ondsel, and users looking to build or contribute to assemblies can use Ondsel.

## I've built a frame and it feels sloppy - why?
### Adapters purposely gap joined parts to account for assembly misalignment and profile tolerance at the part level. These gaps are to allow accuracy defining parts in the future without overconstraining the system.

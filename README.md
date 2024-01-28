# tinyFrame

<div align="center">

![logo](/repoData/logo.png)

tinyFrame is a 3D printed modular tooling framing system focused on ease of manufacture, reusability and accuracy
</div>

# Modular, Customizable and Open Source Tooling
## Cost effective
At $1/foot, this system is 1/2 the cost of PVC tubing and:
- 1/8 the cost of 80/20 compatible T-Slot framing
- and still cheaper than wood while maintaing reusability 
## Accurate
Modern 3D printers such as the Bambu P1P can hit roughly 250 micron of profile and positional tolerance. This is looser in practice due to warping of prints, but can be tuned. 
## Customizable
CAD is provided and users can model and customize their designs before manufacture.
## Open Source
Free to use. Improves over time with contribution.

# Example
Frame members (T230-X-X) are joined together by connectors (CX-X-X) and adapters (M1-X-X). Below is 2 x 1 x 1 frame used for storage. The storage containers are also made available.
| CAD | Reality |
:------------------------------: | :---------------------------|
| ![4](/repoData/SS4.png) | ![1](/repoData/SS1.png) |


Slice and print individual parts in the right quantities to make the frame on a 3D printer.

![sample frame](/repoData/SS2.png)

Break apart and use these parts to create the frame you designed. Save your parts for later - they're interchangeable and can be easily reused. In the below example, roughly 22 feet was printed in a single Bambu P1P print bed with one 1 kg spool of filament.

![printed parts](/repoData/SS3.png)

# Getting Started
Download the repository and use your CAD platform of choice to import the STP files for use.
Contributions must be made using FreeCAD or Ondsel.
More information TBD.

# Use
All prints designed for Polymaker PLA on a Bambu P1P 3D printer.
More information TBD.

# FAQs
## Why isn't tinyFrame ratable for structural use?
FDM 3D printed parts are anisotropic which makes them difficult to analyze. Additionally, they are not controllable for key mechanical properties because the process is heavily dependent on several factors (humidty, slicing configuration, temperatures, etc.)

## Why Ondsel and not FreeCAD?
FreeCAD does not natively support assemblies yet, but does support Workbenches that do. Ondsel, an interoperable FreeCAD derivative which is actively supported, supports and is building on assembly support. With that said - Ondsel is backwards compatible at the part level. Contributions or changes can be made using FreeCAD or Ondsel, and users looking to build or contribute to assemblies can use Ondsel.

## I've built a frame and it feels sloppy - why?
Adapters purposely gap joined parts to account for assembly misalignment and profile tolerance at the part level. These gaps are to allow accuracy defining parts in the future without overconstraining the system.

# TODO
- Finish 'Getting Started'
- Finish 'Use'
- Break MX into assembly
- Create assembly drawings 
- Fix current platform design (see unreleased directory)
- Calculations on T230
	- Need to find worst case combined loading
	- Optimize wall thickness so that maximum bending stress at tube wall equals maximum shear stress at thread / .62
- System anisotropic: develop failure theory that approximates to a worst case allowable yield stress
	- Need to test at:
		- Different humidites
		- Water content of PLA
		- Different loadings
		- Shear
		- Tensile
- sContainer1 walls too thin. Need to find better thickness
	- Need to add draft angle to walls to make container stackable
- sContainer2 walls too thin. Same need as above
	- Draft angle requires testing to see if stacking working as designed
- Part Naming schema needs to be explained
- Need to redefine mate-points on assemblies and verify
- Develop documentation at tinyframe.dev

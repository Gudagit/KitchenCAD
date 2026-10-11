# KitchenCAD

A Windows desktop application for designing kitchens: from room dimensions to part lists, shop drawings and CNC programs. Written in C# (WinForms) with no third-party libraries, about 15,000 lines of code.

This repository is a portfolio showcase. **The source code is private; a demo build and a code walkthrough are available on request** (see below).

## The problem it solves
Building a kitchen means re-typing the same dimensions into several tools (drawings, cut lists, drilling programs, labels), and every copy is a chance for a mistake. KitchenCAD keeps a single parametric model: enter a dimension once, and all parts, hardware holes, drawings and machine programs are recalculated from it.

## Features
- Layout by wall (L-shaped and U-shaped kitchens) with doors and windows, plus warnings for overlaps and clearance problems
- Base, wall and tall cabinets and drawer units; carcass, fronts, hardware and joinery are generated from parameters
- Free interior division, half-joint grids, wine shelf, blind corner, rounded and chamfered ends
- 3D view, exploded assembly view, and a photorealistic renderer (custom path tracer)
- Cut lists, nesting, part labels, and dimensioned shop drawings
- Export to PDF, DXF (R12 and R2000) and CNC programs

## Screenshots
The user interface is in Serbian.

![3D view of a kitchen](screenshots/01-3d-kuhinja.png)
![Wall elevations with room warnings](screenshots/02-izgled-zidova.png)
![Dimensioned shop drawing](screenshots/03-shop-crtez.png)
![Exploded assembly view](screenshots/04-eksplodirani-prikaz.png)
![Wood textures in 3D](screenshots/05-teksture.png)
![Part drawing with CNC operations](screenshots/06-crtez-dela-cnc.png)

## Technology
C#, .NET Framework 4, WinForms, GDI+. A custom path tracer with a BVH acceleration structure, a nesting algorithm, DXF and PDF export, and template-based CNC program generation.

## How it was built
I developed this program in collaboration with an AI assistant (Claude Code). I defined what the program does, the cabinet-making rules and dimensions, and tested and reviewed every result; the assistant wrote the code from my requirements.

## Demo and source code on request
To try the program or review the code, contact me at **gudagluposti@gmail.com**. I send the demo as a ZIP file and grant read-only access to the private repository.

## Notes
- The CNC output has not been verified on a physical machine.
- Manufacturer names (Blum, Zebra, AutoCAD and others) are mentioned only to describe compatibility; this project is not affiliated with them.

## License
All rights reserved. Text and images are published for portfolio viewing only; the software and its source code may not be copied, modified or used without permission. See [LICENSE](LICENSE).

Author: Ivana

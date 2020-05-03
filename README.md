# Metal Bar Normal Modes

ElmerFEM model for the search of normal modes of a metal bar.

Part of the [accompanying repositories](https://github.com/Computational-Acoustics) of the [Modelling Acoustics with Open Source Software](https://crocoduckoducks.github.io/modelling-acoustics-with-open-source-software/) tutorials series.

## Covering Episodes

* [Elastic Modes of a Metal Bar](https://crocoduckoducks.github.io/science/physics/opensource/2019/06/09/elastic-modes-of-a-metal-bar.html).
* [Refining the Metal Bar Model](https://crocoduckoducks.github.io/science/physics/opensource/2020/02/15/refining-the-metal-bar-model.html).

## Software Overview

The table below reports the software used for this project.

| Software                                           | Usage                |
|----------------------------------------------------|----------------------|
| [FreeCAD](https://www.freecadweb.org/)             | 3D Modeller          |
| [Salome Platform](https://www.salome-platform.org) | Pre-processing       |
| [ElmreFEM](http://www.elmerfem.org)                | Multiphysical solver |
| [ParaView](https://www.paraview.org/)              | Post-processing      |

## Repo Structure

* `elmerfem` contains the ElmreFEM project.
* `geometry.FCStd` is the FreeCAD geometry model. This file can be used to export geometric entities to _BREP_ files to pre-process with Salome. _BREP_ files are excluded from the repo as they are redundant.
* `meshing.hdf` is the Salome study of the geometry. It contains the geometry pre-processing and meshing. The mesh is exported into `elmerfem` as `elmerfem/Mesh_1.unv`.

The repo contains only the _source_ of the simulation. To obtain results, the study must be solved.


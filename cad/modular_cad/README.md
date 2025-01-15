This folder contains a parametric version of the model. The Computer Assisted Design (CAD) file was made with **FreeCAD v1.0.0** (v1.0.0 or above is required if you want to open it, since the model uses the new Assembly workbench and other new features available since v1).

# Features

Here is a list of the most important features of the model:

**Regarding the box:**
- Double walls: we initially added 2 walls to the model so that we could use colored transparent sheets to act as optical filters and filter the light.
- Adjustable latches: these latches allow the lid to be tightly attached to the box.

**Regarding the strips:**
- Strip attachment: the strips are attached to the box with molted nylon screws for easy use. To avoid having to drill the box bottom, a piece called "strip attachment" is glued to the bottom part of the box, with threaded holes to screw the strips.
- 2 parts strips: the strips are composed of two parts, including a lid. The strips are 3D printed, while the lids are laser cut in acrylic sheets.

![techdraws](../img/png/techdraws.svg)

# Parametric model

This parametric model helps making specific boxes and strips.

## Visible parameters

Most important parameters were kept visible in the Model tree > VarSet > Data.
These are the available parameters:

| Variable name | Description |
| --- | --- |
| box_height | This is useful if you want better access to the strips placed inside the box. |
| filter_slot | Slot to place the filter. |
| pmma_thickness | Defines the thickness of the acrylic sheets. |
| hole_rad | Radius of the hole in the strip lid, for the particles to access the wells. |
| strip_nb | Number of strips wanted. |
| well_nb | Number of wells wanted. |
| well_rad | Radius of the wells. |

![alt text](../img/png/variables.png)

## Hidden parameters

There are also a lot of hidden parameters that you might be interested to investigate.
Right click on the VarSet Data > tick *Show hidden*.

![alt text](../img/png/hidden_variables.png)

# How to export files

## 2D files (for laser cutting)

There are various ways to export files for laser cutting.

### With native FreeCAD functions

[![3D to 2D export](https://img.youtube.com/vi/lLCqwrhGM3o/0.jpg)](https://www.youtube.com/watch?v=lLCqwrhGM3o)

### With macros or external workbenches

Some macros or external workbenches might also work.
As an example, the Laser Cut Interlocking external workbench (LC interlocking) has an *export* feature used to convert 3D shapes to 2D.

## 3D files (for 3D printing)

- Click on the part you want to export;
- Ctrl + E (Or File > Export);
- Select the STL extension;
- Save.

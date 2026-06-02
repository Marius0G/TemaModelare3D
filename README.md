# Iris Box - Storage Container with Mechanical Iris Lid

## 1\. Project Description

The **Iris Box** is a fully 3D-printable storage container featuring a mechanical iris lid mechanism with **6 blades**. Inspired by the smooth, captivating motion of camera shutters and mechanical iris diaphragms, this project transforms that mechanism into a functional desktop storage box.

The lid opens and closes by rotating a dedicated disc, which drives all six blades simultaneously in a synchronized radial motion — creating a satisfying mechanical aperture that reveals or conceals the contents inside.

### Key Features

* **6-blade mechanical iris lid** — Provides a smooth, visually striking opening/closing action.
* **Bayonet-style twist-lock connectors** — The three main body sections (bottom, middle, top) assemble by sliding together and rotating, similar to a telescope or camera lens mount. No glue or screws required.
* **Fully 3D-printable design** — All components are designed with printability in mind: minimal overhangs, chamfered edges, and appropriate tolerances for moving parts.
* **Clean, organized Fusion 360 project** — Sketches are named, components are structured, and motion links are defined to simulate the iris mechanism.

### Inspiration

This project draws inspiration from two YouTube videos demonstrating mechanical iris mechanisms:

* [Iris Mechanism Build Video 1](https://www.youtube.com/watch?v=l9jnfk2sK0Y)
* [Iris Mechanism Build Video 2](https://www.youtube.com/watch?v=ToWUMI30UFo)

The original designs were re-engineered from the ground up in **Autodesk Fusion 360** to create an original, printable product. Key contributions include:

* Redesigning the housing into a **3-part stackable box** with integrated bayonet connectors.
* Adding a dedicated **rotating disc** to actuate the iris from the outside.
* Sizing and tolerancing all components specifically for **FDM 3D printing** (0.2 mm layer height, PETG).
* Optimizing geometry to minimize support requirements and ensure reliable print-in-place assembly.
* Adding the whole storage/box part in the idea

### How It Works

1. The **6 blades** are arranged in a circular overlapping pattern inside the top housing.
2. Each blade features a **pin** on one end and a **slot** on the other. The pin of each blade rides in a curved guide track, while the slot engages with a drive pin on the rotating disc.
3. When the user rotates the **outer disc**, the drive pins push/pull all six blades simultaneously, causing them to pivot and slide — opening or closing the central aperture.
4. The three body sections (**bottom** → **middle ring** → **top housing**) connect via bayonet-style tabs. You insert one section into the next, then twist clockwise to lock it in place.

\---

## 2\. Project Files

|File|Type|Description|
|-|-|-|
|`Proiect Modelare 3D - Iris Box.f3d`|Fusion 360 Project|Complete CAD project with all components, sketches, joints, and motion studies|
|`CutiePrinciapala\_jos.stl` / `.3mf`|STL / 3MF|Bottom section of the box (main storage compartment)|
|`CutiePrinciapala\_mijloc.stl`|STL|Middle ring section (spacer / extension)|
|`CutiePrincipala\_sus.stl`|STL|Top section housing the iris mechanism|
|`DiscRotire.stl`|STL|Rotating disc that actuates the iris blades|
|`Dinte.stl`|STL|Single iris blade — **print 6 copies**|
|`irisbox\_0.2mm\_PETG\_MK3S\_9h45m.gcode`|G-code|Pre-sliced print file for Original Prusa i3 MK3S (PETG, 0.2 mm layer height)|

\---

## 3\. Video Showcase



\---

## 4\. Components / Parts List

|#|Component|Quantity|Purpose|
|-|-|-|-|
|1|**Bottom Box** (`CutiePrinciapala\_jos`)|1|The main storage compartment. Features female bayonet slots at the top rim for connecting to the middle ring.|
|2|**Middle Ring** (`CutiePrinciapala\_mijloc`)|1|An optional spacer/extension ring. Has male bayonet tabs on the bottom and female slots on top. Can be omitted for a shorter box.|
|3|**Top Housing** (`CutiePrincipala\_sus`)|1|Houses the entire iris mechanism. Contains the curved guide tracks for the blade pins and the inner ledge where the rotating disc sits. Features male bayonet tabs on the bottom.|
|4|**Rotating Disc** (`DiscRotire`)|1|The user-facing actuator ring. Sits inside the top housing and features 6 drive pins on its underside that engage with the blade slots. Knurled/textured outer edge for grip.|
|5|**Iris Blade** (`Dinte`)|**6**|The individual blades that form the iris aperture. Each blade has a pivot pin (rides in guide track) and a slot (engages with disc drive pin). The blades overlap in a circular pattern to form a hexagonal aperture.|

### Assembly Overview

1. **Print all parts.** Ensure 6 copies of `Dinte.stl` are printed.
2. Insert the **rotating disc** into the **top housing** (disc sits on the inner ledge, drive pins facing down).
3. Place all **6 blades** onto the drive pins (slot over pin) and seat the pivot pins into the curved guide tracks. The blades should overlap in a clockwise/counterclockwise pattern.
4. Connect the **middle ring** to the **top housing** using the bayonet tabs — align, insert, and twist to lock.
5. Connect the **bottom box** to the **middle ring** using the same bayonet action.
6. Rotate the outer disc to open and close the iris!

\---

## 5\. Print Settings

|Parameter|Value|
|-|-|
|**Material**|PETG|
|**Layer Height**|0.2 mm|
|**Printer**|Original Prusa i3 MK3S|
|**Nozzle Temperature**|240 °C (typical for PETG)|
|**Bed Temperature**|85 °C|
|**Estimated Total Print Time**|\~9h 45min|
|**Supports**|Not required (design optimized for support-free printing)|
|**Infill**|15-20% gyroid or grid|

### Print Orientation Recommendations

* **Bottom Box**: Print upright (open side up) — no supports needed.
* **Middle Ring**: Print flat on its rim — no supports needed.
* **Top Housing**: Print upside-down (iris cavity facing up) for best guide track surface quality.
* **Rotating Disc**: Print flat with drive pins facing up.
* **Blades**: Print flat on the largest face. A brim may help with bed adhesion due to the small footprint.

\---

## 6\. Resources Used

### Inspiration \& Reference

* [Iris Mechanism Video 1](https://www.youtube.com/watch?v=l9jnfk2sK0Y) — Mechanical iris design principles
* [Iris Mechanism Video 2](https://www.youtube.com/watch?v=ToWUMI30UFo) — Iris box concept and assembly

### Software

* **Autodesk Fusion 360** — 3D CAD modeling, motion studies, and STL export
* **PrusaSlicer** — G-code generation for the Prusa MK3S

### Hardware

* Original Prusa i3 MK3S (FDM 3D printer)
* PETG filament

\---

## 7\. Design Considerations

### Printability

* All edges are chamfered or filleted to improve print quality and reduce stress concentrations.
* Moving parts (blades, disc) include **0.3–0.4 mm clearance** to account for FDM tolerances and ensure smooth movement without post-processing.
* The bayonet connectors include a slight interference fit that loosens after the first assembly/disassembly cycle — typical for 3D-printed snap fits.
* No component requires support material when printed in the recommended orientation.

### Motion Study

The Fusion 360 project includes a **motion link** between the rotating disc and all 6 blades, allowing you to animate the iris opening and closing by dragging the disc rotation joint.

\---

## 


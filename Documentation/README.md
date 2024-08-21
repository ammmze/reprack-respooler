# Documentation

## Bill of Materials / BOM

### Printed parts

| Name | Quantity | Notes |
| --- | --- | --- |
| Spool holder frame | 1 | Use the "Main parts" > "Frame.3mf" from [here](https://www.printables.com/model/292276-auto-rewind-spool-holder-for-reprack/files). You can omit the one cross member piece that has a long slot for the filament. The re-spooler has an replacement for that. |
| Rear roller | 1 | Use  the "Main parts" > "Cylinder Shell.3mf" from [here](https://www.printables.com/model/292276-auto-rewind-spool-holder-for-reprack/files). You only need 1 of these for this application, NOT 2. And you do NOT need the coils either. |
| [Drive wheel - for 608 bearing](./STL/Drive%20wheel%20-%20for%20608%20bearing.stl) | 1 | |
| [Drive wheel bearing adapter](./STL/Drive%20wheel%20bearing%20adapter.stl) | 1 | |
| [Drum](./STL/Drum%20x2.stl) | 2 | |
| [Frame front cross member left](./STL/Frame%20front%20cross%20member%20left.stl) | 1 | |
| [Frame front cross member right](./STL/Frame%20front%20cross%20member%20right.stl) | 1 | |
| [Frame](./STL/Frame.stl) | 1 | |
| [Inner Shoulder](./STL/Inner%20Shoulder%20x2.stl) | 2 | |
| [R4 bearing idler adapter](./STL/R4%20bearing%20idler%20adapter.stl) | 1 | Only needed if using an R4 bearing for the idle bearing instead of a 625 bearing. May want to enable "detect thin walls", which seemed to have the slicer do it in a single wall rather than like 1.5 walls. |
| [Re-spooler sled](./STL/Re-spooler%20sled.stl) | 1 | |
| [Roller Grip](./STL/Roller%20Grip.stl) | 1 | |
| [Sleeve TPU](./STL/Sleeve%20TPU%20x2.stl) | 2 | |
| [Tension Arm Left](./STL/Tension%20Arm%20Left.stl) | 1 | |
| [Tension Arm Right](./STL/Tension%20Arm%20Right.stl) | 1 | |
| [Tension nut](./STL/Tension%20nut.stl) | 1 | |

### Hardware

| Name | Quantity | Notes |
| --- | --- | --- |
| 608 Bearings | 5 | 2 used in each shaft and one in the drive wheel. May be a bit excessive, but it's a common and cheap bearing. |
| 625 or R4 bearing | 1 | Be sure to print R4 adapter if using R4 bearing. No extra adapter needed for 625, it fits directly in the tension arm. |
| #211 O-rings | 2 | 13/16" ID, 1 1/16" OD |
| M3 heat insert | 5 | Voron standard 5mm OD, 4mm L |
| Spring from BMG extruder kit | 1 | 6mm OD, 1mm wire, 15mm free length |
| M3 nut | 8 | Main spool holder frame |
| M3 x 6mm Socket head cap screw | 1 | Fastens re-spooler to sled |
| M3 x 8mm Socket head cap screw | 8 | Main spool holder frame |
| M3 x 12mm Socket head cap screw | 2 | Fastens tension arm halves |
| M3 x 25mm Socket head cap screw | 1 | Pivot for tension arm |
| M3 x 30mm Socket head cap screw | 1 | Tension screw |
| One-way bearing | 1 | 8mm bore, 12mm Length, 14mm Diameter, Octagon shape |
| 8mm x 80mm metal rod | 1 | Main shaft for respooler |

> [!NOTE]
> The above BOM includes the hardware needed for the spool holder frame from the original project.

## Assembly

### Spool holder frame

First assemble the spool holder frame and rear cylinder (minus the spring coil) using the instructions provided [here](https://www.printables.com/model/292276-auto-rewind-spool-holder-for-reprack). It's easy...just insert some M3 nuts and M3 x 8mm screws, toss in a couple 608 bearings and screw the cap on the cylinder. And omit the upper-front piece, the re-spooler has a replacement cross member.

### Re-spooler

1. Insert heat set inserts ([1 in tension nut, 2 in tension arm, and 1 in side of frame](./heat%20set%20inserts.jpg), [1 in bottom of frame](./heat%20set%20inserts%202.jpg))
2. Assemble ECAS04 Collets, remove the rubber seal (it won't be used). I find it easiest to install the latch (typically blue in most ECAS) by placing the body in the tension arm, then close up the tension arm and use it as a tool to grip the ECAS body and press the latch in. Then take it out and do the other one. See [this](./tension%20arm%20as%20ecas%20tool.jpg) photo.
3. Assemble the drive wheel (see [image](./drive%20wheel%20assembly.jpg)). Insert 608 bearing into drive wheel, then insert drive wheel adapter to the center of the 608 bearing. Note this adapter is slotted. This allows the drive wheel to slide back and forth as part of the tensioning mechanism.
4. Add idle bearing, drive wheel, and ECAS collets to the tension arm. The idle bearing can use either a 625 bearing directly, or an R4 bearing with the small adapter ring. Finish up the tension arm by putting the 2 halves together and fasten with 2 12mm screws. See [image](./tension%20arm%20assembly.jpg)
5. Insert the tension nut into the slot in the re-spooler frame, followed by the spring. It is recommened the heat insert is toward the back of the respooler, so the tension screw is pulling it through the tension nut, not out of it. See [image](./tension%20nut%20and%20spring.jpg).
6. Insert one way bearing into the "Roller Grip" and slide it onto the 8mm shaft. Then figure out which way it spins freely and which way it locks. When looking at the left side of the respooler, you want it to lock when spinning clockwise and it should spin freely when going counter clockwise.
7. Insert 1 608 bearing into the respooler frame, followed by the shaft with the one way bearing, and finally the last 608 bearing.
8. Assemble the roller drums. These are slightly tapered in an attempt to help keep the spool from wandering (though it didn't really help). Slide the TPU sleeve onto the roller drum then screw on the inner shoulder. Finally slide them onto either end of the shaft. Make sure they aren't pinching the frame or friction will be too much.
9. Place the tension arm into place and put 25mm screw through the pivot hole.
10. Install tension screw just above the pivot, back through the spring and into the tension nut. Optionally you can toss an M3 washer on this tension spring for better distribution of load.
11. Slide the sled into the spool holder frame and attach the cross member pieces using 8mm screws. See [image](./sled%20and%20cross%20member%20pieces.jpg).
12. Slide the respooler in from the front and insert 6mm srew in the bottom to lock it into place. See [image](./final%20lock%20screw.jpg)

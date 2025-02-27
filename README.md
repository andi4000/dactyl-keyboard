# Andi4000 6x7 Dactyl-ManuForm Fork

![Dactyl Manuform 6x7 ISO-DE](resources/dactyl-manuform-6x7-10.jpg)

Pictured is the finished build with (close to) ISO-DE Layout, with DSA Profile
Keycaps from YMDK, and some blank 1U keycaps.

[Click here](#firmware) for the QMK Firmware for this layout.

![Dactyl Manuform 6x7 ISO-DE](resources/dactyl-manuform-6x7-12.jpg)

## TODO
- reduce heat insert diameter

## Differences
- 6x7 Layout. Coming from TKL ISO Layout, I am too lazy to use layers and learn
  a new layout. I also need dedicated F-Keys.
- No Wire Post
- Mount for [Delock Cable USB 2.0 Micro-B Female Panel-Mount](https://www.delock.com/produkt/85245/merkmale.html)
- Flipped RJ9 mount, so that the cable clip will end up on the upper side
- New Promicro Mount

See [right.stl](things/right.stl) for preview.

## FDM 3D-Print Setup
- I use Ultimaker Cura (v5.1.1) as slicer, with following settings
    - 0.2mm layer height
    - (**Important**) Support Structure: Tree --> extremely easier to remove
      compared to normal
    - 10% Infill
    - 10mm Brim
- Printer: stock Sovol SV02 with heated bed, Esun PLA with 205°C nozzle temp 
  and 60°C bed temp.
- PVA glue (UHU Stic) applied to the bed, especially on the brim and sidewalls
  area because they tend to warp, which is a common (big) print issue.
- How to know where the brim and side wall will go? Start print and stop when
  the outer brim is printed. That would be the boundaries. I applied generous
  amount of PVA glue there.
- Once the print reaches ca. Z=10mm, if warping is not present, print is more
  likely to be succeeded, w.r.t. warping.
- Be careful on removing support structure around the Promicro mount. Make sure
  you know how it should look like without the support. See `right.stl`.


## Assembly
For 6x7 you need following items:
- 86 Cherry-MX (or compatible) Switches
- 82 1U Keycaps. I use DSA profile keycaps. Cherry profile are reported to also
  work.
- 4 1U or 1.25U Keycaps for the upper thumb
- M3 Heat Inserts, at least 10 pcs.
- M3x5 countersink screws, at least 10 pcs.

Wired and (almost fully) assembled left side:
![wired left side](resources/dactyl-manuform-6x7-07.jpg)

What really helped during the assembly was to have and use following:
- [Amoeba single-switch PCB](https://deskthority.net/viewtopic.php?t=11420) from
  a local vendor. I bought 100 pcs. with some spares just in case I messed up.
- A good soldering iron. I used [Ersa C25 25W](https://www.ersa-shop.com/ersa-l%C3%B6tkolben-multitip-230v-p-2787.html).
  I went through two cheap soldering irons, both end up with broken tip and
  subpar results. Also a metal solder tip cleaner.
- Single-core jumper wires. I used wires with 0.2 sq. mm cross section. It's
  stiff compared to wires with multi-core, which make the PCBs to stay in place
  before soldering.
- Multimeter to do continuity check. Cheap one will do.

Additionally I also use XH-Type connector at the ProMicro as idiot-proofing.

## Build Photos
<details>
<summary>Finished 24h-long print.</summary>
"Tree" support structure really makes removing supports easier.

![fresh out of the oven](resources/dactyl-manuform-6x7-02.jpg)
</details>

<details>
<summary>Sanded, primered, painted, clear coat.</summary>

![sanded and painted](resources/dactyl-manuform-6x7-01.jpg)
</details>

<details>
<summary>Continuity check after soldering diodes.</summary>
Easier if you do this in batch of e.g. 10 PCBs

![continuity check](resources/dactyl-manuform-6x7-03.jpg)
</details>

<details>
<summary>Wiring harness with Amoeba PCB for the left side.</summary>
With XH-Connectors for the rows and columns

![wiring left with XH connector](resources/dactyl-manuform-6x7-04.jpg)

![wiring left](resources/dactyl-manuform-6x7-08.jpg)
</details>

<details>
<summary>Mounted wiring harness for the left side.</summary>
Soldering the top left (the deepest point) was really difficult.
I found it to be easier to first remove the switch, put PCB on position,
then carefully insert the switch back.

![wiring mounted](resources/dactyl-manuform-6x7-05.jpg)
</details>

<details>
<summary>Close up of the mounted wiring harness for the left side.</summary>
Bokeh!

![wiring mounted](resources/dactyl-manuform-6x7-06.jpg)
</details>

<details>
<summary>Wiring harness for the right side.</summary>
It was a very sunny day

![wiring right](resources/dactyl-manuform-6x7-09.jpg)
</details>

<details>
<summary>Finished!</summary>

![Done](resources/dactyl-manuform-6x7-11.jpg)
</details>

## Firmware

For firmware flashing please refer to this page on QMK: [qmk_firmware for 6x7 Dactyl Manuform ISO-DE](https://github.com/qmk/qmk_firmware/tree/master/keyboards/handwired/dactyl_manuform/6x7/keymaps/iso-de)


## License

The source code for generating the models (everything excluding the [things/](things/) and [resources/](resources/) directories is distributed under the [GNU AFFERO GENERAL PUBLIC LICENSE Version 3](LICENSE).  The generated models and PCB designs are distributed under the [Creative Commons Attribution-NonCommercial-ShareAlike License Version 3.0](LICENSE-models).


## Original Readme
[README.orig.md](README.orig.md)


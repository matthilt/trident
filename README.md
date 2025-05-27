# BLUE

## This is a Build Log for my Voron Trident 300 mm DIY 3D Printer called "Blue"

## Colors
* Primary Color: 3dPrintLife Black
* Accent Color: 3dPrintLife Blue

## Kit

* [Formbot VORON Trident CoreXY 3D Printer Kit](https://www.formbot3d.com/products/voron-trident-corexy-3d-printer-kit-with-premade-wiring-harness)
  Dragon Standard Flow Hotend Upgrade
* [Stealthburner Extruder Upgrade Kit for Voron 2.4 or Trident](https://www.formbot3d.com/products/-176)
  I know its standard now, but my kit came with parts required for Afterburner.
* [PIF parts printed by wsebastian](https://pif.voron.dev/)

## Issues

1. Magnetic Sheet for Bed
    * When I pulled the paper backing off it pulled the glue off the magnet as well.
    * Purchased [Magnetic Flex Plate Double-Sided and Single-Sided with 3M Magnetic Backing (Energetic & West3D Collab)](https://west3d.com/products/double-sided-texture-smooth-flex-plate-with-3m-magnetic-backing-energetic-west3d-collab)
    * It said 3M on the back. Must have been more like 1.5M.
2. LEDs in Stealthburner Kit
    * My research says they are RGB but the colors are not correct. I have tried the other options in the config file. Still wrong colors.
    * I'm leaving it as it is for now. I don't really care about the colors.
    * Well I broke the LEDs by plugging them in backwards to "test." Lesson learned. Good news, another set is on the way.
    * Installed new LEDs from eBay. All is good.
3. Seems small but the hammerhead nuts that came with the kit did not want to fit in the extrusion. Most of them time I just used TNuts instead.
    
## Mods I've done
* [LDO Motors Input Shaper Kit (ADXL)](https://kb-3d.com/store/ldo/655-ldo-motors-input-shaper-kit-1661370490021.html)
* [Nevermore Micro V5 Duo](https://github.com/nevermore3d/Nevermore_Micro)
* [Decontaminator](https://github.com/LoganFraser/VoronMods/tree/main/DecontaminatorTrident/STLs)
* [20x20mm Profile Covers](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/chri.kai.in/20x20mm_Profile_Covers)
* [Chamber Thermistor](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/samwiseg0/extrusion_thermistor_mount)
* [Eddie's LED Bar Clips](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/eddie/LED_Bar_Clip)
* [Bed Fans](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/CannedBass/Trident_Bed_Fans) w/ [Ellis's Macros](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/Ellis/Bed_Fans)
      * Ehhh, seemed like too much air movement. Prints suffered
* [Top corner sealing plug for Voron Trident](https://www.printables.com/model/375617-top-corner-sealing-plug-for-voron-tridentv24)
      * Installed (with a hammer)

## Macros to check out
* A Better Print_Start Macro
* [KAMP](https://github.com/kyleisah/Klipper-Adaptive-Meshing-Purging)
* Adaptive Mesh and Purge

## To Do
* Separate config into separate files
  * Move pressure_advance from extruder.cfg to PRINT_START
  * Move pressure_advance_smooth_time to PRINT_START
* Check pwm_cycle_time in heated_bed.cfg
  *Need to PID Tune
* Finish re-doing config files a la [Mr. Zimmerman](https://github.com/EricZimmerman/Voron24)

# HIGH-TEMP AMU-FIRMWARE
This is the custom firmware for a a bed-slinger style 3D printing Automatic Manufacturing Unit (AMU). 

Key features include:
 
    Rotation Distance calculator included, to calibrate stepper motor/ extruder movements to dimensional accuracy. 
    Automated Bed Leveling: Utilizes a BL/CRTouch probe for precise bed calibration.
    Full Pin Mapping: Compatible with Creality 4.2.2 to 4.2.7 motherboards, making it easier to integrate with these popular board versions.
    Advanced Temperature Control: Includes PID tuning for consistent and accurate temperatures.

----------------------------------------------------------------------------------------------------
Compatibility

    Motherboards: Compatible with Creality 4.2.2 to 4.2.7 boards.
    Probes: Fully supports the BL/CRTouch probe for automatic bed leveling.
    Displays: Supports various LCD displays; check the lcd_type setting in the configuration file for compatibility.

----------------------------------------------------------------------------------------------------
1. Flashing the Firmware

To flash the firmware onto your printer, follow the standard procedure for your Creality board:

    Download the firmware from this repository.
    Copy the firmware file (firmware.bin) to a microSD card.
    Insert the card into your printer and power it on.
    The printer should automatically flash the firmware.

2. Calibration

After flashing the firmware, you will need to calibrate your printer, especially the BLTouch probe offsets for accurate bed leveling.

    X and Y offsets: Measure the distance from the probe’s tip to the nozzle, and set the appropriate values for x_offset and y_offset in the configuration file.
    Z offset: Adjust the Z offset to fine-tune the distance between the nozzle and the bed after X and Y offsets are set.

3. Customizing Pin Map

       If you are using a different Creality motherboard or need to adjust pin assignments, you can modify the pin mapping section of the configuration file.

----------------------------------------------------------------------------------------------------
   Required Hardware 

This firmware is made for the following hardware for enhanced printing:

    Bi-Metal Heatbreak: Enables high-temp printing, ideal for advanced materials.
    Upgraded Fans: Ensures consistent temperature control during long prints.
    High-Speed Motion: Features upgraded motors and linear rails for faster, more accurate prints.


---------------------------------------------------------------------------------------------------------------------------------------------
PLEASE USE ROTATION CALCULATOR WHEN SWITCHING MATERIALS, DIFFERENCES IN STIFFNESS OF MATERIAL WILL CAUSE DIMENSIONAL ACCURACY
----------------------------------------------------------------------------------------------------------------------------------------------

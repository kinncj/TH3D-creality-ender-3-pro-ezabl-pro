EXTRACT ALL FILES BEFORE PROCEEDING

Open firmware with Arduino IDE included. If you are on Windows double click OpenFirmwareWindows.bat to load it.

If you are on a Mac use the included Arduino Installer.

All changes are made in the Configuration.h file.

Firmware Sketch file is located in Firmware\TH3DUF_R2\TH3DUF_R2.ino

* ************** How to use this firmware - READ THIS *********************************
*
* Uncomment means removing the 2 // in front of #define.
* 
* FLASHING NOTES:
* ALL slicers (Simplify3D, Cura, Slic3r, etc) or anything else that connects to the COM port must be CLOSED for the firmware to be flash.
* If anything is connected to the COM port when flashing it will fail, typically "access denied" is listed in the error section of the Arduino IDE.
* You MUST use the Included Arduino IDE to flash the firmware if on Windows and if you are on a Mac or Linux follow the guide in our knowledgebase to setup your IDE to work with the firmware.
* 
* EZABL SETUP NOTES: 
* If you have EZABL uncomment the mount you are using with the printer. 
* If you have a custom/unsupported mount uncomment #define CUSTOM_MOUNT and enter your offsets 
* below in the CUSTOM MOUNT section. Refer to the EZABL guide to get your offsets.
* 
* STEP 1:
* Select the correct board from the tools menu for the printer you are flashing.
* Read the printer title for the model you are flashing, it will show what board to select.
*
* STEP 2:
* Uncomment the printer you want to flash. The printers are sorted A-Z by brand name.
* If you are using the CR-10S DUAL board with the Ender 3 then read the specific section below on how to do this.
*
* STEP 3: 
* Select the COM port your printer is on from the Tools menu. If you do not see the COM port try
* downloading the latest drivers from the manufacturer or TH3D site on our knowledgebase.
* 
* STEP 4:
* Verify you have the correct board selected, printer model uncommented, and if you are using EZOUT and/or EZABL
* the lines you need to use them are also uncommented.
*
* STEP 5:
* Once you have your settings verified click the arrow in the upper left to upload to the board.
*
* STEP 6:
* Reset your eeprom. You can send M502 then M500 to reset the EEPROM OR on the printer LCD go to 
* Control > Initialize EEPROM to clear out the EEPROM to defaults.
*
* BOOTLOADER FLASHING NOTES:
* For flashing your bootloader with an Uno make sure to select Arduino as ISP for the programmer
* 
* There are other features in the TH3D Extras section so look there for V6 Hotend,
* Bootscreen settings, Titan Extruder and more. You only need to edit this file.
* 
* ERROR NOTES:
* If you get errors flashing READ the message it gives you and double check that you selected
* the correct board from the Tools menu in Arduino. Turn off any AV systems and reboot the computer.
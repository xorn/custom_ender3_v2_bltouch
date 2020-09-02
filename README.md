# custom_ender3_v2_bltouch
I wasn't satisified with the options for Ender 3 V2 with BLTouch. 
I've changed only things to optimize firmware for V2 (Thanks to CHEP), enabled BLtouch ect: 
 - Enabled BLTouch - Use BLTouch port 
 - High Speed BLTouch Profile
 - Default probe offset for Jovan Kostenov's Mount - Change offset using M851 command and save to EEPROM with M500 if you use a different mount.
 -Adds G2 / G3 Arc support
 - Adds G10 / G11 Firmware based retraction (Use M207, M208, M209 to configure)
 - Adds M600 - Filament Change
 - Adds M603 - Set Filament Load / Unload length
 - Adds M701 - Load Filament
 - Adds M702 - Unload Filament
 - Enabled Advanced OK
 - Enabled CLASSIC_JERK
 - Enabled S_CURVE_ACCELERATION
 - Uses hardware EEPROM, not emulated on SD Card.

You will need to print a BLTouch mount by Jovan Kostenov

Known issues:
 - Printing files from the SD card with a filename longer than 22 characters makes the printer go crazy - Issue #18790
 - [FIXED] Z-Offset via menu might not work while printing - Issue #18787
 - [FIXED] Cancelling a print from the SD via the screen may cause the printer to stop responding. Power cycle to recover.

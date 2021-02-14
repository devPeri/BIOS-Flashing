***** Important Notice *****


You must update the IPMI firmware to version 2.0 or above first, Before upgrading this BIOS.

To disable ME (Intel Management Engine), before BIOS update starts, power down the system, and set the JPME1 and/or JPME2 (if applicable) jumpers on the motherboard to pin 2-3 location.  ***Fail to do so may result in unnecessary RMA process.***  After the BIOS update, please power down the system, and return the jumpers to their default locations (pin 1-2).


================================================
Standard BIOS Update Procedure
================================================

1. Save this BIOS update package to your computer.

2. Extract the files to a DOS bootable device (such as a bootable USB stick, or a CD).

3. Boot to a DOS prompt and type AMI.BAT BIOSname.### to start the BIOS update.

4. Do not interrupt the process until the BIOS update is complete.

5. After the message indicating BIOS update has completed, unplug the AC, clear the CMOS, and then plug in the AC, power on the system.

6. Go to the BIOS configuration, load the default setting, save and exit the BIOS.


================================================
BIOS Recovery (see user's manual for details)
================================================

Recovery BIOS with a USB Drive

If the BIOS file is corrupted and the system is not able to boot up, this feature will allow you to recover the BIOS image using a USB-attached device.  A USB flash drive or a USB CD/DVD ROM drive may be used for this purpose.  Please note that the USB hard disk drive is NOT supported at this moment.  Follow the procedure below to recover the BIOS.

1. Use a different system, copy the standard BIOS binary image file into a USB flash drive or a writable CD/DVD disc's Root Directory, and rename the file to “SUPER.ROM”.

2. While the system is turned off, insert the USB device that contains the new BIOS binary image (“SUPER.ROM”).

3. Right after powering on the system, press and hold <Ctrl> and <Home> keys together until the USB device's LED indicator comes on.  This may take a few seconds or up to one minute to start the process.

4. Once the USB device's LED is on, release the <Ctrl> and <Home> keys.  The system may generate beep codes to indicate that the BIOS ROM firmware is being reprogrammed, and a message may also be displayed on the screen.  DO NOT INTERRUPT THIS PROCESS UNTIL IT’S FINISHED!

5. After the Boot Sector Recovery Process is complete, the system will reboot automatically.

6. Boot into USB drive again.  When DOS prompt appear, please type AMI.BAT BIOSname.### to start BIOS update, just like in standard procedure.

7. Do not interrupt the process until the BIOS update is complete.

8. After you see the message of BIOS has completed the update, unplug the AC, clear the CMOS, and then plug in the AC, power on the system.  Go to the BIOS configuration, load the default setting, save and exit the BIOS.


Notes:

** There will be additional beeping after flashing the BIOS, due to the JPME1 and JPME2 jumper location changes.

*** If the BIOS flash failed, you may contact our RMA Dept. to have the BIOS chip reprogrammed.  This will require shipping the board to our RMA dept. for repair.  Please submit your RMA request at http://www.supermicro.com/support/rma/.



********* BIOS Naming Convention **********

BIOS name     : PPPPPSSY.MDD
PPPPP         : 5-Bytes for project name
SS            : 2-Bytes supplement for PPPPP
Y             : Year,  9 -> 2009, 0-> 2010, 1->2011
MDD           : Month / Date

E.g.  BIOS with the build date: 2010/1/15:
        X8ST3-F -> X8ST30.115
        X8SIL-F -> X8SIL0.115

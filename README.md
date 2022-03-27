Creality-Ender7-Klipper-Starter-Pack

Please note this is meant for intermediate to advanced users, and if you use these steps or files makes sure to thoroughly test your printer.
(make sure to have a hand on the main power to the printer to quickly shut off incase something unexpected happen)
before starting first print please go through checks to ensure movement of print head, bed is as per expectation from manual movement steps.
* individually check heated bed and hotend temps (set small values and check if temp readings are as expected)
* check functionality of all endstop
* check homing 
* check your extruder is able to extrude the instructed amount of filament (maybe an estep adjusment is required)
* perform PID tuning for heated bed and hotend
* recomended to then do pressure advance tuning


NOTE: In an ideal world the config's i provided works for you out of the box, as i have done the above steps and been testing the printer for quite some time.
      but  i hope you realize what changing the firmware does, for instance you no longer can use the lcd on the printer, so please really consider doing these steps to reduce your risks
    

      
Additional note: i have plan to integrate my raspberry pi into the printer and also connect it to the ender7's built in lcd to get some functionality out of that, its just a plan for now , however if anyone has already made any steps along that directions let me knw if u anything to share or require support ( Raech me at johnsonthomas ( a t ) d u ck ( d o t ) com

HW Info
========
printer: Ender 7
raspberry: pi zero 2w

SW Info
=======
I made use of mainsailos for my raspberry pi zero 2W, that already has all dependencies required to build the firmware as well
winscp to transfer files to and from to the raspbi
putty incase youare on windows and need to ssh

File Info
=========
* .config => The klipper config file in the klipper directory (this has the presets required for ender7 from make menuconfig)
* 2022-03-23_19h35_32.png => essential changes for klipper firmware build from make menuconfig (u could set these manually ore replace .config file mentioned above)
* 2022-03-23_19h49_44.png =>screenshot showinng the location of the .config file used by klipper firmware build step
* k06032022firmware.bin => prebuild klipper firmware for creality ender7 with the ***!!!!SAFETY CRITICAL!!!! intial pin configuration (set in .config above) to avoid the printer heated bed powering on at startup when no raspberry is connected)***
* printer.cfg => ender7 printer cfg for klipper


# ***UNDERSTAND THAT YOU MAKE USE OF THE INSTRUCTIONS HERE AT YOUR OWN RISK AND THIS IS AN UN OFFCIAL REPO AND NOT IN ANY WAY RELATED TO CREALITY***

https://github.com/nevermore3d/StealthMax

https://github.com/SanaaHamel/nevermore-controller?tab=readme-ov-file#klipper-config-minimal

https://github.com/bigtreetech/EBB/tree/master/EBB%20SB2209%20CAN%20(RP2040)

I didn't configure nevermore because it uses a lot of personal settings, and it would be easier for you to do it yourself. The second link describes config.

Things to change/calibrate before printing:
    
+ Get the serials of both boards (in Main.cfg)
+ PID tune both hotend and bed (in Main.cfg)
+ Set the right z offset for tap (in Bed-Related.cfg)
+ Find the location of the endstop (in Bed-Related.cfg)
+ Also set the z endstop offset in stepper_z (in Main.cfg)
+ Tune E steps for extruder (in Main.cfg)
+ Copy paste the controller board fan section for how many you have (in Main.cfg)
+ Check macros, I included my PRINT_START but still c: (in Macros.cfg)
+ Change printer.cfg for what end you use (mainsail or fluidd)
+ Change KAMP for what you need, I only enabled adaptive meshing since its usefull for proximity probes, TAP, PNP, NPN, etc. (in KAMP/KAMP_Settings.cfg)
+ KAMP also requires firmware retraction, set your desired settings (in FRetraction.cfg)

Easiest way to install is download as zip, and paste all the files inside the prinnter_data/config folder

-------------------------------------------------
 With love, from Suzuki

# 0w0

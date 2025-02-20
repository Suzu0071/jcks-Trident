https://github.com/nevermore3d/StealthMax

https://github.com/SanaaHamel/nevermore-controller?tab=readme-ov-file#klipper-config-minimal

https://github.com/bigtreetech/EBB/tree/master/EBB%20SB2209%20CAN%20(RP2040)

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

Download all the files in this repository to your main config location:

    git clone https://github.com/Suzu0071/jcks-Trident temp
    mv temp/.git ~/printer_data/config
    rm -rf temp
    cd ~/printer_data/config
    git checkout .
    cd

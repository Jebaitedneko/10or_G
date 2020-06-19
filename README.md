# Mido to G porting guide


# Pre-Requisites (To be done only once)


1. Download this file: https://github.com/Jebaitedneko/mido_G_autoporter/archive/master.zip


2. Download a treble mido rom (3.18 kernel) of your choice.


3. Install the recovery (OFX_R10.1_MIDO_PORT.img) from the recoveries folder. You need to be on this recovery.


4. Copy vendor_1G_repartition.zip, env_updater.zip, audio_fix.zip, cam_fix_encrypted.zip and cam_fix_decrypted.zip to sdcard.


5. Flash vendor_1G_repartition.zip from recovery. Use volume buttons to interact with the repartition zip tool. Follow the next instructions carefully.


6. During flashing, select 1GB (1024mb) AFTER DATA.


7. DO NOT SELECT SYSTEM.


8. If you get asked to format data during the vendor zip flashing, allow it using volume buttons.


9. 1GB Vendor partition will be created.


10. If it shows failed to mount data and vendor, you need to go to menu -> manage partitions -> select vendor -> repair fs.


11. If it still fails, then go to menu -> manage partitions -> select vendor -> change fs -> ext2 and then again change fs -> ext4. Do the same for data partition.


# ROM Installation (To be done every time)


Grab my latest kernel release from here: https://github.com/Jebaitedneko/android_kernel_10or_G/releases
Select assets and download latest treble zip.


1. Enter recovery (OFX_R10.1_MIDO_PORT.img).


2. Wipe data system cache vendor dalvik.


3. Flash env_updater.zip.


4. Flash ROM zip.


5. Reboot recovery.


6. Flash audio_fix.zip.


7. Flash cam_fix_encrypted.zip.


8. Flash my latest kernel zip you downloaded before.


9. Reboot to system.


10. If camera doesn't work, first try opencamera. If it still doesn't work, enter recovery and install cam_fix_decrypted.zip (cam_fix_encrypted.zip should be already installed).


11. Enjoy!

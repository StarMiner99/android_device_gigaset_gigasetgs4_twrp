# android_device_gigaset_gigasetgs4_twrp
TWRP Device Tree for Gigaset GS4

Current Status:
userdata is unreadable
No OS Installed! Are you sure you wish to reboot? only disapears if you refresh sizes in backup

Blocking checks
- [x] Correct screen/recovery size
- [x] Working Touch, screen
- [-] Backup to internal/microSD <-- microsd only /data encryption breaks this
- [-] Restore from internal/microSD <--- /\
- [x] reboot to system
- [x] ADB




Medium checks
- [ ] update.zip sideload <-- normal adb probably broke this one (worked before)
- [x] UI colors (red/blue inversions)
- [x] Screen goes off and on
- [-] F2FS/EXT4 Support, exFAT/NTFS where supported <-- f2fs not working. Fat32 is also working
- [x] all important partitions listed in mount/backup lists <-- need to press "refresh sizes" to load the partition sizes.
- [?] backup/restore to/from external (USB-OTG) storage (not supported by the device) <-- probably yes
- [x] backup/restore to/from adb (https://gerrit.omnirom.org/#/c/15943/)
- [ ] decrypt /data
- [-] Correct date <-- change time zone in settings. Time isnt visible due to the front camera resets after every reboot :\



Minor checks
- [x] MTP export
- [x] reboot to bootloader
- [x] reboot to recovery
- [x] poweroff <-- sometimes triggers a reboot
- [x] battery level
- [x] temperature
- [?] encrypted backups <-- cant find a button to encrypt it so i dont know
- [?] input devices via USB (USB-OTG) - keyboard, mouse and disks (not supported by the device)
- [?] USB mass storage export
- [x] set brightness
- [x] vibrate
- [?] screenshot <-- idk i have linux (there is a script for windows)
- [ ] partition SD card <-- unable to remove partition table

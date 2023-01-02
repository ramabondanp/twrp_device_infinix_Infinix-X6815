# TWRP device tree for Infinix Zero 5G (Infinix-X6815/B)

## Status

Current state of features (from [here](https://twrp.me/faq/OfficialMaintainer.html)):

### Blocking checks

- [ ] Correct screen/recovery size
- [ ] Working Touch, screen
- [ ] Backup to internal/microSD
- [ ] Restore from internal/microSD
- [ ] reboot to system
- [ ] ADB

### Medium checks

- [ ] update.zip sideload
- [ ] UI colors (red/blue inversions)
- [ ] Screen goes off and on
- [ ] F2FS/EXT4 Support, exFAT/NTFS where supported
- [ ] all important partitions listed in mount/backup lists
- [ ] backup/restore to/from external (USB-OTG) storage
- [ ] [backup/restore to/from adb](https://gerrit.omnirom.org/#/c/15943/)
- [ ] decrypt /data
- [ ] Correct date

### Minor checks

- [ ] MTP export
- [ ] reboot to bootloader
- [ ] reboot to recovery
- [ ] poweroff
- [ ] battery level
- [ ] temperature
- [ ] set brightness
- [ ] vibrate
- [ ] screenshot
- [ ] partition SD card

## Building

```bash
source build/envsetup.sh
lunch twrp_Infinix-X6815-eng
mka bootimage
```

> ***NOTE: For OrangeFox/TWRP builds, you can build recovery with [this patch](https://github.com/ItsVixano/android_bootable_recovery/commit/d8f3043a212e15db63ccf76ea0f09a55308e2bdf) if you want to get 60FPS on recovery***


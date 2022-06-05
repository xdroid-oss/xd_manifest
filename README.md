![XD](https://github.com/xyz-prjkt/xyz_assets/raw/main/begins.png)
# xdroidOSS | xdroid Open Source Software
a android based on AOSP with Minimalist UI Design.

### Requirements
- Around 500GB disk space.
- Around 18GB RAM running Linux.

### Sync our source ###
```bash
repo init -u https://github.com/xdroid-oss/xd_manifest -b twelve-dev
```
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build our source ###
```bash
. build/envsetup.sh
lunch xdroid_$devicecodename-userdebug
make xd -j$(nproc --all)
```

### Documentations ###
#### Settings
Our settings need to overlayed in device tree, you need to define your device information for our about phone section.
Reference
```bash
https://github.com/xdroid-devices/xd_device_xiaomi_lavender/commit/a94de499460e5a84aeb4cdac0c4e82ce5d88de4f
```
#### Bootanimations
Our build system need to defined about your resolution in device tree .mk e.g xdroid_lavender.mk by adding XDROID_BOOT := 1080.
We have 3 variant boot resolution ( 720, 1080, 1440 )

If u have a problem with boot animation ( some device with low ram have that issue ), u didn't need to define XDROID_BOOT, it will be automatically using legacy of XD bootanimation
Reference
```bash
https://github.com/xdroid-devices/xd_device_xiaomi_lavender/commit/6f2ed2af8ee5a6165ffd231d368b03cbee5e3989
```
### Credits ###
 * [**AOSP**](https://android.googlesource.com)
 * [**CAF**](https://source.codeaurora.org)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**POSP**](https://github.com/PotatoProject)
 * [**StatixOS**](https://github.com/StatiXOS)
 * [**WeebProject**](https://github.com/WeebProject)
 * [**AOSPMasterVayu**](https://github.com/AOSP-Master-Vayu)
 * [**AEX**](https://github.com/AospExtended)

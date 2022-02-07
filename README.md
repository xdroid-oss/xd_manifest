![XD](https://github.com/xyz-prjkt/xyz_assets/raw/main/begins.png)
# xdOSS | xdroid Open Source Software
a android based on AOSP with Minimalist UI Design.

### Requirements
- Around 500GB disk space.
- Around 18GB RAM running Linux.

### Sync our source ###
```bash
        repo init -u https://github.com/xdroid-oss/xd_manifest -b twelve
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

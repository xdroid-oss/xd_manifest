![banner](https://raw.githubusercontent.com/xdroid-oss/.github/55654e4a1b88977f60e2116d7cbeed17e87f450b/banner.png)
# xdroidOSS | xdroid Open Source Software
a android based on AOSP with Minimalist UI Design.

## Sync our source
```bash
repo init -u https://github.com/xdroid-oss/xd_manifest -b fifteen --git-lfs
```
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
## Building the System

Initialize the ROM environment with the envsetup.sh script.

```bash
. build/envsetup.sh
```

Lunch your device after cloning all device sources if needed.

```bash
lunch xdroid_$devicecodename-aosp_target_release-buildtype
```

Start compilation

```bash
mka xd
```

---

Note:  

**aosp_target_release**: bp1a (As of April ASB)  
**buildtype**: user, userdebug, eng

![footer](https://github.com/xdroid-oss/.github/raw/main/footer.png)

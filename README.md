<img src="https://raw.githubusercontent.com/RevengeOS-Revived/android_manifest/r11.0/assets/banner.jpg"> 

## Build the ROM!
To get started with the building process, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html).
### Initialize your local repository using this command:
```bash
repo init -u https://github.com/RevengeOS-Revived/android_manifest -b r11.0
```
### Sync the ROM sources using this command:
```bash
repo sync -c --force-sync --no-tags --no-clone-bundle -j$(nproc --all) --optimized-fetch --prune
```
### Initiate build:
```bash
source build/envsetup.sh
lunch revengeos_<devicecodename>-user
make bacon
```
&nbsp;

## Credits:
 - [AOSP](https://android.googlesource.com)
 - [LineageOS](https://github.com/LineageOS)
 - [DirtyUnicorns](https://github.com/dirtyunicorns)
 - [AospExtended](https://github.com/AospExtended)
 - [PixelExperience](https://github.com/PixelExperience)
 - [ABC](https://github.com/ezio84)

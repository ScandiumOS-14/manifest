![Scandium OS](https://raw.githubusercontent.com/ScandiumOS-14/manifest/refs/heads/14/banner.png)

Getting Started:
===============

To get started with Scandium OS, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

### Create ScandiumOS Folder ###
```bash
mkdir ScandiumOS
cd ScandiumOS
```
### Sync our source ###
```bash
repo init --depth=1 -u https://github.com/ScandiumOS-14/manifest -b 14
```
```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune
```

---------------------------------------------------------------------------------------
### Build our source ###
```bash
$ . build/envsetup.sh
$ lunch scandium_$device-userdebug
$ make bacon
```
---------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------
### Supported Flags ###
```bash
-> SCANDIUM_MAINTAINER := "Your Name"
-> SCANDIUM_BUILD_GAPPS := true/false
-> SCANDIUM_BUILD_TYPE := OFFICIAL/UNOFFICIAL
-> SCANDIUM_FACE_UNLOCK_SUPPORTED := true/fale
```
---------------------------------------------------------------------------------------

# Credits:

 * [**LineageOS**](https://github.com/LineageOS)
 * [**ProtonAOSP**](https://github.com/ProtonAOSP)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**ProjectBlaze**](https://github.com/ProjectBlaze)

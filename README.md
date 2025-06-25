![Scandium OS](https://raw.githubusercontent.com/ScandiumOS-14/manifest/refs/heads/14/banner.png)

Getting Started:
===============

To get started with Project Blaze, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

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
$ lunch scandium_$device-ap2a-userdebug
$ make bacon
```
---------------------------------------------------------------------------------------

# Credits:

 * [**LineageOS**](https://github.com/LineageOS)
 * [**ProtonAOSP**](https://github.com/ProtonAOSP)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**ProjectBlaze**](https://github.com/ProjectBlaze)

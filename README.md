Getting Started:
===============

To get started with Project Blaze, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

To initialize your local repository, use a command like this:

```bash
repo init --depth=1 -u https://github.com/KernelBuilding/manifest -b 14
```

Then to sync up:

```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune
```

---------------------------------------------------------------------------------------
 Compilation of Scandium OS:
 ==================

From root directory of Project, perform following commands in terminal

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

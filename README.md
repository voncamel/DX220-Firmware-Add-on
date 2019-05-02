# iBasso DX220 firmware add-on by Lurker

## Introduction
Android 8.1 for DX220 protects main partitions with [Verity](https://source.android.com/security/verifiedboot), which makes it tricky for end user to flash custom firmware. [Magisk](https://magiskmanager.com/) allows developers to alter system systemless-ly, i.e. without any direct modification of the protected parts of the firmware image. That's why my modifications for 8.1 are distributed as add-ons: you must have installed and running the original firmware, then you apply (flash over) an add-on. It makes the download smaller and update process faster!

To check the current add-on version in Android mode, go to _Settings_, _About DX220_, _Build number_ at the bottom.

**WARNING:** Add-ons are *not* compatible with encrypted devices!
**WARNING:** Do *not* update Magisk via MagiskManager! It will cause problems!

## How to apply or update the add-on
There are two packages to choose from: either Windows-only (using included AndroidTool), or any platform (using [DX220-bootable SD-card](https://github.com/Lurker00/DX220-Firmware-Add-on/tree/master/FirmwareUpdater)). The ZIP archive with the add-on contains `readme.txt` file with full instruction. Please read and follow it.

**Note:** Updating an add-on removes additional [Magisk](https://magiskmanager.com/) modules. You'll have to re-install them after the update.

If you need Magisk Manager, please install it manually from the [official source](https://github.com/topjohnwu/Magisk/releases/).

## How to return back to the official firmware
After iBasso released OTA-like update (1.01.092), it is enough to re-apply the update, then do a factory reset.

## Changes made
### Android
* Google Play Store added.
* [Magisk](https://magiskmanager.com/) can be used to install additional modules, and to provide root access.
* [USB Audio application](https://github.com/Lurker00/DX200-USB-Audio-Release/blob/master/README.md), which is also useful for its [System settings](https://github.com/Lurker00/DX200-USB-Audio-Release/blob/master/README.md#system-settings).
* Custom build of [HibyMusic](https://play.google.com/store/apps/details?id=com.hiby.music), which plays bit perfect PCM up to 32/384kHz with no additional efforts, and fully compatible with [USB Audio application](https://github.com/Lurker00/DX200-USB-Audio-Release/blob/master/README.md) for bit perfect DSD and SACD ISO playback.
* 126MHz CPU frequency added (216MHz is officially lowest), which is enough for most tasks.
* The process of [device registration](https://www.google.com/android/uncertified/) is much simplified (required to make Google Play Services work on uncertified device).
### Mango
* Removed Android services, that are not used in this mode.
* Performance insreased.
### Common
* Safer parameters of battery charger to prevent overheating.

## History of public releases
* [**1.18**](https://github.com/Lurker00/DX220-Firmware-Add-on/releases/tag/v1.18) - release for official firmware 1.01.092.

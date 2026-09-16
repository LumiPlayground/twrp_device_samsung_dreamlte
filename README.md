# TWRP Device Tree for Samsung Galaxy S8 (Exynos)

## Notes

Decryption doesn't work

## Kernel Source

Available [here](https://github.com/LumiPlayground/android_kernel_samsung_exynos8895/tree/sep-10.0-for-twrp)

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/LumiPlayground/twrp_device_samsung_dreamlte.git -b android-12.1 device/samsung/dreamlte
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_dreamlte-eng
mka recoveryimage
```

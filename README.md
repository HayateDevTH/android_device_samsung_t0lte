## How To Compile

# Create dirs
```
mkdir twrp; cd twrp
```

## Init repo
```
repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-11
```

## Clone repo
```
git clone https://github.com/HayateDevTH/android_device_samsung_t0lte -b android-11 device/samsung/t0lte
```

## Sync repo
```
repo sync -j$(nproc --all)
```

## Build
```
source build/envsetup.sh; export ALLOW_MISSING_DEPENDENCIES=true; lunch twrp_t0lte-eng; mka recoveryimage
```

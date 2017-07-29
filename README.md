## TWRP device tree for QMobile X70 (J220)

Add to `.repo/local_manifests/J220.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/qmobile/J220" name="android_device_qmobile_J220" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_J220-eng
make -j5 recoveryimage
```

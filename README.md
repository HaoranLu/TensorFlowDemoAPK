# TensorFlowDemoAPK
Before Installation, make sure you are using Android 5.0 or higher

Demo APK Download link:
https://drive.google.com/file/d/0B6JHKJylCp8ES1g0bGdVV1dCRWc/view?usp=sharing

No_tensorflow_demo Download link:
https://drive.google.com/file/d/0B6JHKJylCp8EdjZ4SWFGeU13OEU/view?usp=sharing

No_tensorflow_demo.apk is the one turn off tensorflow but keep all other functions.

If adb debugging is enabled on your Android 5.0 or later device, you may then
use the following command from your workspace root to install the APK once
built:

```bash
$ adb install -r -g path/to/the/tensorflow_demo.apk
```

Some older versions of adb might complain about the -g option (returning:
"Error: Unknown option: -g").  In this case, if your device runs Android 6.0 or
later, then make sure you update to the latest adb version before trying the
install command again. If your device runs earlier versions of Android, however,
you can issue the install command without the -g option.

If camera permission errors are encountered (possible on Android Marshmallow or
above), then the `adb install` command above should be used instead, as it
automatically grants the required camera permissions with `-g`. The permission
errors may not be obvious if the app halts immediately, so if you installed
with bazel and the app doesn't come up, then the easiest thing to do is try
installing with adb.


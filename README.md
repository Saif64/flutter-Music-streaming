# Music Streaming app

##### To run the app project first install ***fvm*** on your system.

***for IOS build it's preferred to archive from xCode and upload the symbol files to as well.***

## run:

```
fvm use 3.19.6
```

```
configure firebase credantials and setup the firebase project on this device
```

```
fvm flutter pub get
fvm flutter run
```

## To give build for Android

```
fvm flutter build appbundle --release --obfuscate --split-debug-info=./debug_info
fvm flutter build apk --release --obfuscate --split-debug-info=./debug_info
```

## for IOS build

```
fvm flutter build ios --release --obfuscate --split-debug-info=./debug_info
fvm flutter build ipa --release --obfuscate --split-debug-info=./debug_info
```

## for IOS upload-symbols

```
Pods/FirebaseCrashlytics/upload-symbols -gsp Runner/GoogleService-Info.plist -p ios build/Runner.xcarchive/dSYMs
```
 
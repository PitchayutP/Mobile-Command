### Keytool

```shell
keytool -genkey -V -keystore key.keystore -keyalg RSA -keysize 2048 -validity 10000 -alias keys
```

### Jarsigner

```shell
jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore key.keystore EVPTTB-1.00.02-145-debug.apk keys
```

### Zipalign
```shell
zipalign -v 4 EVPTTB-1.00.02-145-debug.apk signed.apk
```
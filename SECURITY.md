# Security

To report a security problem in Notevine, use **Report a vulnerability** on the [Security tab](https://github.com/BBallBoyDaBoss/notevine-releases/security/advisories/new) of this repository. The report stays private until a fix is out.

Do not post security problems as public issues. Include the app version (Settings, Help and about), your Android version, and the steps to reproduce.

## Check a download

Every APK is signed with the same Notevine key. The signing certificate's SHA-256 fingerprint is:

```
a0:cb:eb:c4:7e:a3:ff:2b:90:ef:ab:a8:01:d6:a2:cb:7e:e1:0f:18:65:f8:b6:cf:67:be:1e:d8:d1:4e:f1:c2
```

To check an APK on a computer with the Android SDK, run `apksigner verify --print-certs Notevine.apk`. The line `Signer #1 certificate SHA-256 digest` must match the fingerprint above, without the colons.

The release notes also list the file's own SHA-256 checksum. That checks the download, and the fingerprint checks who signed it.

# HoldFast Wallet — signed APK releases

**HoldFast Wallet** (`app.aroundtheblock.wallet`, formerly ATB Wallet for DigiByte (DGB) and DigiByte Mobile) is a
self-custody DigiByte wallet for Android, published by **Around The Block LLC**. It is not published by the DigiByte project.

- **Install from Google Play** (recommended): https://play.google.com/store/apps/details?id=app.aroundtheblock.wallet
- **Or install the signed APK** from the [releases](../../releases) of this repository. Play installs and these APKs are
  signed with the same key, so either one can update the other.
- **Source code:** https://github.com/JohnnyLawDGB/digibytewallet-android
- **More, including moving from the old DigiByte Wallet (`io.digibyte`):** https://digiscope.me/wallet

This repository holds release artifacts only. The sideload build's update check reads its releases.

## Verify an APK before installing

Every APK here is signed by this certificate:

```
SHA-256: 7E:36:DD:B2:85:61:B7:85:6A:D0:B6:27:BF:15:65:39:F8:B5:7F:97:24:21:48:D5:65:09:0C:B0:AA:8E:DF:87
```

```sh
sha256sum aroundtheblock-wallet-v<version>.apk        # must match the SHA-256 in the release notes
apksigner verify --print-certs aroundtheblock-wallet-v<version>.apk
# "Signer #1 certificate SHA-256 digest: 7e36ddb28561b7856ad0b627bf156539f8b57f97242148d565090cb0aa8edf87"
```

An app that looks like this one but is signed by anything else is not ours.

Experimental, open-source software provided as is, with no warranty. You hold your own keys, and nobody can recover them
or reverse a transaction. Terms: https://digiscope.me/wallet/terms · Privacy: https://digiscope.me/wallet/privacy-policy

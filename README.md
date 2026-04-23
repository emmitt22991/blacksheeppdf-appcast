# Black Sheep PDF — Update Feed

This public repo hosts the Sparkle auto-update feed (`appcast.xml`) for [Black Sheep PDF](https://github.com/emmitt22991/blacksheeppdf), which is a private repo.

- **Appcast URL (what the app checks):** https://emmitt22991.github.io/blacksheeppdf-appcast/appcast.xml
- **Raw fallback:** https://raw.githubusercontent.com/emmitt22991/blacksheeppdf-appcast/main/appcast.xml

Updates are pushed here automatically by the main repo's release workflow on every `v*.*.*` tag. DMG binaries live in the main repo's GitHub Releases and are signed with a Developer ID certificate and notarized by Apple; the appcast entries carry an EdDSA signature that Sparkle verifies against the `SUPublicEDKey` baked into the app's `Info.plist`.

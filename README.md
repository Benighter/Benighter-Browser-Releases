# Benighter Browser releases

Signed Android downloads and the update feed for **Benighter Browser**. Application source and signing material are private.

[Download the latest Android APK](https://github.com/Benighter/Benighter-Browser-Releases/releases/latest)

This Android preview uses a maintained Mozilla GeckoView engine with original Benighter branding and a dedicated OpenBackend account for encrypted browser sync. Browsing works without an account. Android 8 or later is required. Both ARM64 phones and x86-64 test devices are supported by the APK.

Version 0.2.0 introduces a compact browser interface with bookmark shortcuts, recent history, and System, Light and Dark appearance settings. Menus, account forms and update dialogs follow the selected theme. Websites that support a colour preference receive the same choice.

The Android 35 emulator renders dim system buttons in three-button navigation. Gesture navigation is verified; physical-phone behaviour still needs checking.

The app checks this repository for updates, verifies the APK's checksum, package, version and signing identity, and opens Android's installation confirmation. Release assets contain the APK, its SHA-256, `android-update.json` and release notes.

Encrypted sync covers bookmarks, history, normal-tab URLs, settings, saved passwords and extension inventory. Use a separate sync passphrase and keep it safe: an account password reset cannot recover encrypted data. Private tabs, website cookies/login sessions, downloaded file contents and extension internal settings stay on the device. Each encrypted collection currently has a 1 MiB protocol limit, with provider free-plan quotas also applying. Verification and recovery-email delivery are not yet established for this preview.

Firefox-compatible Mozilla-signed extensions require explicit installation and permission review. Chrome CRX extensions and automatic Chrome/Kiwi profile migration are not supported. A Windows browser is planned separately. The first preview has emulator verification and is not a complete browser-security audit or a physical-phone test.

GeckoView is Mozilla's engine, distributed unmodified under the [Mozilla Public License 2.0](https://www.mozilla.org/MPL/2.0/) and its bundled third-party licenses. The app's About screen opens the engine notices. Matching [GeckoView artifacts and Java sources](https://maven.mozilla.org/maven2/org/mozilla/geckoview/geckoview/158.0.20261007201254/) and [Firefox release sources](https://archive.mozilla.org/pub/firefox/releases/) are available from Mozilla. Benighter Browser is independent of Mozilla, Kiwi and Google.

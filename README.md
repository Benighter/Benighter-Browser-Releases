# Benighter Browser releases

Signed Android downloads and the update feed for **Benighter Browser**. Application source and signing material are private.

[Download the latest Android APK](https://github.com/Benighter/Benighter-Browser-Releases/releases/latest)

This Android preview uses a maintained Mozilla GeckoView engine with original Benighter branding and a dedicated OpenBackend account for encrypted browser sync. Browsing works without an account. Android 8 or later is required. Both ARM64 phones and x86-64 test devices are supported by the APK.

Version 0.4.0 separates account sign-in from encrypted sync: choose Turn on sync or Not now, then create or unlock your vault only when you want to sync. Google sign-in is configured as a preview; its interactive account test stalled and remains unverified. Email sign-up, sign-in and encrypted sync passed native emulator checks. The Kiwi-style top-right menu, grouped settings, clean bottom edge and charcoal Dark / Light / System themes remain. Google is the default search provider, with alternatives available. The browser interface contains no ads or sponsored placements.

Built-in filtering blocks known advertising and tracker domains in normal and private tabs, with a per-site pause control. First-party and video ads may remain; uBlock Origin is available in the searchable extension store. ZIP / XPI file installation requires a Mozilla-signed Firefox Android extension. Chrome Web Store, CRX and unsigned ZIP packages are incompatible; some desktop extension APIs are unavailable on Android.

The Import browser data screen previews bookmark HTML / JSON, Chrome Takeout ZIP / history JSON and password CSV exports before saving. Existing entries are kept and duplicates skipped. Password imports require a device screen lock. Chrome Sync is restricted to Google Chrome: signing in with the same email does not transfer Chrome data. Export data from the original browser, then import the files into Benighter.

The app checks this repository shortly after opening or returning to the app and every 15 minutes while you browse. It verifies the APK's checksum, package, version and signing identity, then opens Android's installation confirmation. Rapid app switching is throttled, and dismissed update prompts have a one-day cooldown. Release assets contain the APK, its SHA-256, `android-update.json` and release notes.

Encrypted sync covers bookmarks, history, normal-tab URLs, settings, saved passwords and extension inventory. Use a separate sync passphrase and keep it safe: an account password reset cannot recover encrypted data. Private tabs, website cookies/login sessions, downloaded file contents and extension internal settings stay on the device. Each encrypted collection currently has a 1 MiB protocol limit, with provider free-plan quotas also applying. Verification and recovery-email delivery are not yet established for this preview.

Extensions require explicit permission review. Website cookies, sign-ins and payment cards cannot be imported. A Windows browser is planned separately. This preview has Android emulator verification; physical-phone coverage and a complete browser-security audit remain pending. Bundled advertising / tracking domain lists are provided by the [Block List Project](https://github.com/blocklistproject/Lists) under its upstream license, available from About Benighter.

GeckoView is Mozilla's engine, distributed unmodified under the [Mozilla Public License 2.0](https://www.mozilla.org/MPL/2.0/) and its bundled third-party licenses. The app's About screen opens the engine notices. Matching [GeckoView artifacts and Java sources](https://maven.mozilla.org/maven2/org/mozilla/geckoview/geckoview/158.0.20261007201254/) and [Firefox release sources](https://archive.mozilla.org/pub/firefox/releases/) are available from Mozilla. Benighter Browser is independent of Mozilla, Kiwi and Google.

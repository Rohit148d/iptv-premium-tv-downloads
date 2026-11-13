# IPTV Premium TV — Fire TV downloads

Signed Android TV / Android-based Fire TV app. This public repository contains the installation APK, checksum and public signing certificate. Application source and signing keys are managed separately.

Version: **1.0.0**, Android **6.0/API 23+**. Fire OS 5 and non-Android Vega OS devices are unsupported. No IPTV subscription or media catalog is supplied.

## Install using Downloader

1. Install **Downloader by AFTVnews** from the Fire TV Appstore.
2. Open **Settings → My Fire TV → Developer options → Install unknown apps**, then allow **Downloader**. If Developer options is hidden, open **About**, select the device name seven times, and go back.
3. Open Downloader, enter the URL below, and select **Go**.
4. After the APK downloads, choose **Install**, then **Open**.

```text
https://github.com/Rohit148d/iptv-premium-tv-downloads/raw/refs/heads/main/app.apk
```

[Download APK](https://github.com/Rohit148d/iptv-premium-tv-downloads/raw/refs/heads/main/app.apk)

The APK contains the app's public Supabase client identifiers. It includes no service-role key, signing private key, provider account or saved user data. Use your own M3U/Xtream provider details, or sign into your existing app account.

## Verification and updates

Compare the downloaded file with **SHA256SUMS.txt**. **SIGNATURE.txt** records the release signing certificate. Future updates must use the same signing identity and a higher version code. Installing a compatible signed update preserves local app data; uninstalling removes local data.

Seventeen unit tests, Android lint, emulator HLS playback, favorite persistence and signed installation checks passed. Physical Firestick, real IPTV-provider and authenticated cross-device account tests remain outstanding. This is a sideload preview.

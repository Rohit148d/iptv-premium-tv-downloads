# IPTV Premium TV — Fire TV downloads

Signed Android TV / Android-based Fire TV app. This public repository contains the installation APK, checksum and public signing certificate. Application source and signing keys are managed separately.

## Separate Family Cable TV app

For a simpler live-TV app, install **Family Cable TV 1.0.0** using Downloader:

```text
https://tinyurl.com/rohit-family-tv
```

Large controls, automatic return to the last channel, the full selected category
in one list, direct remote channel switching, guide, favorites, M3U/Xtream sources
and existing app accounts. It installs alongside the regular app below.
[Family Cable setup and download](FAMILY-CABLE.md).

## IPTV Premium TV

Version: **1.2.0**, Android **6.0/API 23+**. Fire OS 5 and non-Android Vega OS devices are unsupported. No IPTV subscription or media catalog is supplied.

## Family TV and remote controls in 1.2.0

- **Up/Right = next channel; Down/Left = previous channel** during live playback.
- **OK** opens the large channel list. **MENU** holds optional audio, subtitle and retry controls. Live playback has no permanent Previous/Next toolbar.
- **Settings → Family Mode** enables big Watch TV / All Channels / Favorite Channels controls and last-channel startup. **Setup → Full app** returns to movies, series, guide, sources and accounts.
- Channel changes continue across internal pages and wrap at either end. Favorite-only mode cycles through saved live favorites.
- Install over the regular app; the app ID and signing key are unchanged. The separate Family Test APK is preserved unchanged and has a different app ID.

## Retained from 1.1.0

- Cinematic glass home tiles, top tabs and icon rail, provider backdrops, poster shelves and gold remote focus.
- Movie/series catalogs above 32 MiB load in streaming pages of 48 titles. Browse by category and use Previous/Next for later titles.
- Compact TV layouts and the existing M3U/Xtream, guide, favorites, episodes, playback and Supabase account features.
- Same app ID and signing certificate as 1.0. Install this update over the existing app to preserve saved sources and preferences.

## Install using Downloader

1. Install **Downloader by AFTVnews** from the Fire TV Appstore.
2. Open **Settings → My Fire TV → Developer options → Install unknown apps**, then allow **Downloader**. If Developer options is hidden, open **About**, select the device name seven times, and go back.
3. Open Downloader, enter the URL below, and select **Go**.
4. After the APK downloads, choose **Install**, then **Open**.

```text
https://tinyurl.com/rohit-iptv-tv12
```

[Download APK](https://github.com/Rohit148d/iptv-premium-tv-downloads/raw/refs/heads/main/app.apk)

The version-specific short URL redirects to the signed 1.2.0 APK and requires no sign-in.
Enter the whole short URL in Downloader's address field; it is not a numeric code.

The APK contains the app's public Supabase client identifiers. It includes no service-role key, signing private key, provider account or saved user data. Use your own M3U/Xtream provider details, or sign into your existing app account.

## Verification and updates

Compare the downloaded file with **SHA256SUMS.txt**. **SIGNATURE.txt** records the release signing certificate. Future updates must use the same signing identity and a higher version code. Installing a compatible signed update preserves local app data; uninstalling removes local data.

28 unit tests, Android lint, emulator HLS playback, favorite persistence, signed in-place upgrade, direct remote key dispatch, channel paging/wrap and Family Mode restart checks passed. Physical Firestick, real IPTV-provider and authenticated cross-device account tests remain outstanding. This is a sideload preview.

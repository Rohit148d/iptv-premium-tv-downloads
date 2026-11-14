# Family Cable TV

A separate, signed Android TV / Android-based Fire TV app focused on live TV.
It installs beside IPTV Premium TV and the older Family Test app.

## Install with Downloader

1. Open Downloader on your Firestick. Enable Install unknown apps for Downloader
   in Fire TV settings if needed.
2. Enter **https://tinyurl.com/rohit-family-tv** and select Go → Install.
3. Open **Family Cable TV**. In Setup → Account, sign in with your existing app
   account to restore saved sources and preferences. Or add an M3U link / Xtream
   Codes connection under Setup → Sources.

[Direct signed APK](https://raw.githubusercontent.com/Rohit148d/iptv-premium-tv-downloads/family-cable-v1.0.0/family-cable.apk)

Version **1.0.0**, version code **1**, application ID
`com.rohit148d.iptvpremium.cable.tv`. Android API 23+ is required. Devices using
non-Android Vega OS or Fire OS 5 are unsupported. No IPTV subscription is supplied.

Guest sources belong to the app where they were entered. Restore through an app
account or add them once in this separate app. Uploading a playlist file requires
an app account and an Android document picker; TVs without a picker offer the
M3U-link/Xtream alternatives. Existing account playlist files restore normally.

## For everyday watching

- Open the app and the last successfully watched channel starts automatically.
- **Up / Right:** next channel. **Down / Left:** previous channel.
- **OK:** channel list. **MENU:** optional playback controls and TV setup.
- Type **66** on number buttons to jump to channel 66 after two seconds; OK
  tunes immediately and Back cancels. Without number buttons, use
  **MENU → Jump to channel** for the large on-screen keypad.
- **Back:** large TV home with Watch TV, categories, favorites and program guide.
- Hold OK on a channel to add/remove a favorite.

Every channel in the selected live category loads in one scrollable list, with
no 48-channel pages. Channel surfing stays within that selection and wraps at
either end. Last channel, category and favorite scope are encrypted on the TV
and kept independently per account/source. Hidden channels remain excluded.
Category and favorite scope also have an account backup fallback on a fresh
installation, alongside the existing saved sources, settings and live history.
An unavailable channel does not replace the last successful channel.

This app opens/resumes TV playback; it does not replace the Fire TV home screen
or override device boot/power settings. The regular app retains movie/series
features. No phone website or Roku app is modified by this release.

For future cable updates, install over Family Cable TV to keep device data.
`CABLE-SHA256SUMS.txt` and `CABLE-SIGNATURE.txt` record verification information.
No provider credentials, saved user data, service keys or private signing files
are included. Only the public Supabase client identifiers are packaged.

Parsing uses streamed safety budgets. Selections exceeding 20,000 live channels
or the response/record budgets fail clearly and keep the previous list rather
than silently truncating it. Native M3U file uploads support up to 10 MiB.

39 unit tests cover full-category loading, number entry, existing app behavior and failure
retention. Physical Firestick, real-provider and authenticated cross-device
checks remain outstanding. This is a sideload preview.

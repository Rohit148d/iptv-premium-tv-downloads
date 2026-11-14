# Release history

## 1.2.0

Adds Family TV with a large channel browser, all/favorite channel scopes, encrypted last-channel resume and easy return to the full app. The ordinary remote arrows change live channels before video controls can consume them. No permanent live Previous/Next toolbar remains; OK opens the channel list and MENU holds optional controls. Channel changes cross internal pages and wrap in both directions. Existing account/source/preferences formats and the release signing identity are retained.

Validation: 28 JVM tests and emulator key-injection checks for direct arrows, continuous browsing, first/last wrap, favorites-only viewing, Family startup and persistence. Physical hardware and real-provider tests remain outstanding.

## 1.1.0

Fixes the Response is too large failure when opening large Xtream movie and series catalogs. Records are streamed into small visible pages, with category selection and Previous/Next. Unknown bulky metadata is skipped; failed page requests retain the previous page.

Adds glass home tiles, a cinematic provider backdrop, poster shelves, metadata previews, top tabs, an icon rail and gold remote focus. A compact layout fits smaller TV viewports. Existing app accounts, playlists, category rules, favorites and preferences retain their formats. The signing certificate and application ID are unchanged.

Validation: 21 JVM tests, Android release lint, signature verification, mocked >32 MiB catalog browsing, paging, category selection, remote focus, episode playback/continuation, process-restart persistence and a signed 1.0-to-1.1 emulator upgrade. No physical Firestick, real-provider or live authenticated account test is claimed.

## 1.0.0

Initial native Android TV / Fire TV sideload preview. The original signed APK and checksum remain available in the v1.0.0 Git tag.

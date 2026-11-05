# OnCue 2.0

The updated 2.0 build uses version code 19 and application ID
`io.github.mutebutton.oncue`. It retains the current OnCue signing certificate,
so it installs over the previous version-code-17 OnCue build without resetting
settings. Much older installs with a different certificate require reinstalling;
see [signing reset](SIGNING_RESET.md).

The launcher icon now uses the approved glass media-card artwork, filling the
Android launcher mask without an inset backing. A rounded fallback serves
Android 7, and the existing signing certificate supports normal APK updates.

This update clarifies notification access and recommends unrestricted background
battery usage for more reliable timestamps on all devices, with Samsung-specific
navigation instructions. It also adds Android 7 fallback launcher icons and
checks for mismatched widget resource overrides. Widget appearance and playback
logic are unchanged. Android 12+ defaults to a 4-by-1 widget.

Verification of this update focuses on setup, settings links, resources, and a
physical Samsung widget smoke check. The previous APK passed 170 emulator checks;
that full suite is not claimed as rerun on this APK. See the release attachment
`VERIFICATION.txt` for its exact identity and validation scope.

See [known limitations](KNOWN_LIMITATIONS.md) for battery and accessibility
boundaries. Historical 1.0 remains on release/1.0.

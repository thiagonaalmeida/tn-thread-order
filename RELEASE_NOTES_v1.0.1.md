# TN Thread Order 1.0.1

Maintenance release focused on command handling, visual refresh reliability, and internal cleanup.

## Download

Download the attached file:

- `tn-thread-order-1.0.1.xpi`

## SHA256

`62199105a49c90964f2d04cb0a7c7c8cdae5ecca9907d2ca178389b05d74d21b`

## Compatibility

- Thunderbird 152.*

## Highlights

- Improved reliability of commands on collapsed threads.
- Preserved Thunderbird native collapsed-thread behavior for thread-level actions.
- Fixed visual refresh after read, unread, star, unstar, junk, and tag actions.
- Improved row action menu and direct row control handling.
- Improved collapsed thread summary updates so state changes are reflected smoothly in the preview pane.
- Hardened projected thread state matching across folders and accounts.
- Improved projected row cache validation after expand and collapse operations.
- Improved compatibility with visual extensions that consume projected row metadata.
- Removed obsolete internal code paths.
- Reduced repeated parsing during row rendering.
- Adjusted connector dot styling to better match Thunderbird native alignment.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

## Notes

This extension uses Thunderbird Experiment APIs because Thunderbird does not currently expose the required message-list internals through standard WebExtension APIs.

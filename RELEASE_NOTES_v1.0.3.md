# TN Thread Order 1.0.3

Maintenance release focused on enabling automatic updates for manually installed GitHub releases.

## Download

Download the attached XPI file from this release:

- [tn-thread-order-1.0.3.xpi](https://github.com/thiagonaalmeida/tn-thread-order/releases/download/v1.0.3/tn-thread-order-1.0.3.xpi)

## SHA256

`060e757ee7b1eebbb6626bab119e85b7ce4d5246304e4a8147427d86e9a8d05d`

## Compatibility

- Thunderbird 152.*
- Thunderbird 153.*

## Highlights

- Added self-hosted update support for manually installed releases using Thunderbird's `update_url` mechanism.
- Uses the public update manifest hosted through GitHub Pages.
- Preserves the stable TN Thread Order 1.0.2 behavior.
- No functional behavior changes were made to thread projection, collapsed-thread command handling, preview synchronization, Card View, or Table View.
- Keeps Thunderbird's default Table View appearance intact.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

After installing this version manually, future releases can be discovered through Thunderbird's add-on update mechanism using the extension's self-hosted update manifest.

## Notes

TN Thread Order was submitted to Thunderbird Add-ons, but the gallery is currently not accepting new add-ons using Experiment APIs unless they use unmodified copies of published Thunderbird API drafts. TN Thread Order depends on Thunderbird message-list internals that are not currently exposed through standard WebExtension APIs.

This release does not change the extension's core behavior. It only adds the update channel required for reliable GitHub-based distribution while the official gallery restriction remains in place.

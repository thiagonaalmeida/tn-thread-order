# TN Thread Order 1.0.2

Compatibility release focused on Thunderbird 153.0 / 153.x support, TNCode icon alignment, and preservation of the stable 1.0.1 behavior.

## Download

Download the attached XPI file from this release:

- [tn-thread-order-1.0.2.xpi](https://github.com/thiagonaalmeida/tn-thread-order/releases/download/v1.0.2/tn-thread-order-1.0.2.xpi)

## SHA256

`af781654e26f8264d04d83c91c45aee8d9588649a3151bc8ebf28a1014f35a5d`

## Compatibility

- Thunderbird 152.*
- Thunderbird 153.*

## Highlights

- Restored compatibility with Thunderbird 153.0 and Thunderbird 153.x.
- Kept Thunderbird 152.x compatibility.
- Updated the extension icon to match the current TNCode brand mark.
- Preserved the stable TN Thread Order 1.0.1 behavior for projected thread ordering.
- Preserved collapsed-thread command handling and Thunderbird native collapsed-thread semantics.
- Preserved smooth collapsed thread summary refresh in the preview pane.
- Preserved projected row state signaling for compatible visual extensions.
- Kept Thunderbird's default Table View appearance intact.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

## Notes

Thunderbird 153 did not expose a native newest-first thread projection that replaces TN Thread Order. The compatibility blocker for version 1.0.1 was the extension compatibility range in the manifest.

This extension uses Thunderbird Experiment APIs because Thunderbird does not currently expose the required message-list internals through standard WebExtension APIs.

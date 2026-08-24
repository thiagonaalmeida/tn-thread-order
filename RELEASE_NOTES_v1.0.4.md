# TN Thread Order 1.0.4

Compatibility maintenance release for Thunderbird 154.

## Download

Download the attached XPI file from this release:

- [tn-thread-order-1.0.4.xpi](https://github.com/thiagonaalmeida/tn-thread-order/releases/download/v1.0.4/tn-thread-order-1.0.4.xpi)

## SHA256

`6a5bf5e731ac866be829af40692ce4d2d41d1671e0b072f4121cb5ae29934b3d`

## Compatibility

- Thunderbird 152.*
- Thunderbird 153.*
- Thunderbird 154.*

## Highlights

- Added compatibility with Thunderbird 154.0 / 154.x.
- Thunderbird 153 and 154 source paths used by TN Thread Order were reviewed before extending the compatibility range.
- Runtime testing on Thunderbird 154 confirmed the extension loads without console errors and the newest-first thread projection remains operational.
- Preserves the stable TN Thread Order 1.0.3 behavior.
- No functional behavior changes were made to thread projection, collapsed-thread command handling, preview synchronization, Card View, or Table View.
- Keeps Thunderbird's default Table View appearance intact.
- Preserves the self-hosted update mechanism introduced in version 1.0.3.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

Users already running version 1.0.3 can receive this release through Thunderbird's add-on update mechanism after the 1.0.4 update manifest is published.

## Notes

TN Thread Order continues to use Thunderbird Experiment APIs because the message-list internals required by the extension are not currently exposed through standard WebExtension APIs.

This release is intentionally limited to Thunderbird 154 compatibility. It does not alter the extension's established functional behavior.

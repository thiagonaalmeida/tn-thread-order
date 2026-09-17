# TN Thread Order 1.0.6

Compatibility and bug-fix release for Thunderbird 156.

## Download

Download the attached XPI file from this release:

- [tn-thread-order-1.0.6.xpi](https://github.com/thiagonaalmeida/tn-thread-order/releases/download/v1.0.6/tn-thread-order-1.0.6.xpi)

## SHA256

`3ea86e5a7c174570d4c0cbea250064c187e8e81a229038cc79919525a92246dc`

## Compatibility

- Thunderbird 152.*
- Thunderbird 153.*
- Thunderbird 154.*
- Thunderbird 155.*
- Thunderbird 156.*

## Highlights

- Added compatibility with Thunderbird 156.0 / 156.x.
- Fixed double-clicking a collapsed projected thread so it opens the same newest message shown in the TN Thread Order preview and row projection.
- Preserved Thunderbird 156 native Table View account colors when a collapsed thread projects a message from a different account.
- Preserves newest-first ordering, relationship indicators, preview synchronization, context-command behavior, selection/focus handling, and Thunderbird-native Table View appearance.
- Preserves the self-hosted GitHub update mechanism introduced in version 1.0.3.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

Users already running version 1.0.5 can receive this release through Thunderbird's add-on update mechanism after the 1.0.6 update manifest is published.

## Notes

TN Thread Order continues to use Thunderbird Experiment APIs because the message-list internals required by the extension are not currently exposed through standard WebExtension APIs.

This release keeps the existing ordering and relationship behavior intact and limits functional changes to Thunderbird 156 integration plus the projected-row double-click fix.

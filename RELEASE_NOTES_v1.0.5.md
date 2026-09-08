# TN Thread Order 1.0.5

Compatibility maintenance release for Thunderbird 155.

## Download

Download the attached XPI file from this release:

- [tn-thread-order-1.0.5.xpi](https://github.com/thiagonaalmeida/tn-thread-order/releases/download/v1.0.5/tn-thread-order-1.0.5.xpi)

## SHA256

`669591e8aa7102d9e4bac5e065ceb33827e5607fa96430bfac7838e31467f181`

## Compatibility

- Thunderbird 152.*
- Thunderbird 153.*
- Thunderbird 154.*
- Thunderbird 155.*

## Highlights

- Added compatibility with Thunderbird 155.0 / 155.x.
- Updated the Table View read/unread localization IDs used by Thunderbird 155 while keeping compatibility with Thunderbird 152-154.
- Updated Card View projected read/new status metadata for Thunderbird 155.
- Updated default preference loading to avoid Thunderbird 155's blocked `jar:file:` subscript path.
- Preserves TN Thread Order's established newest-first ordering, relationship indicators, preview synchronization, context-command behavior, selection/focus handling, and native Table View appearance.
- Preserves the self-hosted GitHub update mechanism introduced in version 1.0.3.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

Users already running version 1.0.4 can receive this release through Thunderbird's add-on update mechanism after the 1.0.5 update manifest is published.

## Notes

TN Thread Order continues to use Thunderbird Experiment APIs because the message-list internals required by the extension are not currently exposed through standard WebExtension APIs.

This release is limited to Thunderbird 155 compatibility and related integration adjustments. It does not change the extension's core newest-first ordering behavior.

# TN Thread Order 1.0.7

Compatibility maintenance release for Thunderbird 157.

## Download

Download the attached XPI file from this release:

- [tn-thread-order-1.0.7.xpi](https://github.com/thiagonaalmeida/tn-thread-order/releases/download/v1.0.7/tn-thread-order-1.0.7.xpi)

## SHA256

`a69bd1170788d96af18c16ff961f0fc73dd44f1eb35182798aef0a92a5a0d4ce`

## Compatibility

- Thunderbird 152.*
- Thunderbird 153.*
- Thunderbird 154.*
- Thunderbird 155.*
- Thunderbird 156.*
- Thunderbird 157.*

## Highlights

- Added compatibility with Thunderbird 157.0 / 157.x.
- Reviewed the Thunderbird 156 and 157 source paths used by TN Thread Order before extending the compatibility range.
- Runtime testing on Thunderbird 157 confirmed the extension starts normally after restart, operates as expected, and produces no observed console errors.
- Preserves the stable TN Thread Order 1.0.6 behavior, including newest-first ordering, relationship indicators, preview synchronization, projected-row double-click handling, context-command behavior, selection/focus handling, and native Table View account colors.
- Keeps Thunderbird's default Table View appearance intact.
- Preserves the self-hosted GitHub update mechanism introduced in version 1.0.3.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

Users already running version 1.0.6 can receive this release through Thunderbird's add-on update mechanism after the 1.0.7 update manifest is published.

## Notes

TN Thread Order continues to use Thunderbird Experiment APIs because the message-list internals required by the extension are not currently exposed through standard WebExtension APIs.

This release is intentionally limited to Thunderbird 157 compatibility. It does not alter the extension's established functional behavior.

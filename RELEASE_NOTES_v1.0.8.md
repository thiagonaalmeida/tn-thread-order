# TN Thread Order 1.0.8

Command-targeting reliability and stability release for Thunderbird 157.

## Download

Download the attached XPI file from this release:

- [tn-thread-order-1.0.8.xpi](https://github.com/thiagonaalmeida/tn-thread-order/releases/download/v1.0.8/tn-thread-order-1.0.8.xpi)

## SHA256

`9c3c94af80e83c2731da4bd822c7df1203ecac9f7bc0df33cb91fa0178874cb2`

## Compatibility

- Thunderbird 152.*
- Thunderbird 153.*
- Thunderbird 154.*
- Thunderbird 155.*
- Thunderbird 156.*
- Thunderbird 157.*

## Highlights

- Fixed keyboard Reply and related message commands so they act on the message visibly represented by TN Thread Order instead of Thunderbird's underlying structural thread message.
- Hardened message-command routing across keyboard shortcuts, context menus, message-header actions, and projected multi-selection.
- Improved projected selection restoration after native Thunderbird commands, preventing stale multi-message selections from resurfacing after an operation.
- Improved immediate visual refresh after read/unread, star, and tag state changes, including projected multi-selection.
- Hardened context-menu and message-header actions such as Tags, Archive, Delete, Junk, and Not Junk so transient Thunderbird view updates cannot silently redirect an action to a different message.
- Preserves native thread/folder-scoped behavior, newest-first ordering, preview synchronization, Card View relationship indicators, and Thunderbird-native Table View appearance.
- Preserves the self-hosted GitHub update mechanism introduced in version 1.0.3.

## Validation

- Tested with Thunderbird 157 using keyboard navigation, Reply and state shortcuts, context menus, message-header controls, Enter, multi-selection, Junk/Not Junk, Archive/Delete, tags, stars, read/unread state, and rapid-navigation stress scenarios.
- Additional stress testing covered Thunderbird view refreshes and projected message targeting during rapid navigation.
- The core newest-first ordering algorithm and Thunderbird-native Table View appearance remain unchanged.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

Users already running version 1.0.7 can receive this release through Thunderbird's add-on update mechanism after the 1.0.8 update manifest is published.

## Notes

TN Thread Order continues to use Thunderbird Experiment APIs because the message-list internals required by the extension are not currently exposed through standard WebExtension APIs.

This release resolves GitHub issue #5 and does not change the extension's core newest-first ordering behavior.

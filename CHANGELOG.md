# Changelog

## 1.0.0 - 2026-06-22

Initial public release of TN Thread Order.

### Added

- Newest-first ordering for Thunderbird threaded conversations.
- Collapsed thread projection so the newest message is shown as the main thread row.
- Expanded thread projection with newest messages first.
- Card View support with relationship indicators for conversation branches.
- Table View support using Thunderbird-native row layout, icons, message states, and indentation.
- Preview pane synchronization so the displayed conversation follows the projected newest-first order.
- Click/selection handling so projected rows open the correct underlying message.
- Support for cross-account and Unified Inbox threads using Message-ID/References-aware relationship resolution.
- English and Portuguese (Brazil) localization.
- Options page for enabling/disabling list and preview behavior.

### Notes

- Compatible with Thunderbird 152.*.
- This extension uses Thunderbird Experiment APIs because Thunderbird does not currently expose the required message-list internals through standard WebExtension APIs.
- Distribution is currently handled through GitHub Releases.

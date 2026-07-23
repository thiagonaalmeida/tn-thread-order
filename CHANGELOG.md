# Changelog

## 1.0.2 - 2026-07-22

### Fixed

- Restored compatibility with Thunderbird 153.0 and Thunderbird 153.x.
- Updated the Thunderbird compatibility range while keeping Thunderbird 152.x support.

### Improved

- Updated the extension icon to match the current TNCode brand mark.
- Preserved the stable 1.0.1 behavior for projected thread ordering, collapsed-thread command handling, preview refresh, and projected row state signaling.
- Kept Thunderbird's default Table View appearance intact.

## 1.0.1 - 2026-06-28

### Fixed

- Improved context-menu command targeting for projected Thunderbird thread rows.
- Corrected visual state refresh after read, unread, star, unstar, junk, and tag actions.
- Corrected direct row button handling for read/unread, star/unstar, and junk actions on projected rows.
- Improved collapsed thread summary refresh so state changes update smoothly in the preview pane.
- Improved projected row cache validation after thread expand and collapse operations.
- Hardened collapsed thread state matching across folders and accounts.

### Improved

- Preserved Thunderbird native selection as the authority while routing projected row commands to the displayed message.
- Preserved native collapsed-thread behavior for full-thread delete, archive, move, and thread-level state operations.
- Restored Thunderbird native focus handoff after projected direct-button commands, avoiding residual focus highlights.
- Notifies compatible visual extensions when a projected row's read, flagged, or tag state changes.
- Reduced repeated parsing during row rendering.
- Removed obsolete internal code paths.
- Aligned the thread-connector dot with Thunderbird's native rail line in Card View.
- Kept Thunderbird's default Table View appearance intact.

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

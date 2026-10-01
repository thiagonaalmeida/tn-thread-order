# Changelog

## 1.0.7 - 2026-10-01

### Fixed

- Added compatibility with Thunderbird 157.0 and Thunderbird 157.x.
- Corrected projected-row multi-selection so Shift, Ctrl/Cmd, and Thunderbird's native selection mechanisms preserve the complete selected set.
- Corrected the multiple-message pane so it reflects only the messages represented by the selected TN Thread Order rows and keeps TNTO projected ordering.
- Added command-only projected selection mapping so native Thunderbird consumers resolve the messages represented by projected multi-selection without replacing the user's visual selection.

### Improved

- Applied the projected multi-selection mapping to relevant context-menu state, command routing, and multi-selection drag payload preparation.
- Reviewed the Thunderbird 156 and 157 source paths used by TN Thread Order before extending the compatibility range.
- Preserved collapsed-thread command semantics and the stable 1.0.6 newest-first ordering, relationship indicators, single-selection preview synchronization, projected-row double-click handling, selection/focus behavior, native Table View account colors, and Thunderbird-native Table View appearance.

### Notes

- Tested with Thunderbird 157.
- Runtime testing confirmed normal startup after restart, expected TN Thread Order behavior, and no observed console errors.
- Multi-selection was tested with and without GMail Labels 0.3, in Card View and Table View, using Shift and Ctrl selection; the multiple-message pane showed only the selected messages in the correct TNTO projected order.
- The correction is generic and contains no GMail Labels-specific detection, workaround, or compatibility branch.
- Delete, Archive, Move, and other destructive/message-operation paths were reviewed as part of the projected-selection mapping but were not runtime-tested specifically with GMail Labels installed.
- No changes were made to the core newest-first ordering algorithm or Thunderbird's native Table View appearance.

## 1.0.6 - 2026-09-17

### Fixed

- Added compatibility with Thunderbird 156.0 and Thunderbird 156.x.
- Fixed double-click activation on collapsed projected threads so the opened message matches the newest message shown by TN Thread Order.
- Updated Thunderbird 156 Table View account-color projection so collapsed cross-account threads keep the native color of the projected message account.

### Improved

- Preserved Thunderbird 156 native Table View account-color behavior by using the projected message's server identity.
- Preserved the stable newest-first ordering, relationship indicators, preview synchronization, context-command routing, direct row-state commands, and selection/focus behavior from version 1.0.5.

### Notes

- Tested with Thunderbird 156.
- The double-click fix resolves GitHub issue #3.
- No changes were made to the core newest-first ordering algorithm, relationship visualization, or collapsed-thread command semantics.

## 1.0.5 - 2026-09-07

### Fixed

- Restored compatibility with Thunderbird 155.0 and Thunderbird 155.x.
- Updated Table View read/unread localization IDs to match Thunderbird 155 while preserving compatibility with Thunderbird 152-154.
- Synchronized Thunderbird 155 Card View read/new status metadata with the message projected by TN Thread Order.
- Updated default preference loading for Thunderbird 155 to avoid the newly blocked `jar:file:` subscript path while preserving the existing behavior on Thunderbird 152-154.

### Improved

- Preserved the stable 1.0.4 thread ordering, relationship indicators, preview synchronization, collapsed-thread commands, selection/focus behavior, and native Table View appearance.
- Verified the Thunderbird 155 compatibility changes with runtime testing after reviewing the relevant Thunderbird 154 and 155 source changes.

### Notes

- Tested with Thunderbird 155.
- No changes were made to the core newest-first ordering algorithm or collapsed-thread command semantics.

## 1.0.4 - 2026-08-24

### Fixed

- Restored compatibility with Thunderbird 154.0 and Thunderbird 154.x by extending the supported Thunderbird version range after source review and runtime testing.

### Improved

- Preserved the stable 1.0.3 behavior with no functional changes to thread projection, collapsed-thread command handling, preview synchronization, Card View, or Table View.
- Confirmed the existing projection, selection/focus, context-command, preview, and row-state integration paths remain compatible with Thunderbird 154.

### Notes

- Tested with Thunderbird 154.
- Keeps Thunderbird's default Table View appearance intact.

## 1.0.3 - 2026-07-23

### Added

- Added self-hosted update support for manually installed GitHub releases using Thunderbird's `update_url` mechanism.

### Improved

- Preserved the stable 1.0.2 behavior with no functional changes to thread projection, command handling, preview synchronization, Card View, or Table View.

### Notes

- This release exists to enable automatic updates for users who install TN Thread Order outside Thunderbird Add-ons while new Experiment API add-on reviews remain paused for the official gallery.

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

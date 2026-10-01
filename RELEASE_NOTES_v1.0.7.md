# TN Thread Order 1.0.7

Compatibility and projected multi-selection correctness release for Thunderbird 157.

## Download

Download the attached XPI file from this release:

- [tn-thread-order-1.0.7.xpi](https://github.com/thiagonaalmeida/tn-thread-order/releases/download/v1.0.7/tn-thread-order-1.0.7.xpi)

## SHA256

`86a285068f9019c385a32f055dd4ee2c18e0d74d9a9ae1c2e584e862e8fde70b`

## Compatibility

- Thunderbird 152.*
- Thunderbird 153.*
- Thunderbird 154.*
- Thunderbird 155.*
- Thunderbird 156.*
- Thunderbird 157.*

## Highlights

- Added compatibility with Thunderbird 157.0 / 157.x after reviewing the Thunderbird 156 and 157 source paths used by TN Thread Order.
- Corrected projected-row multi-selection so Shift, Ctrl/Cmd and Thunderbird's native selection mechanisms preserve the complete selected set instead of allowing projected single-selection reconciliation to collapse it to one row.
- Keeps the multiple-message pane synchronized with the messages represented by the selected TN Thread Order rows and preserves TNTO projected ordering.
- Adds command-only projected selection mapping so native Thunderbird consumers can resolve the messages represented by a projected multi-selection without replacing the user's visual selection.
- Applies the same projected selection mapping to relevant context-menu state, command routing and multi-selection drag payload preparation.
- Preserves collapsed-thread command semantics and the established TN Thread Order 1.0.6 behavior for newest-first ordering, relationship indicators, single-selection preview synchronization, projected-row double-click handling, selection/focus behavior, native Table View account colors, and Thunderbird-native Table View appearance.
- Preserves the self-hosted GitHub update mechanism introduced in version 1.0.3.

## Validation

- Tested with Thunderbird 157 after restart with no observed console errors and normal established TN Thread Order behavior.
- Multi-selection was tested with and without GMail Labels 0.3, in both Card View and Table View, using Shift and Ctrl selection.
- The multiple-message pane displayed only the selected messages and in the correct TN Thread Order projected order.
- The correction is generic. TN Thread Order does not detect GMail Labels and contains no GMail Labels-specific workaround or compatibility branch.
- Delete, Archive, Move and other destructive/message-operation paths were reviewed as part of the projected-selection mapping but were not runtime-tested specifically with GMail Labels installed.

## Installation

1. Download the XPI file attached to this release.
2. In Thunderbird, open **Add-ons and Themes**.
3. Click the gear icon.
4. Choose **Install Add-on From File…**.
5. Select the downloaded XPI file.

Users already running version 1.0.6 can receive this release through Thunderbird's add-on update mechanism after the 1.0.7 update manifest is published.

## Notes

TN Thread Order continues to use Thunderbird Experiment APIs because the message-list internals required by the extension are not currently exposed through standard WebExtension APIs.

This release does not change the core newest-first ordering algorithm or Thunderbird's native Table View appearance.

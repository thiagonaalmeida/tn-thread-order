# TN Thread Order

**TN Thread Order** is a Thunderbird extension that makes threaded conversations easier to follow when you prefer the newest message first.

It reorders Thunderbird threads so the latest message becomes the visible main message, keeps expanded conversations newest-first, synchronizes the preview pane with the projected order, and supports both Card View and Table View.

> This repository hosts public releases, documentation, support, issues, and discussions. The extension is distributed as a packaged `.xpi` file through GitHub Releases.

## Features

- Shows the newest message as the main row in collapsed threads.
- Keeps expanded conversations ordered newest-first.
- Synchronizes Thunderbird's preview pane with the projected newest-first message.
- Preserves click/selection behavior so projected rows open the correct message.
- Supports Thunderbird Card View with relationship indicators for conversation branches.
- Supports Thunderbird Table View using Thunderbird-native layout, icons, indentation, flags, account colors, and message states.
- Handles complex threads across accounts and Unified Inbox using message headers such as `Message-ID` and `References`.
- Includes English and Portuguese (Brazil) localization.

## Compatibility

- Thunderbird **152.***.
- Thunderbird **153.***.
- Tested with Thunderbird 153.

Thunderbird's message-list internals are not fully exposed through standard WebExtension APIs, so this extension uses Thunderbird Experiment APIs.

## Installation

1. Download the latest `.xpi` file from the [Releases](../../releases) page.
2. Open Thunderbird.
3. Go to **Add-ons and Themes**.
4. Click the gear icon.
5. Choose **Install Add-on From File…**.
6. Select the downloaded `.xpi` file.
7. Confirm the installation.
8. Restart Thunderbird if needed.

Starting with version 1.0.3, manually installed GitHub releases include a self-hosted update manifest. Thunderbird can use its add-on update mechanism to detect future TN Thread Order releases published through this repository.

## Thunderbird Add-ons status

TN Thread Order was submitted to Thunderbird Add-ons, but the gallery is currently not accepting new add-ons using Experiment APIs unless they use unmodified copies of published Thunderbird API drafts.

Because TN Thread Order depends on Thunderbird message-list internals that are not currently exposed through standard WebExtension APIs, distribution is handled through GitHub Releases while that restriction remains in place.

## Options

TN Thread Order includes an options page where you can enable or disable list projection and preview ordering behavior.

## Privacy

TN Thread Order runs locally inside Thunderbird. It does not collect personal data, does not send message content to external services, does not use analytics, and does not sell or share user data.

See [PRIVACY.md](PRIVACY.md) for details.

## Support

Use [Issues](../../issues) for bug reports and [Discussions](../../discussions) for questions, feedback, and feature ideas.

When reporting a bug, include:

- Thunderbird version.
- Operating system.
- Whether you are using Card View or Table View.
- Whether the issue happens in a normal folder or Unified Inbox.
- A screenshot or short screen recording when possible.

## Sponsorship

If this extension helps your Thunderbird workflow, GitHub Sponsors support is welcome.

## License

TN Thread Order is distributed under the Mozilla Public License 2.0.

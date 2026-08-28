# Privacy Policy — NOC Toolkit

**Last updated:** August 28, 2026

## Overview

NOC Toolkit ("the extension") is a browser tool for IT and network diagnostics: IP lookup, DNS resolution, and subnet calculation. This policy explains what data the extension does and does not collect.

## What the extension does NOT do

- It does not collect, transmit, or store any personal data on our servers — we don't operate any servers.
- It does not track your browsing activity.
- It does not use analytics, telemetry, or advertising SDKs of any kind.
- It does not access the content of the web pages you visit. The extension only runs inside its own popup window.

## What data is processed, and how

When you use a feature, the extension sends a request directly from your browser to a third-party lookup service to fetch the result you asked for:

| Feature | Data sent | Sent to |
|---|---|---|
| IP Lookup | The IP address you typed, or a request for your own public IP | [ipwho.is](https://ipwho.is) |
| DNS Lookup | The domain name you typed | [Google Public DNS](https://developers.google.com/speed/public-dns/docs/doh) (`dns.google`) |
| Subnet Calculator | Nothing — this runs entirely on your device with no network request | — |

These requests go directly from your browser to the third-party service named above; NOC Toolkit itself never sees or stores this data. Each service's own privacy policy governs how they handle that request (typically standard server logs, e.g. IP address and timestamp, consistent with normal web server operation).

## Local storage

The extension uses your browser's local storage (via the `chrome.storage` API) to remember two small preferences on your own device only:
- which tab (IP / DNS / Subnet) you last had open
- which DNS record type you last selected

This data never leaves your device and is not accessible to us or to any third party.

## Permissions

The extension requests:
- `storage` — to remember the preferences described above
- Host access to `ipwho.is` and `dns.google` — the two lookup services described above

No other permissions are requested. The extension cannot read, modify, or access any other website you visit.

## Changes to this policy

If this policy changes, the "Last updated" date above will be revised. Material changes will also be reflected in the extension's Chrome Web Store listing.

## Contact

Questions about this policy can be directed to the developer via the contact information listed on the Chrome Web Store listing page.

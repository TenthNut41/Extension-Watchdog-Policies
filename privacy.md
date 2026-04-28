# Privacy Policy for Extension Watchdog

Effective date: 28th April 2026

Extension Watchdog is a Chrome extension that monitors Chrome extensions selected by the user and alerts the user if a watched extension becomes disabled, enabled again, or unavailable.

This privacy policy explains what information the extension handles, how it is used, and when it may be transmitted.

## Information the extension stores locally

Extension Watchdog stores the following information locally in the user's Chrome browser profile:

- Watched extension IDs
- Watched extension names
- Last known watched extension statuses
- Last checked timestamps
- Local notification preference
- Optional remote webhook setting
- Optional webhook URL, if the user enables remote webhook alerts
- Password credential metadata, including a PBKDF2-SHA-256 password hash, salt, iteration count, and creation timestamp

The extension does not store the plaintext password.

## How the information is used

The stored information is used only to provide the extension's core functionality:

- To remember which Chrome extensions the user has chosen to monitor
- To check whether watched extensions are enabled, disabled, or unavailable
- To show local Chrome notifications when a watched extension changes status
- To send an optional remote webhook alert when a watched extension becomes disabled
- To protect the extension settings screen with a user-created local UI password

The local UI password protects only the extension settings screen in the current Chrome profile. It is not a replacement for operating-system account security.

## Remote webhook alerts

Remote webhook alerts are off by default.

If the user enables remote webhook alerts and saves a supported webhook URL, the extension may send an alert to that webhook when a watched extension becomes disabled.

Supported webhook destinations are:

- Slack incoming webhooks
- Discord webhooks
- n8n Cloud webhooks

Remote webhook alerts are intentionally sent only when a watched extension becomes disabled. Local Chrome notifications may still report enabled-again or unavailable status changes.

A disabled-extension webhook alert may include:

- Watched extension name
- Watched extension ID
- Status
- Detection source
- Detection time
- Whether the alert is a webhook test

Webhook data is sent only to the webhook URL configured by the user.

## Information the extension does not collect

Extension Watchdog does not read, collect, store, or transmit:

- Browsing history
- Website page contents
- Cookies
- Open tabs
- Form data
- Saved passwords
- Search history
- Website activity
- Analytics or advertising identifiers

## Third-party services

The extension does not use analytics, advertising, tracking scripts, or external services by default.

The extension only contacts a third-party service if the user explicitly enables remote webhook alerts and provides a supported Slack, Discord, or n8n Cloud webhook URL.

## Data sharing

Extension Watchdog does not sell, rent, or share user data with advertisers, data brokers, or unrelated third parties.

Data is transmitted only when the user enables remote webhook alerts, and only to the user-configured webhook endpoint.

## Data retention

Extension Watchdog stores settings locally in the user's Chrome browser profile until the user changes them, clears extension data, or uninstalls the extension.

The developer does not operate a separate server for storing Extension Watchdog data.

## Security

The extension stores data locally using Chrome extension storage.

Remote webhook alerts, when enabled, require HTTPS webhook URLs. The extension does not support non-HTTPS webhook URLs.

The settings UI password is hashed using PBKDF2-SHA-256 with a random salt. The plaintext password is not stored.

## Limited Use

The use of information received from Chrome extension APIs will adhere to the Chrome Web Store User Data Policy, including the Limited Use requirements.

Information accessed through Chrome extension APIs is used only to provide the extension's single purpose: monitoring user-selected installed Chrome extensions and sending user-configured alerts.

The extension does not sell, transfer, or use this information for advertising, profiling, credit-worthiness, or any unrelated purpose.

## Changes to this policy

This privacy policy may be updated if the extension's functionality or data handling practices change.

The updated version will be posted at this same URL with a new effective date.

## Contact

For questions about this privacy policy, contact:

Extension Watchdog
autostaged@gmail.com

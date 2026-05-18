# Privacy Policy — Guest Exporter for Luma

_Last updated: 2026-05-19_

This privacy policy describes how the **Guest Exporter for Luma** Chrome extension (the "Extension") handles data.

## Short version

The Extension does not collect, transmit, sell, or store any personal data on any server. Everything happens locally in your browser.

## What the Extension does

When you click the **Export guests** button on a Luma event-manage page, the Extension:

1. Reads the event ID from the URL of the page you are on.
2. Sends authenticated requests to Luma's own servers (`luma.com` and `api2.luma.com`) using your existing browser session cookies — the same cookies your browser already sends when you load the page manually.
3. Receives the guest list from Luma, exactly as the Luma dashboard would.
4. Displays the guest list inside a modal on the page.
5. When you click **Copy**, writes the formatted text to your operating system's clipboard.
6. When you click **Download**, generates a file in your browser and saves it to your local Downloads folder.

## What data is involved

The data the Extension processes is the guest information that Luma already shows you on the event-manage page: guest names, email addresses, LinkedIn handles (if registrants provided them), companies, job titles, registration timestamps, and any custom registration question answers.

This data belongs to the event organizer (you) and the guests who registered. You are the data controller; the Extension is a passive tool that helps you move data you already have access to into a spreadsheet-friendly format.

## What we do NOT do

- We do **not** send any data to any server controlled by the Extension author.
- We do **not** include any third-party analytics, telemetry, tracking, or advertising SDKs.
- We do **not** store guest data in `chrome.storage`, `localStorage`, IndexedDB, cookies, or anywhere else after the modal is closed.
- We do **not** read or modify pages other than `https://luma.com/event/manage/*`.
- We do **not** sell, share, or transfer data to anyone.

## Permissions we request, and why

- **`clipboardWrite`** — to copy the formatted guest list to your clipboard when you click **Copy**.
- **Access to `https://luma.com/*`** — to inject the export button on your Luma event-manage page.
- **Access to `https://api2.luma.com/*`** — to fetch the guest list through Luma's own authenticated endpoints using your existing session cookies.

## Third parties

The Extension communicates only with Luma (`luma.com` and `api2.luma.com`). It does not interact with any other third party. Your interaction with Luma is governed by Luma's own privacy policy and terms of service.

## Your responsibilities

Guest data may include personal information protected by laws such as the GDPR, CCPA, or similar regulations in your jurisdiction. As the event organizer, you are responsible for handling that data lawfully — for example, only exporting it for a legitimate purpose, storing the exported file securely, and respecting your guests' rights.

## Children

The Extension is not directed at children under 13 and does not knowingly collect any data from children.

## Changes

If this policy changes, the new version will be published in this repository with an updated date at the top.

## Contact

Questions or concerns? Open an issue at **https://github.com/nursultanmj/guest-exporter-for-luma/issues**.

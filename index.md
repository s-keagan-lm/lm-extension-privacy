# LM Leads Privacy Policy

_Last updated: 2026-10-07_

LM Leads ("the extension") is a Chrome extension published by Lystrup Maher for use with its Reach CRM. This policy explains what the extension reads, where it sends it and what it keeps.

## What the extension reads

Only when you click **Capture this posting**, **Scan form** or **Mark Submitted**, the extension reads the Upwork page you are viewing:

- Job postings: title, description, budget, skills, and client details shown on the page (name, country, rating, total spent, payment-verified status).
- Proposal pages: the cover-letter and question boxes, and the text of a submitted proposal.

It does not read Upwork pages in the background, does not read any other website, and does not track your browsing.

## Where the data goes

- **Reach (Lystrup Maher's CRM).** Captured job details, drafts and submission status are sent to the Reach server you configure (default `https://lm.reach.ascnt.app`), authenticated with your personal API token. Reach stores them as part of your workspace's leads.
- **LM Upwork Watcher (Lystrup Maher's drafting service).** When you ask for a draft, the job title, description, budget, skills and client country/rating/spend are sent to the drafting service, which uses an AI model provider (Anthropic) to generate proposal text and returns it to you. **TODO: confirm this matches the watcher's retention and provider terms.**

Data is not sent anywhere else, and is not sold, rented or used for advertising.

## What is stored in your browser

- Your Reach API base URL, API token and drafting service URL, in Chrome's synced extension storage (`chrome.storage.sync`), which Chrome may sync across your signed-in devices.
- Short-lived interface state (such as which draft you last copied) in session storage, which Chrome clears when the browser session ends.

You can remove all of it by clearing the extension's settings or uninstalling it.

## Security

All traffic to Reach and the drafting service uses HTTPS. Plain HTTP is accepted only for `localhost` development servers. Keep your API token private; you can revoke it at any time in Reach under Settings > API tokens.

## Your choices

Uninstalling the extension stops all data collection. Leads and drafts already saved in Reach are governed by your Reach workspace; ask your Reach administrator to delete them.

## Not affiliated with Upwork

LM Leads is an independent tool and is not affiliated with, endorsed by or sponsored by Upwork.

## Contact

Questions about this policy: marketing@lystrupmaher.com 

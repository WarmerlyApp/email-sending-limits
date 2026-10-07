# Email sending limits by provider

What Google Workspace, Microsoft 365, Outlook.com, Zoho Mail, Hostinger Titan and GoDaddy Workspace Email say they let one mailbox send, copied from each provider's own documentation, with the source link on every row. Open data, last checked **2026-10-07**.

- [`data/limits.json`](data/limits.json), the full dataset with notes
- [`data/limits.csv`](data/limits.csv), one row per limit, easy to open in a spreadsheet

Maintained by [Warmerly](https://warmerly.com). The readable version, with advice on how many cold emails are actually safe to send, is at [warmerly.com/email-outreach/limits](https://warmerly.com/email-outreach/limits). A companion dataset covers [what Gmail, Yahoo and Outlook.com require from bulk senders](https://github.com/WarmerlyApp/bulk-sender-requirements).

## The figures

| Provider | Limit | Source |
| --- | --- | --- |
| Google Workspace (Gmail) | 2,000 messages a day (500 on trial accounts). Up to 500 external recipients per message and 3,000 external recipients a day. 100 recipients per message over SMTP for POP/IMAP users. | [Google](https://knowledge.workspace.google.com/admin/gmail/gmail-sending-limits-in-google-workspace) |
| Microsoft 365 (Exchange Online) | 10,000 recipients a day, up to 1,000 recipients per message, 30 messages a minute. | [Microsoft](https://learn.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits) |
| Outlook.com | Microsoft 365 subscribers: 5,000 recipients a day, 500 per message, 1,000 a day to people you have never emailed. Free accounts: lower, but no figure is published. | [Microsoft](https://support.microsoft.com/en-us/office/sending-limits-in-outlook-com-279ee200-594c-40f0-9ec8-bb6af7735c2e) |
| Zoho Mail | 50 to 500 external emails an hour, set dynamically by sender reputation. 1,000 an hour internal. 150 recipients per message (paid), 100 (free). | [Zoho](https://www.zoho.com/mail/help/adminconsole/rates-and-limits.html) |
| Hostinger Titan Email | Per mailbox, per hour and per day: Free 50 and 300, Business 200 and 500, Enterprise 300 and 1,000. | [Hostinger](https://www.hostinger.com/support/5326155-parameters-and-limits-of-titan-email-at-hostinger/) |
| GoDaddy Workspace Email | 500 recipients a day, 300 an hour, 200 a minute. **Unconfirmed**, see below. | [GoDaddy](https://www.godaddy.com/help/workspace-email-account-limitations-2949) |

## Read this before you rely on a number

- **These are ceilings, not safe targets.** A provider accepting 2,000 messages a day does not mean a new mailbox can send that many without being filtered. Mailbox reputation throttles you first.
- **`null` means not published**, not unlimited.
- **GoDaddy is marked `unconfirmed`.** GoDaddy's help page returns 403 to automated requests, so the figures come from search-engine summaries of that page. If you can read it, please send a correction.
- Providers change limits without notice. Each row carries its source and the dataset carries a `last_checked` date.

## Use it

The data is licensed [CC BY 4.0](LICENSE). Use it in articles, tools or spreadsheets, and credit "Warmerly (warmerly.com)" with a link back to this repository.

## Corrections

Spotted a stale or wrong figure? Open an issue or a pull request with a link to the provider's page (a quote or screenshot helps). Corrections to provider documentation links are the most useful contribution. Providers we should add are welcome too, if their limits are published.

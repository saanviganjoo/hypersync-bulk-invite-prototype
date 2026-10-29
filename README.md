# Bulk Invite via CSV: prototype

A clickable, single-file prototype of the **Bulk invite via CSV** flow for the Account Opening Status screen.
All data is mock. Nothing is sent anywhere.

**Live demo:** https://saanviganjoo.github.io/hypersync-bulk-invite-prototype/

## What it shows
- The three-dots drawer now holds **Bulk invite via CSV** and the **Automated email** toggle, which keeps the main toolbar uncluttered.
- Upload a one-column CSV headed exactly `Employee ID`. Everyone listed is invited, even if their status would normally block it.
- One validation flow: any problem (wrong header, duplicate / empty / unknown Employee ID) shows the same *Error Detected* review screen, with highlighted cells, an errored-CSV download and a Re-upload button.

## Try it
Open the demo, click **⋮ → Bulk invite via CSV**, and upload one of the files in [`sample-csv/`](sample-csv):

| File | Result |
|---|---|
| `valid.csv` | 8 valid IDs, "All records valid", Send 8 invites |
| `errors.csv` | Wrong header plus a duplicate, an unknown ID and an empty ID: Error Detected |

Mock employee IDs that exist in the prototype: `0081`, `0085`, `0088`, `0090`, `0092`, `0094`, `0097`, `0101`, `0103`, `0106`, `0110`, `0112`.

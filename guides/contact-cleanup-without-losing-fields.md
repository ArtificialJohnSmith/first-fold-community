# Clean up duplicate contacts without losing the details you need

The difficult part of cleaning an address book is deciding which records describe the same person. Two records with one shared email may belong to a household. Two identical names may belong to different people. A duplicate suggestion should start a review.

This workflow uses [ContactWeave](https://contactweave.foggyibis16.chatgpt.site/), First Fold's free vCard and CSV cleanup tool. It works from exported files. It does not connect to an account, synchronize changes or automatically merge contacts.

## 1. Export before changing anything

Export your address book from the application that currently holds it. Keep that file unchanged in a private location.

Prefer vCard when your destination supports it and you need multiple phone numbers, email addresses or custom properties. CSV is useful for inspecting simple columns, but a flattened spreadsheet can lose photos, labels and structured details.

Use a small fictional example to learn the controls before opening an important address book. ContactWeave's **Try a fictional example** is suitable for exploring the review process.

## 2. Decide what counts as the same person

Consider these fictional records:

| Record | Name | Email | Phone |
| --- | --- | --- | --- |
| A | Alex Rivera | alex@example.com | Work number |
| B | Alex R. | alex@example.com | Mobile number |
| C | Morgan Rivera | home@example.com | Household number |
| D | Jamie Rivera | home@example.com | Household number |

A and B are candidates for review. Their email matches and the names are compatible, but you should still check that the address has not been reassigned.

C and D should not be collapsed merely because they share contact details. A shared household address and phone can be valid information for two different people.

Before merging, decide which display name, organization and individual values you want to keep. Preserve both a work number and a mobile number when both remain useful.

## 3. Import and review phone normalization

Import vCard, CSV or TSV. Map spreadsheet columns before importing. Supported vCard versions are 3.0 and 4.0; 2.1 is outside this tool's supported formats.

If all local phone numbers belong to one country, choose that country before previewing normalization. For a mixed-country address book, leave the country unselected and use explicit international numbers where you know them.

Normalization is formatting assistance. It does not establish that a number is reachable or belongs to a particular person. Keep extensions distinct.

Use **Preview normalization** and review changes before applying them. A guessed country can turn a plausible local number into the wrong international number.

## 4. Review each merge field by field

Open a match candidate, or select two contacts to compare. Inspect names, emails, phones and retained properties. Approve only the merge you actually intend.

After a merge, inspect the resulting contact rather than immediately moving through the entire candidate list. In particular:

- Are both needed phone numbers still present?
- Did the right display name survive?
- Are old and current employers distinguishable?
- Have two household members stayed separate?
- Did custom fields remain meaningful?

The tool provides single-step undo for the most recent merge or normalization. That is helpful for an immediate mistake; it is not a substitute for keeping original exports.

## 5. Choose your exports deliberately

Download a **full backup JSON** before closing or reloading. It contains original file text, working records and the edit log. Keep it private: a backup and an audit log can contain contact details too.

For migration, export a clean **vCard** and inspect it in the destination application before committing a large import. Mixed vCard versions and unusual custom fields may need a compatibility check.

CSV export is intentionally lossy. It also prefixes values beginning with certain formula-like characters with an apostrophe, including international phone numbers beginning with “+”. That reduces spreadsheet formula risk but changes the exported value. Do not assume that CSV can round-trip every contact field unchanged.

An audit-only JSON records changes; it is not the restorable full backup.

## 6. Finish in the destination address book

ContactWeave leaves your source address books unchanged. Plan the destination import separately so you do not accidentally add a second copy of every existing record. Review that application's merge or import behavior first.

Working sessions are memory-only. Reloading clears them. The tool accepts up to 2,000 contacts, 5 MiB per contact file and 10 MiB per session; full-backup restore has a separate 64 MiB limit.

The reliable finish is a reviewed export plus a private recoverable backup, with no unexplained field loss.

---

Published by First Fold, the maker of ContactWeave. Features are free; support is optional. [Explore all 30 tools](https://first-fold-launch.foggyibis16.chatgpt.site/crypto-toolkit). Product instructions checked against the available workbench implementation on October 14, 2026.

# Set up an equipment checkout log you can recover later

A small equipment cupboard often needs a few answers: what is available, where it belongs, and what has gone out. A useful log also needs a way to survive a closed tab or a cleared browser.

[Stockroom](https://stockroom-local.foggyibis16.chatgpt.site/) is First Fold's free browser-local equipment catalog. It supports quantities, locations, issues, returns, QR labels and portable backups. It is a single-device workflow without team synchronization.

## 1. Decide what each catalog entry represents

Before entering items, distinguish a shared equipment type from an individually tracked asset.

For example:

- **CABLE-USBC-2M:** eight interchangeable cables stored in Drawer B
- **PROJECTOR-01:** one specific projector stored in Cabinet A
- **TRIPOD-01:** one specific tripod stored in Cabinet A

If you need to know which physical projector was issued, give each projector a separate ID and a quantity of one. A single entry called “projector, quantity 3” answers a quantity question but is less useful for distinguishing individual units.

Use stable IDs that will still make sense after moving equipment to a different shelf. Put the current shelf in the location field rather than relying on the ID to encode it forever.

## 2. Start with a physical count

Add equipment or import new items from CSV. Check the actual starting quantity against the shelf.

Use a simple fictional example: eight identical cables, three issued, one later returned.

- Starting stock: 8
- Issue: 3
- Available after issue: 5
- Return: 1
- Available after return: 6
- Still checked out: 2

The numbers are useful only if real movements are recorded. Recount when records and the shelf disagree; do not quietly adjust a number just to make the dashboard look tidy.

If you set low-stock thresholds, choose them from your actual operating needs. Review the **Low stock** view together with items that are currently checked out. A temporary shortage and a permanent loss need different responses.

## 3. Record movements as they happen

Log stock additions, issues and returns. Review **Checked out** and the activity log at a regular point in your working day.

Keep one editing tab. Without synchronization, two tabs or devices can develop different versions of the inventory. For a shared cupboard, designate one record keeper or a clear handover process.

The tool is useful for a small local workflow. If multiple staff need simultaneous editing, permissions and an authoritative shared record, evaluate a system designed for that job.

## 4. Print labels with the right expectation

Stockroom can produce QR labels. These encode **STOCKROOM:ID**, not a public item-record URL.

That matters: scanning a label with an arbitrary phone camera does not create a hosted, synchronized checkout page. Treat the code as an identifier for your process.

Inspect a sample label at the size you will actually print. Check readability, the equipment ID and the printed name. Labels may expose equipment details to anyone who can see them, so choose names appropriate for the setting.

## 5. Make a full backup before you need one

In-memory work is lost when the tab is refreshed or closed. Optional local saving can preserve records in that browser, but browser storage can still be cleared.

Download a **Backup ZIP** after meaningful changes and before clearing browser data. The ZIP includes records, history and photos. Store it somewhere you control, with a date in the filename.

CSV is a useful inventory summary. It is not the full backup. Keeping only a CSV may leave you without the history or photos you expected to recover.

A simple routine:

1. Record the day's final issue or return.
2. Review checked-out quantities and obvious discrepancies.
3. Export a dated ZIP backup.
4. Keep the previous good backup until you have checked the new one.
5. Before restoring any older backup, preserve the current state so you can return to it.

Treat backup files as potentially private, especially if item notes or photos reveal internal information.

## 6. Know when the workflow has outgrown the tool

The current limits are 300 items, 5,000 transactions and 60 photos. Stockroom does not provide team or cross-device sync.

Do not wait until the limit to think about record retention and handover. If you need independent staff access, a live public checkout page or centralized audit controls, those requirements go beyond this local catalog.

For a small cupboard with one record keeper, consistent IDs, honest counts and recoverable backups do most of the work.

---

Published by First Fold, the maker of Stockroom. Features are free; support is optional. [Explore all 30 tools](https://first-fold-launch.foggyibis16.chatgpt.site/crypto-toolkit). Product instructions checked against the available workbench implementation on October 14, 2026.

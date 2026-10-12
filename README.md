# First Fold Community

Free browser tools for useful everyday work, supported by optional donations.

[Explore all 30 tools](https://first-fold-launch.foggyibis16.chatgpt.site/crypto-toolkit)

This public repository is the home for documentation, volunteer testing, bug reports and feature suggestions. It contains no application source code. The tools remain on their existing hosted sites.

## Start with a real task

- **CatalogGuard:** review catalog CSV changes before an import, including blank overwrites, price swings and variant identity changes.
- **BankImport Rescue:** choose explicit date and decimal rules, review possible repeats and prepare a bank CSV for an accounting import.
- **Cutcraft:** compare one-dimensional cutting plans for bars, boards or pipes, including kerf and trim, then export a cut list.

## Help improve the tools

Try one tool with fictional or non-sensitive sample data. Follow the [volunteer testing checklist](TESTING.md), read the [known limits](KNOWN_LIMITS.md), and open a bug report with reproducible steps. Specific feature suggestions are welcome too.

**Issues are public. Never post private files, financial data, personal contact lists, payment details, passwords, API keys, seed phrases, private keys or other secrets.** Use small synthetic examples and crop or redact screenshots before posting. Do not upload real bank statements, customer records, resumes or dispute evidence. Do not post exploitable security details publicly; a private security reporting channel has not been configured here.

## Try a guided test

- [Seedloom: customers and orders](https://seedloom.foggyibis16.chatgpt.site/guides/customers-orders): use downloadable synthetic fixtures and compare expected results.
- [LaunchLens: broken links](https://launchlens.foggyibis16.chatgpt.site/guides/broken-links): use downloadable synthetic fixtures and compare expected results.

## All 30 tools

Descriptions and limitations below reflect the portfolio review dated October 12, 2026. Availability and behavior can change.

### Crypto preparation

- **[ChainKit](https://first-fold-launch.foggyibis16.chatgpt.site/)**: Check EVM or TRON address formats, compare complete addresses, convert token units exactly and split an amount.
  - Limit: A checksum does not verify ownership or the recipient’s supported asset and network.
- **[CallLens](https://call-lens.foggyibis16.chatgpt.site/)**: Read transfer, approve, transferFrom, setApprovalForAll and the three-argument safeTransferFrom layouts. Token-standard and selector ambiguities stay visible.
  - Limit: Candidate interpretation only. A recognized layout cannot prove what a transaction will do.
- **[PayoutCheck](https://payout-check.foggyibis16.chatgpt.site/)**: Review up to 2,000 USDT Ethereum recipient rows for duplicate addresses, format issues, network declarations and decimal errors. Export findings.
  - Limit: The subtotal excludes error rows but includes duplicates and other warnings. No payments are sent.
- **[PayNote](https://pay-note.foggyibis16.chatgpt.site/)**: Create an unsigned USDT Ethereum payment request with an exact amount, QR code, shareable link and printable details.
  - Limit: Links are editable, wallet support varies, and a request is not proof of payment.
- **[GasBench](https://gas-bench.foggyibis16.chatgpt.site/)**: Calculate exact Ethereum execution fees, upfront reserve and sequential transaction counts from your own gas and fee inputs.
  - Limit: Illustrative arithmetic, not a live quote. Rollup data fees and exchange charges are excluded.

### Build & data

- **[FieldLens](https://field-lens.foggyibis16.chatgpt.site/)**: Inspect JSON and compare versions with exact large numbers, changed-field paths and markers for address and amount fields.
  - Limit: A review aid, not network validation, transaction simulation or a security audit.
- **[DigestBench](https://digest-bench.foggyibis16.chatgpt.site/)**: Hash local files, UTF-8 text or hex bytes with SHA-256, SHA-512 and Ethereum Keccak-256. Compare a full checksum and download a receipt.
  - Limit: A checksum match alone does not establish authenticity or safety.
- **[EpochBench](https://epoch-bench.foggyibis16.chatgpt.site/)**: Convert seconds, milliseconds, microseconds, nanoseconds, Ethereum hex seconds and ISO dates with known offsets. Export exact batch results.
  - Limit: No timezone guessing or blockchain verification. Device time is not trusted network time.
- **[Linkfolio](https://linkfolio.foggyibis16.chatgpt.site/)**: Arrange a profile, avatar and link blocks, choose a theme and download a self-contained HTML page.
  - Limit: The editor is public; your exported page needs separate hosting. No managed page hosting or publishing account.
- **[Rowmint](https://rowmint.foggyibis16.chatgpt.site/)**: Extract HTML tables or repeating rows, review fields and download CSV or JSON. Includes a manual-install Chrome extension.
  - Limit: Collect only data you may use. Chrome extension installation remains untested; the hosted workbench processes supplied HTML.
- **[Seedloom](https://seedloom.foggyibis16.chatgpt.site/)**: Design linked tables with a repeatable seed and export up to 50,000 rows as CSV, JSON or SQLite SQL.
  - Limit: Synthetic fixtures, not anonymization. Finite unique values and device memory constrain generation.
- **[LaunchLens](https://launchlens.foggyibis16.chatgpt.site/)**: Inspect a local ZIP or folder for missing paths, broken anchors, metadata issues and basic indexing signals.
  - Limit: Does not crawl live sites, render JavaScript, verify hosting redirects or audit accessibility.

### Media & design

- **[ImageFit](https://imagefit.foggyibis16.chatgpt.site/)**: Compress or resize static JPEG, PNG and WebP files. Choose dimension bounds and inspect the exported file’s actual bytes, format and dimensions.
  - Limit: A tight limit may be impossible. Compression can reduce detail; destination rules still apply.
- **[FrameHarbor](https://frameharbor.foggyibis16.chatgpt.site/)**: Trim compatible short audio or video, resize encoded video and export profiles supported by your browser.
  - Limit: 25 MiB and 60-second inputs. Codec support varies; no MP3 encoding. Repacking preserves the full clip.
- **[MarkCrate](https://markcrate.foggyibis16.chatgpt.site/)**: Turn a raster image or monogram into an ICO, PNG icon sizes, maskable icons, manifest and installation snippets.
  - Limit: Creates web assets, not a complete PWA or a full desktop icon editor. Check the exported icons at small sizes.
- **[Cueforge](https://cueforge-subtitles.foggyibis16.chatgpt.site/)**: Edit SRT or WebVTT captions, preview offsets and drift correction, flag quality issues and export repaired files.
  - Limit: No transcription or translation. Readability checks are heuristics; advanced positioning and styling are not rendered.

### Work & money

- **[CatalogGuard](https://catalogguard.foggyibis16.chatgpt.site/)**: Compare original and edited catalogs for blank overwrites, price swings and variant identity changes. Review selected formatting fixes before export.
  - Limit: No store connection. Findings need review; this cannot guarantee an import.
- **[BankImport Rescue](https://bankimport-rescue.foggyibis16.chatgpt.site/)**: Map bank CSV, TSV or delimited TXT columns for a QuickBooks or Xero import. Choose date and decimal rules, then review exact totals and possible repeats.
  - Limit: CSV-first. No PDF, OFX, QIF or Excel import, reconciliation, or bank connection.
- **[DisputePack](https://disputepack.foggyibis16.chatgpt.site/)**: Arrange a factual worksheet and locally merged evidence PDFs for manual Stripe dispute preparation. Check output sizes and page counts before review.
  - Limit: No evidence creation, case judgment or submission. No outcome guarantee.
- **[ResumeBench](https://resume-bench.foggyibis16.chatgpt.site/)**: Build role-specific resumes with three single-column templates, selectable-text PDFs, plain text and editable JSON backups.
  - Limit: No AI writing or hiring-system guarantee. Complex-script shaping and right-to-left PDF layouts are unsupported.
- **[Quiet Ledger](https://quiet-ledger.foggyibis16.chatgpt.site/)**: Import transactions, categorize spending, set monthly budgets and savings goals, and export local records.
  - Limit: One currency per workspace. Imported activity is not a verified account balance; there is no bank sync.
- **[MinuteHarbor](https://minuteharbor.foggyibis16.chatgpt.site/)**: Track or enter work sessions, review weekly totals and create downloadable PDF invoices and CSV reports.
  - Limit: Single-user local records. Review recovered timers, invoice details and tax requirements; nothing is sent or paid.

### Files & contacts

- **[Leafpress](https://leafpress-pdf.foggyibis16.chatgpt.site/)**: Merge, reorder, rotate, remove, extract and split pages. Preview prepared outputs and optionally shrink scanned pages.
  - Limit: No OCR, secure redaction or original-text editing. Image-only shrinking loses text and document features.
- **[TwinTrail](https://twintrail.foggyibis16.chatgpt.site/)**: Scan selected files with streaming SHA-256 and optional byte comparison. Choose copies to keep and export a review list.
  - Limit: Read-only: nothing is deleted and no disk space is freed. Folder selection depends on your browser.
- **[ContactWeave](https://contactweave.foggyibis16.chatgpt.site/)**: Import vCard or CSV, inspect likely duplicates, approve merges and export clean contacts with a full backup.
  - Limit: No account sync or automatic merges. Shared names and numbers are clues; review every decision.

### Plan & organize

- **[Stockroom](https://stockroom-local.foggyibis16.chatgpt.site/)**: Record equipment, quantities, issues and returns; attach local photos and create QR labels and portable backups.
  - Limit: Single-device workflow without team sync. Limits: 300 items, 5,000 transactions and 60 photos.
- **[Cutcraft](https://cutcraft.foggyibis16.chatgpt.site/)**: Compare practical cutting arrangements for bars, boards or pipes, account for kerf and trim, and export cut lists.
  - Limit: 1D only; no sheet nesting or machine control. Heuristics do not guarantee the optimal plan. Verify dimensions.
- **[Clearpath](https://clearpath-planner.foggyibis16.chatgpt.site/)**: Build a working-day Gantt plan with finish-to-start dependencies, critical paths, baselines and portable exports.
  - Limit: Single planner, up to 200 tasks. No team collaboration or resource leveling; dates remain planning estimates.
- **[Gather Table](https://gather-table.foggyibis16.chatgpt.site/)**: Import guests, keep households together, review seating rules and arrange tables with printable lists and place cards.
  - Limit: Best-effort auto-arrange is not an optimal solver. Check capacity and conflicts; native printing varies by device.
- **[Roomkind](https://roomkind.foggyibis16.chatgpt.site/)**: Lay out one rectangular room, wall openings and furniture; compare layouts, inspect overlaps and export a measured plan.
  - Limit: One rectangular room per layout; 12 layouts, 100 objects and eight openings. Approximate 2D geometry, not irregular CAD, structural, accessibility or egress validation.

## Privacy and practical limits

Tool inputs are designed for browser-local processing. Optional device saving and exports vary by tool. Browser-local processing is not a security certification: there has been no independent security audit or full network capture across all 30 tools. Hosting logs may exist. The original 12 tools retain default-off bounded aggregate analytics; the newer 18 have no application analytics. The collection's existing opt-in launch counts cover only the original 12.

Keep backups, review generated files before use and verify consequential calculations independently. Crypto tools do not establish transaction safety, ownership or supported networks. Planning tools do not replace professional or safety checks.

## Optional support

The tools are free to use. Donations are optional; current donation options and asset/network labels are shown on the hosted collection and tool pages. There is no paid feature requirement described by this repository. Donations do not imply a support deadline or guaranteed outcome.

## Verification status

The October 12 portfolio review confirmed 30 distinct active public projects and checked the collection's 30 cards, filtering, search and recovery states. Its 83 automated checks passed. These are portfolio/collection checks, not a claim that every feature in every tool has passed end-to-end testing. See [known limits](KNOWN_LIMITS.md) for tool-specific gaps. No continuous-integration workflow is configured in this repository.

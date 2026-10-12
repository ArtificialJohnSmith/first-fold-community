# Known limits and verification gaps

Snapshot: October 12, 2026. These notes describe the reviewed state, not a current warranty.

## Portfolio-wide

- The portfolio pass checked public project status and source-level scopes and donation labels. Per-tool interactive QA largely came from the tool builders.
- Bulk anonymous HTTP reads of individual tool roots returned 403, so the review did not independently fetch and hash-match every live asset.
- The collection was inspected on desktop. Physical-device/mobile browser testing was not performed for the collection.
- There has been no independent security audit or full network capture across all 30 tools.
- No traffic, donation, conversion or profitability results have been established.
- No CI workflow is configured in this documentation repository.

## Tool-specific

### [ChainKit](https://first-fold-launch.foggyibis16.chatgpt.site/)

- Product limit: A checksum does not verify ownership or the recipient’s supported asset and network.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [CallLens](https://call-lens.foggyibis16.chatgpt.site/)

- Product limit: Candidate interpretation only. A recognized layout cannot prove what a transaction will do.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [PayoutCheck](https://payout-check.foggyibis16.chatgpt.site/)

- Product limit: The subtotal excludes error rows but includes duplicates and other warnings. No payments are sent.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [PayNote](https://pay-note.foggyibis16.chatgpt.site/)

- Product limit: Links are editable, wallet support varies, and a request is not proof of payment.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [GasBench](https://gas-bench.foggyibis16.chatgpt.site/)

- Product limit: Illustrative arithmetic, not a live quote. Rollup data fees and exchange charges are excluded.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [FieldLens](https://field-lens.foggyibis16.chatgpt.site/)

- Product limit: A review aid, not network validation, transaction simulation or a security audit.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [DigestBench](https://digest-bench.foggyibis16.chatgpt.site/)

- Product limit: A checksum match alone does not establish authenticity or safety.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [EpochBench](https://epoch-bench.foggyibis16.chatgpt.site/)

- Product limit: No timezone guessing or blockchain verification. Device time is not trusted network time.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [ImageFit](https://imagefit.foggyibis16.chatgpt.site/)

- Product limit: A tight limit may be impossible. Compression can reduce detail; destination rules still apply.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [CatalogGuard](https://catalogguard.foggyibis16.chatgpt.site/)

- Product limit: No store connection. Findings need review; this cannot guarantee an import.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [BankImport Rescue](https://bankimport-rescue.foggyibis16.chatgpt.site/)

- Product limit: CSV-first. No PDF, OFX, QIF or Excel import, reconciliation, or bank connection.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [DisputePack](https://disputepack.foggyibis16.chatgpt.site/)

- Product limit: No evidence creation, case judgment or submission. No outcome guarantee.
- QA coverage or gap: Existing service; this portfolio pass checks public access, hosted/source donation labels and asset integrity, not a repeat of every interaction.

### [ResumeBench](https://resume-bench.foggyibis16.chatgpt.site/)

- Product limit: No AI writing or hiring-system guarantee. Complex-script shaping and right-to-left PDF layouts are unsupported.
- QA coverage or gap: Core hosted flows passed; responsive checks used an iframe rather than physical devices.

### [Quiet Ledger](https://quiet-ledger.foggyibis16.chatgpt.site/)

- Product limit: One currency per workspace. Imported activity is not a verified account balance; there is no bank sync.
- QA coverage or gap: Core hosted flows passed; no full network capture or physical-device tests.

### [MinuteHarbor](https://minuteharbor.foggyibis16.chatgpt.site/)

- Product limit: Single-user local records. Review recovered timers, invoice details and tax requirements; nothing is sent or paid.
- QA coverage or gap: Core CSV and invoice tests passed; Reports tab interactive navigation is unverified.

### [Leafpress](https://leafpress-pdf.foggyibis16.chatgpt.site/)

- Product limit: No OCR, secure redaction or original-text editing. Image-only shrinking loses text and document features.
- QA coverage or gap: Functional public build checked; responsive QA and latest cosmetic wording are unverified.

### [TwinTrail](https://twintrail.foggyibis16.chatgpt.site/)

- Product limit: Read-only: nothing is deleted and no disk space is freed. Folder selection depends on your browser.
- QA coverage or gap: 15 tests and hosted file/export/cancel checks passed; native folder-picker relative paths unverified.

### [ContactWeave](https://contactweave.foggyibis16.chatgpt.site/)

- Product limit: No account sync or automatic merges. Shared names and numbers are clues; review every decision.
- QA coverage or gap: Versioned assets and byte-identical backup restore verified; no account synchronization.

### [FrameHarbor](https://frameharbor.foggyibis16.chatgpt.site/)

- Product limit: 25 MiB and 60-second inputs. Codec support varies; no MP3 encoding. Repacking preserves the full clip.
- QA coverage or gap: Seven output files independently checked; available codecs remain browser-dependent.

### [MarkCrate](https://markcrate.foggyibis16.chatgpt.site/)

- Product limit: Creates web assets, not a complete PWA or a full desktop icon editor. Check the exported icons at small sizes.
- QA coverage or gap: Real exports independently checked; optional final browser QA was not completed.

### [Cueforge](https://cueforge-subtitles.foggyibis16.chatgpt.site/)

- Product limit: No transcription or translation. Readability checks are heuristics; advanced positioning and styling are not rendered.
- QA coverage or gap: 16 tests and hosted SRT/VTT import/export, JSON restore and MP4 playback passed; 390px iframe checked. Final repeated saved-project load/erase and physical-device/cross-browser checks are unverified.

### [Linkfolio](https://linkfolio.foggyibis16.chatgpt.site/)

- Product limit: The editor is public; your exported page needs separate hosting. No managed page hosting or publishing account.
- QA coverage or gap: 36 Node tests, independent HTML parsing, basic hosted editor checks and actual HTML download passed. Downloaded-file browser rendering, avatar import and responsive checks remain unverified.

### [Rowmint](https://rowmint.foggyibis16.chatgpt.site/)

- Product limit: Collect only data you may use. Chrome extension installation remains untested; the hosted workbench processes supplied HTML.
- QA coverage or gap: Hosted demo and extraction overlay tested; actual Chrome extension installation unverified.

### [Seedloom](https://seedloom.foggyibis16.chatgpt.site/)

- Product limit: Synthetic fixtures, not anonymization. Finite unique values and device memory constrain generation.
- QA coverage or gap: Generated downloadable files verified; clipboard readback and valid-import UI unverified.

### [LaunchLens](https://launchlens.foggyibis16.chatgpt.site/)

- Product limit: Does not crawl live sites, render JavaScript, verify hosting redirects or audit accessibility.
- QA coverage or gap: Live ZIP flows and 30 independent tests passed; folder picker unverified.

### [Stockroom](https://stockroom-local.foggyibis16.chatgpt.site/)

- Product limit: Single-device workflow without team sync. Limits: 300 items, 5,000 transactions and 60 photos.
- QA coverage or gap: Core flows checked; physical devices and printers untested.

### [Cutcraft](https://cutcraft.foggyibis16.chatgpt.site/)

- Product limit: 1D only; no sheet nesting or machine control. Heuristics do not guarantee the optimal plan. Verify dimensions.
- QA coverage or gap: Core heuristic and export checks passed; native Print / Save PDF output not captured.

### [Clearpath](https://clearpath-planner.foggyibis16.chatgpt.site/)

- Product limit: Single planner, up to 200 tasks. No team collaboration or resource leveling; dates remain planning estimates.
- QA coverage or gap: Core planner checks passed; erase UI, native Print / Save PDF and final cosmetic reload unverified.

### [Gather Table](https://gather-table.foggyibis16.chatgpt.site/)

- Product limit: Best-effort auto-arrange is not an optimal solver. Check capacity and conflicts; native printing varies by device.
- QA coverage or gap: 20 tests, hosted import/restore/conflict/capacity/storage checks and actual downloads passed; 390px iframe checked. Native OS Print / Save PDF was not observed; printable HTML was verified.

### [Roomkind](https://roomkind.foggyibis16.chatgpt.site/)

- Product limit: One rectangular room per layout; 12 layouts, 100 objects and eight openings. Approximate 2D geometry, not irregular CAD, structural, accessibility or egress validation.
- QA coverage or gap: 15 tests, 500 rotation cases and hosted edit/drag/overlap/undo/restore checks passed; actual SVG independently rendered and 390px iframe checked. Physical devices and printers untested.

